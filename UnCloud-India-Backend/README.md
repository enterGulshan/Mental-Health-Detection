# UnCloud India - Backend API

Backend API server for the UnCloud India mental wellness application.

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- MongoDB Atlas account
- Environment variables configured

### Installation
```bash
npm install
```

### Environment Setup
1. Copy `.env.example` to `.env`
2. Fill in your MongoDB URI and JWT secret
3. Update FRONTEND_URL for CORS

### Development
```bash
npm run dev
```

### Production
```bash
npm start
```

## 📡 API Endpoints

### Health Check
- `GET /` - Server status
- `GET /api/health` - Detailed health check

### Authentication
- `POST /api/auth/signup` - User registration
- `POST /api/auth/signin` - User login
- `GET /api/auth/me` - Get current user
- `PUT /api/auth/profile` - Update user profile
- `POST /api/auth/signout` - User logout

## 🔧 Environment Variables

Required environment variables for production:

```env
NODE_ENV=production
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/database
JWT_SECRET=your_jwt_secret_key
JWT_EXPIRES_IN=7d
FRONTEND_URL=https://your-frontend-domain.com
```

## 🚀 Deployment

This API is configured for deployment on Vercel:

1. Connect your GitHub repository to Vercel
2. Add environment variables in Vercel dashboard
3. Deploy automatically on push to main branch

## 🔒 Security Features

- CORS protection
- Rate limiting
- JWT authentication
- Password hashing with bcrypt
- Input validation
- Helmet security headers

## 📊 Database Models

- **User**: User accounts and preferences
- **Mood**: Mood tracking data
- **ChatSession**: AI therapy chat sessions

## 🤝 Contributing

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

## 📄 License

MIT License - see LICENSE file for details