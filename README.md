# ShopSphere

A full-stack e-commerce learning project built for the CodeAlpha Full Stack Development internship.

## Features
- Product catalogue with search and category filtering
- Product details and persistent shopping cart
- Registration and login with bcrypt password hashing
- JWT-protected checkout and order history
- SQLite database with seeded sample products
- Responsive interface and REST API

## Stack
Node.js, Express, SQLite (better-sqlite3), HTML, CSS and vanilla JavaScript.

## Run locally
```bash
npm install
cp .env.example .env
# Set a long random JWT_SECRET in .env
npm run dev
```
Open http://localhost:3000.

## API
- POST /api/auth/register
- POST /api/auth/login
- GET /api/products
- GET /api/products/:id
- POST /api/orders (authentication required)
- GET /api/orders (authentication required)
- GET /api/health

The database is created automatically in data/app.db. Never commit .env or database files. This is an educational internship project; review and test before production use.
