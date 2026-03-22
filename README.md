# 🚀 QuickBlog - Modern Blogging Platform

> A full-stack blogging platform built with React, Node.js, Express, and MongoDB. Includes admin dashboard, AI content generation, and image optimization.

---

## ✨ Features

### 📝 Blog Features
- Create and manage blog posts
- Upload and optimize images (ImageKit)
- AI-powered content generation (Gemini API)
- Category-based filtering
- Search functionality
- Responsive UI

### 💬 Comment System
- Add comments to blogs
- Admin approval system
- Delete inappropriate comments

### 🔐 Admin Panel
- JWT Authentication
- Dashboard overview
- Manage blogs (create / delete / publish)
- Manage comments (approve / delete)

---

## 🛠️ Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Axios
- React Router
- React Hot Toast

### Backend
- Node.js
- Express.js
- MongoDB + Mongoose
- JWT Authentication
- Multer (file upload)

### Services
- Google Gemini API (AI content)
- ImageKit (image storage & optimization)

---

## 📁 Project Structure

```bash
QuickBlog/
├── client/                 # Frontend React application
│   ├── public/            # Static assets
│   ├── src/
│   │   ├── components/    # Reusable components
│   │   ├── pages/         # Page components
│   │   ├── context/       # React context
│   │   ├── assets/        # Images and static files
│   │   └── main.jsx       # App entry point
│   └── package.json
│
├── server/                # Backend Node.js application
│   ├── configs/           # Database and service configs
│   ├── controllers/       # Route controllers
│   ├── middleware/        # Custom middleware
│   ├── models/            # MongoDB models
│   ├── routes/            # API routes
│   └── server.js          # Server entry point
│
└── README.md
```
## 🎯 API Endpoints

### 📝 Blog Routes

| Method | Endpoint | Description |
|--------|----------|------------|
| GET | `/api/blog/all` | Get all published blogs |
| GET | `/api/blog/:blogId` | Get single blog |
| POST | `/api/blog/add` | Add new blog (Admin) |
| POST | `/api/blog/delete` | Delete blog (Admin) |
| POST | `/api/blog/toggle-publish` | Toggle publish status (Admin) |
| POST | `/api/blog/add-comment` | Add comment to blog |
| POST | `/api/blog/comments` | Get blog comments |
| POST | `/api/blog/generate` | Generate AI content (Admin) |

---

### 🔐 Admin Routes

| Method | Endpoint | Description |
|--------|----------|------------|
| POST | `/api/admin/login` | Admin login |
| GET | `/api/admin/blogs` | Get all blogs (Admin) |
| GET | `/api/admin/comments` | Get all comments (Admin) |
| GET | `/api/admin/dashboard` | Get dashboard data (Admin) |
| POST | `/api/admin/approve-comment` | Approve comment (Admin) |
| POST | `/api/admin/delete-comment` | Delete comment (Admin) |

---

## 🎨 Features Showcase

### 🤖 AI-Powered Content Generation

QuickBlog integrates with Google Gemini AI to help content creators:

- Generate blog content from titles  
- Create engaging descriptions  
- Enhance writing productivity  

---

### 🖼️ Image Optimization

- Automatic image compression  
- WebP format conversion  
- CDN delivery via ImageKit  
- Responsive image loading  

---

### 💬 Comment System

- Real-time comment submission  
- Admin moderation panel  
- Approval workflow  
- User engagement tracking  

---

## 🚀 Deployment

### 🌐 Frontend (Vercel)

- Connect your GitHub repository to Vercel  
- Set environment variables in Vercel dashboard  
- Deploy with automatic CI/CD  

---

### ⚙️ Backend (Vercel)

- Add `vercel.json` configuration  
- Set environment variables  
- Deploy via Vercel CLI or GitHub integration  
