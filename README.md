# 🐦 TWEE TREK  

A scalable backend for a Twitter-like social media application, built with **Node.js, Express, MongoDB, and AWS S3**.  

This backend handles core social features such as tweets, likes, comments, authentication, and image uploads, following a clean architecture with repositories, services, and controllers.  

---

## 🚀 Features  

- ✅ User Authentication (Signup/Login with JWT)  
- ✅ Create, read, and paginate tweets (max 250 chars per tweet)  
- ✅ Image uploads for tweets (via AWS S3)  
- ✅ Like/Unlike tweets & comments  
- ✅ Nested comments (comment on a tweet or another comment)  
- ✅ Hashtag support for tweets  
- ✅ REST API with modular architecture  
- ✅ Secure and scalable codebase  

---

## 📂 Project Structure  

/src
<img width="571" height="237" alt="image" src="https://github.com/user-attachments/assets/08842caa-aab9-4886-a781-737e8db4ba0c" />


markdown
Copy code

---

## ⚙️ Tech Stack  

- **Backend Framework:** Node.js + Express  
- **Database:** MongoDB + Mongoose  
- **Authentication:** JWT (JSON Web Tokens)  
- **File Storage:** AWS S3 (via Multer-S3)  
- **Other Tools:** dotenv, bcrypt, error handling utilities  

---

## 🔑 API Features  

### Authentication  
- **POST** `/api/v1/signup` → Register a new user  
- **POST** `/api/v1/login` → Login and receive JWT  

### Tweets  
- **POST** `/api/v1/tweets` → Create a tweet (max 250 chars, optional image)  
- **GET** `/api/v1/tweets?page=1&limit=10` → Fetch paginated tweets  

### Likes  
- **POST** `/api/v1/likes/toggle` → Like/Unlike a tweet or comment  

### Comments  
- **POST** `/api/v1/comments` → Add a comment to a tweet or another comment  

---

## 🛠️ Installation  

### Prerequisites  
- Node.js & npm installed  
- MongoDB (local or remote)  
- AWS account (for S3 bucket setup)  

### Steps  

1️⃣ **Clone the repo**  
```bash
git clone https://github.com/thecodingbeetle/TweeTrek.git
cd TweeTrek
2️⃣ Install dependencies

bash
Copy code
npm install
3️⃣ Configure environment variables → Create a .env file:

env
Copy code
MONGODB_URI=
JWT_SECRET=
AWS_REGION=
AWS_SECRET_ACCESS_KEY=
ACCESS_KEY_ID=
BUCKET_NAME=
4️⃣ Run the server


Copy code
npm start
Server runs at: http://localhost:3000
