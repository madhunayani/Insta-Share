<div align="center">

# 📸 Insta Share

### A Modern Social Media Platform Built with React

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen?style=for-the-badge&logo=vercel)](https://insta-share-madhunayani.vercel.app)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/madhunayani/Insta-Share)
[![React](https://img.shields.io/badge/React-17.0.1-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://reactjs.org/)
[![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)](LICENSE)

*Experience seamless photo sharing, user interactions, and real-time updates in a stunning Instagram-inspired interface*

[View Demo](#-demo) • [Features](#-features) • [Installation](#-installation) • [Tech Stack](#-tech-stack) • [Contact](#-contact)

</div>

---

## 🌟 Overview

**Insta Share** is a feature-rich social media web application that replicates core Instagram functionalities. Built with React.js and modern web technologies, it offers a smooth, responsive user experience with authentication, real-time post interactions, user profiles, and dynamic content rendering.

Whether you're exploring stories, liking posts, or searching for users, Insta Share delivers a polished and intuitive social networking experience.

---

## ✨ Features

### 🔐 Authentication & Security
- **Secure Login System** with JWT token-based authentication
- Protected routes ensuring authorized access only
- Persistent sessions using `js-cookie`
- Automatic redirect for unauthenticated users

### 📱 Core Functionality
- **Posts Feed** - Browse through a dynamic feed of user posts
- **Stories Carousel** - Swipe through user stories with React Slick
- **Like/Unlike** - Interactive post engagement with real-time updates
- **Comments Section** - View user comments on each post
- **User Profiles** - Dedicated profile pages with user stats and posts
- **My Profile** - Personal profile management
- **Search** - Find users and posts with instant search functionality
- **Responsive Design** - Seamless experience across all devices

### 🎨 UI/UX Highlights
- Clean, Instagram-inspired interface
- Smooth loading states with React Loader Spinner
- Icon integration with React Icons
- Optimized image rendering and lazy loading
- Dark mode compatible (context-based theming)

---

## 🎬 Demo

> **Note:** Replace with your actual Vercel deployment link after deployment

🔗 **Live Application:** [https://insta-share-madhunayani.vercel.app](https://insta-share-madhunayani.vercel.app)

### 📸 Screenshots

<div align="center">

| Login Page | Home Feed |
|:----------:|:---------:|
| ![Login](https://via.placeholder.com/400x250?text=Login+Page) | ![Home](https://via.placeholder.com/400x250?text=Home+Feed) |

| User Profile | Search |
|:------------:|:------:|
| ![Profile](https://via.placeholder.com/400x250?text=User+Profile) | ![Search](https://via.placeholder.com/400x250?text=Search) |

</div>

> **Tip:** Add actual screenshots by uploading images to your repo or using services like [Cloudinary](https://cloudinary.com)

---

## 🛠️ Tech Stack

### Frontend
![React](https://img.shields.io/badge/React-17.0.1-61DAFB?style=flat-square&logo=react&logoColor=white)
![React Router](https://img.shields.io/badge/React_Router-5.3.0-CA4245?style=flat-square&logo=react-router&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)

### Libraries & Tools
- **React Slick** - Carousel for stories
- **React Loader Spinner** - Loading states
- **React Icons** - Icon components
- **js-cookie** - Cookie management for JWT tokens
- **React Testing Library** - Unit testing
- **ESLint & Prettier** - Code quality and formatting

### DevOps & Deployment
![Vercel](https://img.shields.io/badge/Vercel-Deployment-000000?style=flat-square&logo=vercel&logoColor=white)
![Git](https://img.shields.io/badge/Git-Version_Control-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=flat-square&logo=github&logoColor=white)

---

## 🚀 Installation

### Prerequisites

Ensure you have the following installed:
- **Node.js** (v14.x or higher)
- **npm** (v6.x or higher)
- **Git**

### Clone Repository

git clone https://github.com/madhunayani/Insta-Share.git

### Navigate to project directory
cd Insta-Share


### Install Dependencies

npm install


### Environment Setup

No environment variables needed — the app uses an external API endpoint.

### Run Locally

Start development server
npm start


The application will open at `http://localhost:3000` 🚀

### Build for Production

Create optimized production build
npm run build


### Run Tests

Run test suite
npm test


---

## 📁 Project Structure

Insta-Share/
├── public/
│ ├── index.html
│ └── img/
│ └── (logos and icons)
├── src/
│ ├── components/
│ │ ├── Header/
│ │ ├── Home/
│ │ ├── LoginPage/
│ │ ├── Posts/
│ │ ├── Profile/
│ │ ├── SearchPosts/
│ │ ├── Stories/
│ │ └── (other components)
│ ├── SearchContext/
│ │ └── index.js
│ ├── App.js
│ ├── App.css
│ └── index.js
├── package.json
├── vercel.json
└── README.md


---

## 🔌 API Integration

This project uses an external REST API for authentication and data:

**Base URL:** `https://apis.ccbp.in`

### Endpoints Used

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/login` | User authentication |
| GET | `/insta-share/posts` | Fetch all posts |
| POST | `/insta-share/posts/:id/like` | Like/Unlike a post |
| GET | `/insta-share/profile/:username` | Fetch user profile |
| GET | `/insta-share/posts?search=query` | Search posts |

### Authentication

- JWT token received upon successful login
- Token stored in cookies for persistent sessions
- Token sent in `Authorization` header for protected routes

headers: {
Authorization: Bearer ${jwt_token}
}


---

## 🌐 Deployment

### Deploy to Vercel

1. **Push to GitHub**
git add .
git commit -m "Ready for deployment"
git push origin main


2. **Import to Vercel**
- Go to [vercel.com/new](https://vercel.com/new)
- Select your repository
- Framework: **Create React App**
- Click **Deploy**

3. **Automatic Deployments**
- Every push to `main` triggers automatic redeployment

### Manual Deployment

Install Vercel CLI
npm install -g vercel

Deploy
vercel --prod


---

## 🎯 Usage

### Login Credentials (Demo)
Username: rahul
Password: rahul@2021


### Key Features Walkthrough

1. **Login** → Enter credentials to access the platform
2. **Home Feed** → Scroll through posts, like/unlike, view comments
3. **Stories** → Swipe through user stories at the top
4. **Search** → Use the search bar to find users and posts
5. **Profile** → Click on usernames to view their profiles
6. **My Profile** → Access your personal profile from the header

---

## 🤝 Contributing

Contributions are what make the open-source community amazing! Any contributions you make are **greatly appreciated**.

1. **Fork** the Project
2. **Create** your Feature Branch
git checkout -b feature/AmazingFeature
3. **Commit** your Changes
git commit -m "Add some AmazingFeature"
4. **Push** to the Branch
git push origin feature/AmazingFeature
5. **Open** a Pull Request

---

## 🐛 Known Issues

- Stories carousel may lag on slower devices (optimization in progress)
- Search functionality currently searches posts only (users coming soon)

---

## 📝 Roadmap

- [ ] Add dark mode toggle
- [ ] Implement post creation feature
- [ ] Real-time notifications
- [ ] Direct messaging system
- [ ] Video post support
- [ ] User settings page
- [ ] Follow/Unfollow functionality

---

## 📜 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

## 👨‍💻 Author

**Madhu Nayani**

[![GitHub](https://img.shields.io/badge/GitHub-madhunayani-181717?style=flat-square&logo=github)](https://github.com/madhunayani)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/madhunayani)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-FF5722?style=flat-square&logo=google-chrome&logoColor=white)](https://madhunayani.vercel.app)

*Full Stack Developer (MERN) | React.js Enthusiast | Problem Solver*

---

## 🙏 Acknowledgments

- [React Documentation](https://reactjs.org/)
- [React Router](https://reactrouter.com/)
- [Shields.io](https://shields.io/) for badges
- [Vercel](https://vercel.com/) for hosting
- API provided by CCBP

---

<div align="center">

**⭐ If you found this project helpful, please give it a star!**

Made with ❤️ and ⚛️ React

</div>
