<<<<<<< HEAD
NOURISHNET
Food Donation Platform (MERN Stack)

==================================================

PROJECT OVERVIEW

NourishNet is a MERN-stack food donation platform designed to connect Donors, NGOs, Drivers, and Administrators to reduce food waste and distribute food efficiently to those in need.

The system supports four user roles:

Donor – Add and manage food donations
NGO – Request and receive food
Driver – Handle pickup and delivery
Admin – Manage system and monitor activities

Workflow:

Donor adds food items
NGO requests items
Driver delivers food
Admin monitors system

==================================================

KEY FEATURES

Role-based authentication (Admin, Donor, NGO, Driver)
Inventory and donation management
Food request system for NGOs
Real-time stock updates
Order lifecycle tracking
# NourishNet

NourishNet is a MERN-stack food donation platform designed to connect Donors, NGOs, Drivers, and Administrators to reduce food waste and distribute food efficiently to those in need.

## Project Overview

The system supports four user roles:

- Donor: Add and manage food donations
- NGO: Request and receive food
- Driver: Handle pickup and delivery
- Admin: Manage system and monitor activities

Workflow:

1. Donor adds food items
2. NGO requests items
3. Driver delivers food
4. Admin monitors system

## Key Features

- Role-based authentication (Admin, Donor, NGO, Driver)
- Inventory and donation management
- Food request system for NGOs
- Real-time stock updates
- Order lifecycle tracking
- Driver assignment and delivery workflow
- Admin dashboard with analytics
- Responsive frontend design

## Tech Stack

Frontend:

- React
- Vite
- Tailwind CSS

Backend:

- Node.js
- Express.js
- MongoDB (Mongoose)

## Setup Instructions

Step 1: Clone Repository

```
git clone https://github.com/uduladapsara/NourishNet.git
```

Step 2: Install Frontend Dependencies

```
cd NourishNet-Frontend
npm install
```

Step 3: Install Backend Dependencies

```
cd ..\NourishNet-Backend
npm install
```

Step 4: Environment Variables Setup

Frontend (.env)

```
VITE_API_URL=http://localhost:5000/api
```

Backend (.env)

```
PORT=5000
MONGO_URI=mongodb://localhost:27017/nourishnet
JWT_SECRET=your_secret
NODE_ENV=development
```

Step 5: Run Backend

```
cd NourishNet-Backend
npm run dev
```

Step 6: Run Frontend

```
cd ..\NourishNet-Frontend
npm run dev
```

Default URLs:

- Frontend: http://localhost:5173
- Backend: http://localhost:5000

## API Documentation

Base URL: `/api`

Authentication: `Authorization: Bearer <token>`

### Auth APIs

- POST `/api/auth/register` - Register a new user (Public)
- POST `/api/auth/login` - Login user (Public)
- GET `/api/auth/me` - Get current user (Protected)

### User APIs

- GET `/api/users` - Get all users (Admin) (Protected)
- PUT `/api/users/:id` - Update user (Protected)

### Inventory APIs

- GET `/api/inventory` - Get all food items
- POST `/api/inventory` - Add donation item (Donor)
- GET `/api/inventory/:id` - Get single item
- PUT `/api/inventory/:id` - Update item

### Order APIs

- POST `/api/orders` - Create order (NGO)
- GET `/api/orders` - Get orders
- GET `/api/orders/:id` - Get order details
- PUT `/api/orders/:id/status` - Update order status (Driver/Admin)

Order flow: requested -> reserved -> assigned -> picked_up -> delivered -> completed

## Deployment

Backend:

- Deploy using Render or Railway
- Set root folder as NourishNet-Backend
- Use command: npm start
- Add environment variables

Frontend:

- Deploy using Vercel or Netlify
- Set root folder as NourishNet-Frontend
- Build command: npm run build
- Output folder: dist
Year: 3rd Year
Members: TBD

==================================================

FINAL NOTE

NourishNet demonstrates a complete full-stack solution for managing food donations using modern technologies and structured workflows.

=======
NOURISHNET
Food Donation Platform (MERN Stack)

==================================================

