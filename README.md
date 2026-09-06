# WEARTH 🌍

WEARTH is a modern, full-stack e-commerce platform built with the MERN stack. It features a seamless shopping experience with product browsing, cart management, secure authentication, and integrated payment processing.

## 🚀 Features

- **User Authentication:** Secure login and registration using JWT and Google OAuth (Passport.js).
- **Product Management:** Browse products, view detailed descriptions, and manage inventory.
- **Shopping Cart:** Add, remove, and update quantities of items in the cart.
- **Secure Payments:** Integrated with Razorpay for secure and seamless checkout experiences.
- **Image Management:** Image uploading and optimization powered by ImageKit.
- **Responsive Design:** Beautiful, mobile-friendly UI crafted with Tailwind CSS v4.
- **State Management:** Robust global state handling with Redux Toolkit.

## 🛠️ Tech Stack

### Frontend
- **Framework:** React 19 (via Vite)
- **Routing:** React Router v7
- **State Management:** Redux Toolkit
- **Styling:** Tailwind CSS v4
- **HTTP Client:** Axios
- **Payment Integration:** React Razorpay

### Backend
- **Environment:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB (with Mongoose)
- **Authentication:** JSON Web Tokens (JWT), Passport.js (Google OAuth2.0)
- **Payment Gateway:** Razorpay
- **Image Processing:** ImageKit & Multer

## 📂 Project Structure

```text
WEARTH/
├── backend/          # Express backend application
│   ├── src/          # Controllers, Models, Routes, etc.
│   ├── server.js     # Entry point for the backend
│   └── package.json  # Backend dependencies
├── frontend/         # React frontend application
│   ├── src/          # Components, Pages, Features, Redux Store
│   ├── vite.config.js# Vite configuration
│   └── package.json  # Frontend dependencies
└── README.md         # Project documentation
```

## ⚙️ Installation & Setup

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [MongoDB](https://www.mongodb.com/) (Local or Atlas)
- Accounts for [Razorpay](https://razorpay.com/), [ImageKit](https://imagekit.io/), and [Google Cloud Console](https://console.cloud.google.com/) (for OAuth).

### 1. Clone the repository

```bash
git clone <your-repository-url>
cd WEARTH
```

### 2. Backend Setup

Navigate to the backend directory and install dependencies:

```bash
cd backend
npm install
```

Create a `.env` file in the `backend` directory with the following variables:

```env
PORT=3000
NODE_ENV=development
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
GOOGLE_CLIENT_ID=your_google_oauth_client_id
GOOGLE_CLIENT_SECRET=your_google_oauth_client_secret
IMAGE_KIT_PRIVATE_KEY=your_imagekit_private_key
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
FRONTEND_URL=http://localhost:5173
BACKEND_URL=http://localhost:3000
```

Start the backend development server:

```bash
npm run dev
```

### 3. Frontend Setup

Open a new terminal, navigate to the frontend directory, and install dependencies:

```bash
cd frontend
npm install
```

Create a `.env.local` file in the `frontend` directory:

```env
VITE_API_BASE_URL=http://localhost:3000/api
```

Start the frontend development server:

```bash
npm run dev
```

## 📝 Upcoming Features (TODO)
- Enhanced cart icon interactions.
- Redirect flow from order history to a dedicated order success/details page.

## 📄 License

This project is licensed under the ISC License.

