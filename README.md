# 🎓 NextGen — Online Course Platform

A full-stack **online course selling & learning platform** built with **Next.js 15**. Instructors can create and sell courses, while students can purchase, enroll, and watch lessons through a modern, responsive interface — complete with authentication, secure payments, and an admin dashboard.

---

## ✨ Features

- 🔐 **Authentication** — Secure sign-up/sign-in and user management via **Clerk**
- 💳 **Payments** — Course purchases handled with **Stripe** checkout & webhooks
- 📚 **Course Management** — Create, organize, and reorder course sections/chapters using drag-and-drop (**dnd-kit**)
- 🎥 **Video Lessons** — Embedded lesson playback via **react-youtube**
- 🛡️ **Security & Rate Limiting** — Protected against bots/abuse using **Arcjet**
- 🗄️ **Database** — Type-safe queries with **Drizzle ORM** on **PostgreSQL**
- 🎨 **UI Components** — Built with **Radix UI**, **shadcn/ui**, and **Tailwind CSS**
- ✅ **Form Handling & Validation** — **React Hook Form** + **Zod**
- 🐳 **Dockerized Database** — Local PostgreSQL setup via `docker-compose`

---

## 🛠️ Tech Stack

| Category | Technology |
|---|---|
| Framework | Next.js 15 (App Router) |
| Language | TypeScript |
| Styling | Tailwind CSS, tailwindcss-animate |
| UI Components | Radix UI, shadcn/ui, Lucide Icons |
| Auth | Clerk |
| Payments | Stripe |
| Database | PostgreSQL + Drizzle ORM |
| Security | Arcjet |
| Forms | React Hook Form + Zod |
| Drag & Drop | dnd-kit |
| Video | react-youtube |
| Webhooks | Svix |

---

## 📁 Project Structure

```
nextgen/
├── public/
│   └── imgs/products/     # Course/product images
├── src/                   # Application source code (app, components, db, lib, etc.)
├── docker-compose.yml     # Local PostgreSQL container
├── drizzle.config.ts      # Drizzle ORM configuration
├── components.json        # shadcn/ui configuration
├── tailwind.config.ts
├── next.config.ts
└── package.json
```

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/sarifulrana78/nextgen.git
cd nextgen
```

### 2. Install dependencies
```bash
npm install
```

### 3. Set up environment variables
Create a `.env` file in the root directory with the required keys (Clerk, Stripe, Database URL, Arcjet, etc.):
```env
DATABASE_URL=
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
STRIPE_SECRET_KEY=
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=
ARCJET_KEY=
```

### 4. Start the local database
```bash
docker-compose up -d
```

### 5. Run database migrations
```bash
npm run db:generate
npm run db:migrate
```

### 6. Start the development server
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the app.

---

## 📜 Available Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start the development server |
| `npm run build` | Build the app for production |
| `npm run start` | Start the production server |
| `npm run lint` | Run ESLint |
| `npm run db:generate` | Generate Drizzle migration files |
| `npm run db:migrate` | Apply database migrations |
| `npm run db:studio` | Open Drizzle Studio (DB GUI) |

---

## 📸 Screenshots

> *Add screenshots/GIFs of the course catalog, checkout flow, and lesson player here.*

---

## 👤 Author

**Sariful Islam Rana**
- GitHub: [@sarifulrana78](https://github.com/sarifulrana78)
- LinkedIn: [sariful-islam-rana](https://www.linkedin.com/in/sariful-islam-rana)
- Email: sarifulislam536@gmail.com

---

## 📄 License

This project is licensed under the **MIT License**.
