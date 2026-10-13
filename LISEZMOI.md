# TP Authentification (Next.js 15 + Prisma 6 + SQLite)

Toutes les parties du TP sont déjà codées. Pour lancer :

```powershell
npm install
npx prisma migrate dev --name init   # crée prisma/dev.db et le dossier migrations
npm run dev
```

Ouvre http://localhost:3000

- `.env` contient déjà un JWT_SECRET aléatoire (il est ignoré par Git).
- Si tu veux le régénérer :
  `node -e "console.log(require('crypto').randomBytes(32).toString('base64'))"`
- Visualiser la base : `npx prisma studio`
