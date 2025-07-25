# TrendyThreads 🛍️

Welcome to **TrendyThreads**, the stylish online destination for contemporary women's fashion. At TrendyThreads, we celebrate femininity with a carefully curated collection of clothing and accessories that blend trendsetting styles with timeless sophistication.

---

## Features 🌸

- **Explore Collections:** Dive into a variety of fashion categories, each brimming with the latest styles and trends.  
- **User Authentication:** Secure login and registration system to keep your information safe.  
- **Interactive Cart:** Add items to your cart, adjust quantities, or remove them as needed with ease.  
- **Order and Payment Processing:** Smooth checkout process with integrated payment solutions.  
- **Discounts with Coupons:** Use special offers and coupons for great deals on your favorite items.  
- **Analytics Dashboard:** A feature-rich analytics section to track the performance of products and user engagement.  

---

## Project Structure 🗂️

### Backend  
Located under the `backend/` directory:  

- **Controllers:** Logic for handling API requests such as `auth.controller.js`, `product.controller.js`.  
- **Middleware:** Authentication and other reusable middleware for request processing.  
- **Models:** Mongoose schemas and models defining Users, Products, Orders, etc.  
- **Routes:** Express routes that direct API requests to the controllers.  
- **Lib:** Helper utilities and integrations like database connection (`db.js`), payment processing (`stripe.js`), and image handling (`cloudinary.js`).  

### Frontend  
Located under the `frontend/` directory:  

- **Components:** Reusable UI components such as `Navbar.jsx`, `ProductCard.jsx`.  
- **Pages:** Full page React components like `HomePage.jsx`, `AdminPage.jsx`.  
- **Stores:** State management using custom hooks and context providers (`useCartStore.js`, `useProductStore.js`).  
- **Lib:** API service wrappers and utility functions, e.g., `axios.js`.  

---

## Getting Started 🚀

### Prerequisites

- Node.js (v14 or newer)  
- npm or yarn  
- MongoDB instance (local or cloud)  

### Installation and Running

1. **Clone the repository**  
```bash
git clone https://github.com/yourgithub/trendy-threads.git
cd trendy-threads
```

2. Install dependencies
```bash
cd backend
npm install

cd ../frontend
npm install
```
3. Set up environment variables
Create .env files in both backend and frontend directories (see details below).

4. Build and start the backend server
```bash
cd backend
npm run build
npm run start
```
5. Start the frontend development server
In a new terminal window:

```bash
Copy
cd frontend
npm run dev
```
6. Open your browser
Visit http://localhost:5173 (or http://localhost:3000 if configured) to view the app.

7. Environment Variables Setup
```
PORT=5000
MONGO_URI=your_mongo_uri

UPSTASH_REDIS_URL=your_redis_url

ACCESS_TOKEN_SECRET=your_access_token_secret
REFRESH_TOKEN_SECRET=your_refresh_token_secret

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

STRIPE_SECRET_KEY=your_stripe_secret_key
CLIENT_URL=http://localhost:5173
NODE_ENV=development
```

## Usage

- Register a new account or log in with existing credentials.  
- Browse collections and add items to your cart.  
- Complete orders via integrated payment gateway.  
- Use coupons during checkout for discounts.  
- View analytics (for admin users).  

## Folder Structure

```
/trendythreads
├── backend
│ ├── src
│ │ ├── controllers # API request handlers
│ │ ├── middleware # Auth and other middleware
│ │ ├── models # Mongoose models
│ │ ├── routes # Express routes
│ │ └── server.js # Backend entry point
│ ├── package.json
│ └── package-lock.json
│
├── frontend
│ ├── public # Static assets
│ ├── src
│ │ ├── components # React UI components
│ │ ├── context # React context providers
│ │ ├── pages # Full page components
│ │ ├── App.jsx # Root component
│ │ └── main.jsx # ReactDOM render entry
│ ├── package.json
│ ├── vite.config.js
│ ├── tailwind.config.js
│ ├── postcss.config.js
│ ├── eslint.config.js
│ └── package-lock.json
│
├── .gitignore
├── LICENSE
└── README.md
```

## Contributing 👭

We welcome contributions! Please check out the `CONTRIBUTING.md` file for guidelines on how to get involved.

---

## License 📄

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

