# Ikifurni

online store for home product furniture

## Links

- Frontend Web:
- Backend API:

Repositories:

- General: <https://github.com/purnomoarif/ikifurni>
- Backend API: <https://github.com/purnomoarif/ikifurni-api>
- Frontend Web: <https://github.com/purnomoarif/ikifurni-web>

UI Designs:

- Figma:

Inspirations:

- <https://ikea.co.id>
-

## Architecture & Tech Stack

### Client = Presentation Layer (UI)

- HTML
- CSS
  - Tailwind CSS
  - shadcn/ui
- JavaScript
- TypeScript
- React
- React Router
- Docker

### Server = Application Layer (Business Logic)

- JavaScript
- TypeScript
- Hono
- OpenAPI
- Zod
- Docker

### Data Access Layer (Database)

- Prisma
- PostgreSQL
- Docker

## Features

- Home page
  - Hero section
  - Products catalogue
  - Example: <https://www.ikea.co.id/in/penawaran/produk-terlaris>
- Product page
  - Image
  - SKU (stock keeping unit)
  - Name
  - Price
  - Description
  - Add to cart form: quantity input & add to cart button
- Shopping cart page
  - Product items to buy
    - Image, name, price, quantity, total (price x quantity)
    - Remove item
  - Link: continue shopping, go to products catalogue
  - Link: checkout
- Checkout page
  - Order summary
    - Product items to buy
    - Grand total of all product items to buy
- Place order / transaction is being processed

### Home Page

## Entity Relationship Diagram (ERD)

## REST API Endpoints

- Production: `
- Local: `http://localhost:3000`

| Endpoint         | HTTP     | Description               |
| ---------------- | -------- | ------------------------- |
| `/products`      | `GET`    | Get all products          |
| `/products/:id`  | `GET`    | Get product by id         |
| `/products/seed` | `POST`   | Seed all initial products |
| `/products`      | `POST`   | Add new product           |
| `/products`      | `DELETE` | Delete all products       |
| `/products/:id`  | `DELETE` | Delete product by id      |
| `/products/:id`  | `PUT`    | Update product by id      |

### Product

```json
{
  "id": "abc123",
  "slug": "meja-makan",
  "name": "meja-makan",
  "price": 3000000,
  "createdAt": "2025-10-03",
  "updatedAt": "2025-10-03"
}
```
