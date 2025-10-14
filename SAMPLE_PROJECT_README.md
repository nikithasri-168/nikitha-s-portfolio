# 🛒 ShopZone - E-Commerce Platform

A full-stack MERN e-commerce application with secure payment processing, real-time inventory management, and an admin dashboard.

![ShopZone Demo](https://via.placeholder.com/800x400?text=Add+Your+Screenshot+Here)

## 🌟 Features

### User Features
- 🔐 Secure JWT authentication & authorization
- 🛍️ Browse products with search and filters
- 🛒 Shopping cart with real-time updates
- 💳 Stripe payment integration
- 📦 Order tracking and history
- ⭐ Product reviews and ratings
- 📱 Fully responsive design

### Admin Features
- 📊 Sales analytics dashboard
- 📦 Inventory management
- 👥 User management
- 🎯 Order fulfillment tracking
- 📈 Revenue reports

## 🚀 Tech Stack

**Frontend:**
- React.js - UI framework
- Redux - State management
- React Router - Navigation
- Axios - API calls
- Tailwind CSS - Styling

**Backend:**
- Node.js - Runtime environment
- Express.js - Web framework
- MongoDB - Database
- Mongoose - ODM
- JWT - Authentication
- Bcrypt - Password hashing

**Payment:**
- Stripe API - Payment processing

**DevOps:**
- Docker - Containerization
- Heroku - Deployment
- AWS S3 - Image storage

## 📋 Prerequisites

Before running this project, make sure you have:
- Node.js (v14 or higher)
- MongoDB (local or Atlas)
- Stripe account (for payment processing)
- npm or yarn package manager

## ⚙️ Installation

1. **Clone the repository**
```bash
git clone https://github.com/nikithasri-168/shopzone-ecommerce.git
cd shopzone-ecommerce
```

2. **Install dependencies**

Backend:
```bash
cd backend
npm install
```

Frontend:
```bash
cd frontend
npm install
```

3. **Environment Variables**

Create a `.env` file in the backend folder:
```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
STRIPE_SECRET_KEY=your_stripe_secret_key
STRIPE_PUBLISHABLE_KEY=your_stripe_publishable_key
AWS_ACCESS_KEY=your_aws_access_key
AWS_SECRET_KEY=your_aws_secret_key
AWS_BUCKET_NAME=your_bucket_name
```

Create a `.env` file in the frontend folder:
```env
REACT_APP_API_URL=http://localhost:5000
REACT_APP_STRIPE_KEY=your_stripe_publishable_key
```

4. **Run the application**

Backend:
```bash
cd backend
npm run dev
```

Frontend (in a new terminal):
```bash
cd frontend
npm start
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend: http://localhost:5000

## 📁 Project Structure

```
shopzone-ecommerce/
├── backend/
│   ├── config/         # Configuration files
│   ├── controllers/    # Route controllers
│   ├── middleware/     # Custom middleware
│   ├── models/         # Database models
│   ├── routes/         # API routes
│   ├── utils/          # Utility functions
│   └── server.js       # Entry point
├── frontend/
│   ├── public/         # Static files
│   ├── src/
│   │   ├── components/ # React components
│   │   ├── pages/      # Page components
│   │   ├── redux/      # Redux store & slices
│   │   ├── utils/      # Helper functions
│   │   └── App.js      # Main component
│   └── package.json
└── README.md
```

## 🔑 Key Features Implementation

### Authentication
- JWT-based authentication
- Secure password hashing with bcrypt
- Protected routes on both frontend and backend
- Automatic token refresh

### Payment Processing
- Stripe integration for secure payments
- Support for multiple payment methods
- Order confirmation emails
- Failed payment handling

### State Management
- Redux for global state
- Redux Thunk for async actions
- Persistent cart using localStorage
- Real-time inventory updates

## 📊 API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Products
- `GET /api/products` - Get all products
- `GET /api/products/:id` - Get single product
- `POST /api/products` - Create product (Admin)
- `PUT /api/products/:id` - Update product (Admin)
- `DELETE /api/products/:id` - Delete product (Admin)

### Orders
- `POST /api/orders` - Create new order
- `GET /api/orders/:id` - Get order details
- `GET /api/orders/user/:userId` - Get user orders
- `PUT /api/orders/:id/pay` - Update order to paid

### Cart
- `GET /api/cart` - Get user cart
- `POST /api/cart` - Add item to cart
- `PUT /api/cart/:id` - Update cart item
- `DELETE /api/cart/:id` - Remove from cart

## 🧪 Testing

Run tests:
```bash
# Backend tests
cd backend
npm test

# Frontend tests
cd frontend
npm test
```

## 📈 Performance Optimizations

- Redis caching for frequently accessed data
- Image optimization and lazy loading
- Code splitting with React.lazy
- MongoDB indexing for faster queries
- Debounced search functionality

## 🔒 Security Features

- Helmet.js for security headers
- CORS configuration
- Rate limiting on API endpoints
- Input validation and sanitization
- XSS protection
- SQL injection prevention

## 🚀 Deployment

### Backend (Heroku)
```bash
heroku create shopzone-api
git push heroku main
heroku config:set NODE_ENV=production
```

### Frontend (Netlify)
```bash
npm run build
netlify deploy --prod --dir=build
```

## 📝 Environment Variables Checklist

- [ ] MongoDB connection string
- [ ] JWT secret key
- [ ] Stripe API keys
- [ ] AWS credentials
- [ ] Email service credentials (if using)
- [ ] Frontend API URL

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👨‍💻 Author

**Nikitha Sri Garapati**
- Portfolio: [nikithasri-168.github.io](https://nikithasri-168.github.io)
- LinkedIn: [linkedin.com/in/nikithasri-garapati](https://linkedin.com/in/nikithasri-garapati)
- GitHub: [@nikithasri-168](https://github.com/nikithasri-168)
- Email: nikithasri.garapati@gmail.com

## 🙏 Acknowledgments

- Stripe for payment processing
- MongoDB Atlas for database hosting
- All the open-source libraries used in this project

## 📸 Screenshots

### Home Page
![Home](https://via.placeholder.com/800x400?text=Add+Homepage+Screenshot)

### Product Page
![Product](https://via.placeholder.com/800x400?text=Add+Product+Page+Screenshot)

### Admin Dashboard
![Dashboard](https://via.placeholder.com/800x400?text=Add+Dashboard+Screenshot)

---

⭐ Star this repository if you found it helpful!

**Built with ❤️ for E-Commerce Excellence**
