<h1 align="center">
  📝✨ Blog Platform ✨📝
</h1>

<p align="center">
  <img src="https://media.giphy.com/media/IdyAQJVN2KPNm/giphy.gif" alt="Writing Animation" width="350"/>
</p>

<p align="center">
  A full-stack blogging application built with the MERN stack (MongoDB, Express, React, Node.js) and Redux Toolkit. Create, share, and discover amazing blog posts!
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React">
  <img src="https://img.shields.io/badge/Redux-593D88?style=for-the-badge&logo=redux&logoColor=white" alt="Redux Toolkit">
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express.js">
  <img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB">
  <img src="https://img.shields.io/badge/React_Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white" alt="React Bootstrap">
  <img src="https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white" alt="Sass">
</p>

---

## 📖 Table of Contents

- [🌟 About The Project](#-about-the-project)
- [✨ Key Features](#-key-features)
- [🛠️ Technology Stack](#️-technology-stack)
- [🚀 Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation & Setup](#installation--setup)
- [📂 Project Structure](#-project-structure)

---

## 🌟 About The Project

This is a complete blog platform where users can:

* Sign up and log in securely.
* Create new blog posts with titles, content, and cover images.
* View a paginated list of all blog posts.
* Read individual blog posts.
* Edit or delete their own posts.
* Search for posts by keyword.
* View and edit their user profile.

It features a decoupled architecture with a Node.js/Express backend API and a React frontend.

---

## ✨ Key Features

* 👤 **Authentication:** Secure user registration and login using JWT (JSON Web Tokens).
* ✍️ **Post Management (CRUD):** Full Create, Read, Update, and Delete functionality for blog posts.
* 🖼️ **Image Uploads:** Users can upload cover images for their blog posts via the backend API using `multer`.
* 👤 **User Profiles:** View user profiles and edit your own profile information.
* 🔍 **Search Functionality:** Find posts easily using keyword search.
* 📄 **Pagination:** Efficiently browse through posts with numbered pagination.
* 🔄 **State Management:** Robust state handling on the frontend using Redux Toolkit.
* 🎨 **Responsive UI:** Built with React Bootstrap for a clean and responsive user experience across devices.
* 🔐 **Protected Routes:** Middleware ensures only authenticated users can perform certain actions (like creating/editing posts).

---

## 🛠️ Technology Stack

### Backend

* **Runtime:** [Node.js](https://nodejs.org/)
* **Framework:** [Express.js](https://expressjs.com/)
* **Database:** [MongoDB](https://www.mongodb.com/) with [Mongoose](https://mongoosejs.com/) ODM
* **Authentication:** [JSON Web Tokens (JWT)](https://jwt.io/), [bcryptjs](https://www.npmjs.com/package/bcryptjs) for password hashing
* **File Uploads:** [Multer](https://github.com/expressjs/multer)
* **Middleware:** [CORS](https://www.npmjs.com/package/cors)

### Frontend

* **Library:** [React.js](https://reactjs.org/)
* **State Management:** [Redux Toolkit](https://redux-toolkit.js.org/)
* **Routing:** [React Router DOM](https://reactrouter.com/)
* **UI Framework:** [React Bootstrap](https://react-bootstrap.github.io/)
* **Styling:** [Sass (SCSS)](https://sass-lang.com/)
* **Build Tool:** [Vite](https://vitejs.dev/)
* **HTTP Client:** [Axios](https://axios-http.com/)
* **Meta Tags:** [React Helmet Async](https://github.com/staylor/react-helmet-async)

---

## 🚀 Getting Started

Follow these instructions to set up the project locally.

### Prerequisites

* **Node.js & npm:** Make sure you have Node.js (v18+) and npm installed. Download from [nodejs.org](https://nodejs.org/).
* **MongoDB:** You need a MongoDB database. You can use a local installation or a cloud service like [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) (free tier available).

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/vakrahul/BLOG_PLATFORM.git](https://github.com/vakrahul/BLOG_PLATFORM.git)
    cd BLOG_PLATFORM
    ```

2.  **Set up Backend:**
    * Navigate to the backend directory:
        ```bash
        cd backend
        ```
    * Install backend dependencies:
        ```bash
        npm install
        ```
    * Create a `.env` file in the `backend` directory with the following variables:
        ```env
        NODE_ENV=development
        PORT=5000 # Or any port you prefer
        MONGO_URI=YOUR_MONGODB_CONNECTION_STRING
        JWT_SECRET=YOUR_VERY_SECRET_JWT_KEY
        ```
        *(Replace placeholders with your actual MongoDB connection string and a strong JWT secret)*

3.  **Set up Frontend:**
    * Navigate to the frontend directory from the root:
        ```bash
        cd ../web-frontend
        # Or directly: cd BLOG_PLATFORM/web-frontend
        ```
    * Install frontend dependencies:
        ```bash
        npm install
        ```
    * Create a `.env` file in the `web-frontend` directory. Point it to your backend server's URL (likely localhost during development):
        ```env
        VITE_API_URL=http://localhost:5000 # Use the port you set for the backend
        ```

4.  **Run the Application:**
    * **Start the Backend Server:** Open a terminal in the `backend` directory and run:
        ```bash
        npm run dev
        ```
        *(This uses `nodemon` for auto-restarts during development)*
    * **Start the Frontend Development Server:** Open *another* terminal in the `web-frontend` directory and run:
        ```bash
        npm run dev
        ```
    * Open your browser and navigate to the URL provided by Vite (usually `http://localhost:5173`).

---

