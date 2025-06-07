# 🛍️ MiPyme E-Commerce Backend — NestJS & Prisma

[View API Docs](https://github.com/tuusuario/mipymeecomerc-backend#readme)

## 📌 Description

This project is **the backend for the Cuban MiPyme e-commerce platform**, implemented with **NestJS**, **Prisma** and **JWT authentication**. It provides a robust, type-safe API for:

- Vendor management (products, inventory, sales)  
- Customer flows (signup, login, cart, orders)  
- Secure, stateless auth via JWT  

Designed to pair with the Angular frontend, it exposes RESTful endpoints and real-time events (via WebSockets) for order updates.

## 🛠️ Technologies

- **Node.js & NestJS** (modules, DI, pipes)  
- **TypeScript** (strict mode)  
- **Prisma ORM** (schema-first, migrations)  
- **PostgreSQL** (relational data)  
- **@nestjs/jwt** & **Passport.js** (JWT auth)  
- **class-validator** & **class-transformer** (DTOs & validation)  
- **Socket.IO** (order status notifications)

👉 Browse the code here:  
[🔗 github.com/tuusuario/mipymeecomerc-backend](https://github.com/tuusuario/mipymeecomerc-backend)

## 🎨 Why Is It Interesting?

- **Type-safe data layer**: Prisma schema generates typed client for safer queries.  
- **Modular design**: clear separation of auth, users, products, orders, and vendors.  
- **JWT-based security**: stateless, scalable authentication with refresh tokens.  
- **Validation & mapping**: DTOs ensure input is sanitized and transformed.  
- **Real-time updates**: WebSockets notify vendors and customers about order progress.

Great as a template for any enterprise-grade e-commerce API or multi-tenant marketplace.

---

## 🚀 How to Run It

1. **Clone the repo**  
   ```bash
   git clone https://github.com/tuusuario/mipymeecomerc-backend.git
   cd mipymeecomerc-backend
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure environment**
   Copy `.env.example` → `.env` and set:

   ```env
   DATABASE_URL="postgresql://USER:PASSWORD@HOST:PORT/DBNAME?schema=public"
   JWT_SECRET="your-jwt-secret"
   JWT_EXPIRES_IN="3600s"
   ```

4. **Generate Prisma client & migrate**

   ```bash
   npx prisma migrate dev --name init
   npx prisma generate
   ```

5. **Run the development server**

   ```bash
   npm run start:dev
   ```

6. **Explore the API**
   Open [http://localhost:3000/api](http://localhost:3000/api) for Swagger docs.

---

## 📣 Note

This backend is designed to work seamlessly with the Angular frontend at `https://github.com/tuusuario/mipymeecomerc-frontend`. Ensure CORS and API URLs match.

---

## 📌 Author

Developed by **HollowDude**.
Issues, feedback, and PRs are welcome—please fork or open an issue!

```
```
