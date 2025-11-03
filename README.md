# 📝 Google Docs Clone

Un clone moderne de **Google Docs** développé avec **Next.js**, **Clerk** pour l’authentification sécurisée des utilisateurs, et **Liveblocks** pour la collaboration en temps réel et les notifications de présence.  
Ce projet permet à plusieurs utilisateurs de modifier un même document simultanément, de voir les curseurs des autres participants, et de gérer leurs sessions d’authentification de manière fluide.

---

## 🚀 Fonctionnalités principales

- 🔐 **Authentification & gestion des utilisateurs** avec [Clerk](https://clerk.com)
- 🧑‍🤝‍🧑 **Collaboration en temps réel** grâce à [Liveblocks](https://liveblocks.io)
- 🧾 **Éditeur de texte riche** type Google Docs (avec `contenteditable` / `Lexical` / `Tiptap`)
- 💬 **Indicateur de présence** (avatars des utilisateurs connectés)
- 🔔 **Notifications Liveblocks** pour signaler les modifications
- 💾 **Sauvegarde automatique** des documents
- 🌙 **Interface moderne et responsive** (Next.js + Tailwind CSS)
- 🧱 **Architecture modulaire** (API Routes + App Router Next.js 15)

---

## 🧩 Stack technique

| Outil / Technologie | Description                                                |
| ------------------- | ---------------------------------------------------------- |
| **Next.js 15+**     | Framework React côté serveur et client                     |
| **Clerk**           | Authentification et gestion des utilisateurs               |
| **Liveblocks**      | Collaboration en temps réel et présence multi-utilisateurs |
| **Tailwind CSS**    | Stylisation rapide et responsive                           |
| **TypeScript**      | Typage statique pour plus de fiabilité                     |
| **Vercel**          | Déploiement serverless simple et rapide                    |

---

## ⚙️ Installation et configuration

### 1. Cloner le projet

```bash
git clone https://github.com/<ton-username>/google_docs_clone.git
cd google_docs_clone
```

### 2. Installer les dépendances

```bash
npm install
# ou
yarn install
```

### 3. Configurer les variables d’environnement

Crée un fichier .env.local à la racine du projet :

```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_***************
CLERK_SECRET_KEY=sk_test_***************
LIVEBLOCKS_SECRET_KEY=sk_test_***************

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up

SENTRY_AUTH_TOKEN=sntrys_***************
```

🔐 Les clés Clerk sont disponibles sur https://dashboard.clerk.com

🔐 Les clés Liveblocks sont disponibles sur https://liveblocks.io/dashboard/apikeys

### 4. Lancer le serveur de développement

```bash
npm run dev
```

Le projet sera accessible sur :
👉 http://localhost:3000

### 5. Lancer le serveur de développement

```bash
npm run build
npm start
```

## 💻 Déploiement sur Vercel

- Connecte ton dépôt GitHub à Vercel
- Dans les Settings → Environment Variables, ajoute :
  - NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY
  - CLERK_SECRET_KEY
  - LIVEBLOCKS_SECRET_KEY
  - NEXT_PUBLIC_LIVEBLOCKS_PUBLIC_KEY
- Clique sur Deploy

## 👤 Aimane Chanaa

Développeur Full Stack • Passionné par le Web, l’IA et la collaboration en temps réel

📧 Contact : [aimanechanaa@gmail.com]

🌐 GitHub : https://github.com/AymanChanaa