PROJECT OVERVIEW

NourishNet is a MERN-stack food donation platform designed to connect Donors, NGOs, Drivers, and Administrators to reduce food waste and distribute food efficiently to those in need.

The system supports four user roles:

Donor – Add and manage food donations
NGO – Request and receive food
Driver – Handle pickup and delivery
Admin – Manage system and monitor activities

Workflow:

Donor adds food items
NGO requests items
Driver delivers food
Admin monitors system

==================================================

KEY FEATURES

Role-based authentication (Admin, Donor, NGO, Driver)
Inventory and donation management
Food request system for NGOs
Real-time stock updates
Order lifecycle tracking
Driver assignment and delivery workflow
Admin dashboard with analytics
Responsive frontend design

==================================================

TECH STACK

Frontend:
React
Vite
Tailwind CSS

Backend:
Node.js
Express.js
MongoDB (Mongoose)

==================================================

SETUP INSTRUCTIONS

Step 1: Clone Repository

git clone https://github.com/Theekshana-Jayalath/NourishNet-Frontend
git clone https://github.com/Theekshana-Jayalath/NourishNet-Backend

Step 2: Install Frontend Dependencies

cd frontend
npm install

Step 3: Install Backend Dependencies

cd ../backend
npm install

Step 4: Environment Variables Setup

Frontend (.env)

VITE_API_URL=http://localhost:5000/api

Backend (.env)

PORT=5000
MONGO_URI=mongodb://localhost:27017/nourishnet
JWT_SECRET=your_secret
NODE_ENV=development

Step 5: Run Backend

cd backend
npm run dev

Step 6: Run Frontend

cd frontend
npm run dev

Default URLs:

Frontend: http://localhost:5173

Backend: http://localhost:5000

==================================================

API DOCUMENTATION

Base URL:
/api

Authentication:
Authorization: Bearer <token>

AUTH APIs

POST /api/auth/register
Description: Register a new user
Authentication: Public

Request:
{
"name": "User",
"email": "user@email.com
",
"password": "123456",
"role": "donor"
}

Response:
{
"user": {
"id": "1",
"name": "User",
"role": "donor"
},
"token": "jwt_token"
}

POST /api/auth/login
Description: Login user
Authentication: Public

GET /api/auth/me
Description: Get current user
Authentication: Protected

USER APIs

GET /api/users
Description: Get all users (Admin)
Authentication: Protected

PUT /api/users/:id
Description: Update user
Authentication: Protected

INVENTORY APIs

GET /api/inventory
Description: Get all food items

POST /api/inventory
Description: Add donation item (Donor)

GET /api/inventory/:id
Description: Get single item

PUT /api/inventory/:id
Description: Update item

ORDER APIs

POST /api/orders
Description: Create order (NGO)

GET /api/orders
Description: Get orders

GET /api/orders/:id
Description: Get order details

PUT /api/orders/:id/status
Description: Update order status (Driver/Admin)

ORDER FLOW

requested → reserved → assigned → picked_up → delivered → completed

==================================================

DEPLOYMENT

Backend:
Deploy using Render or Railway
Set root folder as backend
Use command: npm start
Add environment variables

Frontend:
Deploy using Vercel or Netlify
Set root folder as frontend
Build command: npm run build
Output folder: dist

==================================================

IMPORTANT NOTES

Do NOT commit .env files
Use MongoDB Atlas for production
Use JWT for authentication
Configure CORS properly
Keep API URL correctly configured in frontend

==================================================

TESTING

Run tests using:

npm test

==================================================

SUBMISSION CHECKLIST

Source code uploaded to GitHub
README file included
API documentation added
Setup instructions provided
Environment variables documented

==================================================

TEAM DETAILS

Module: SE3040 – Application Frameworks
Assignment: Full Stack Application Development
Project: NourishNet - Zero Hunger 
Year: 3rd Year
Members: TBD

==================================================

FINAL NOTE

NourishNet demonstrates a complete full-stack solution for managing food donations using modern technologies and structured workflows.

>>>>>>> f8e21855955ec9385f13000b9475fa9510d07cee
==================================================