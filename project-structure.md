# Project Structure

```
Node-NestJS-TypeScript-PrismaORM-OpenAI-LLM/
├── backend/
│   ├── src/
│   │   ├── app.controller.ts
│   │   ├── app.module.ts
│   │   ├── main.ts
│   │   ├── database/
│   │   │   ├── database.service.ts
│   │   │   └── schema.prisma
│   │   ├── characters/
│   │   │   ├── characters.service.ts
│   │   │   └── characters.controller.ts
│   │   ├── likes/
│   │   │   ├── likes.service.ts
│   │   │   └── likes.controller.ts
│   │   ├── users/
│   │   │   ├── users.service.ts
│   │   │   └── users.controller.ts
│   │   ├── openai/
│   │   │   └── openai.service.ts
│   │   ├── guards/
│   │   │   └── api-key.guard.ts
│   │   └── interfaces/
│   │       └── character.interface.ts
│   ├── prisma/
│   │   ├── seed.ts
│   │   └── migrations/
│   ├── package.json
│   ├── tsconfig.json
│   ├── nest-cli.json
│   └── .env
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   │   ├── layout.tsx
│   │   │   ├── page.tsx
│   │   │   ├── search/
│   │   │   │   └── page.tsx
│   │   │   ├── characters/
│   │   │   │   └── page.tsx
│   │   │   └── globals.css
│   │   ├── components/
│   │   │   ├── CharacterCard.tsx
│   │   │   ├── SearchBox.tsx
│   │   │   └── LikeButton.tsx
│   │   └── lib/
│   │       └── api.ts
│   ├── package.json
│   ├── next.config.js
│   ├── tailwind.config.js
│   ├── tsconfig.json
│   └── .env.local
├── docs/
│   ├── API.md
│   └── SETUP.md
├── .gitignore
├── README.md
├── docker-compose.yml
└── package.json (root)
```
