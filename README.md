TweeTrek

A scalable backend for a Twitter-like social media application, built with Node.js, Express, MongoDB, and AWS S3.

This backend handles core social features such as tweets, likes, comments, authentication, and image uploads, following a clean architecture with repositories, services, and controllers.

🚀 Features

✅ User Authentication (Signup/Login with JWT)
✅ Create, read, and paginate tweets (max 250 chars per tweet)
✅ Image uploads for tweets (via AWS S3)
✅ Like/unlike tweets & comments
✅ Nested comments (comment on a tweet or another comment)
✅ Hashtag support for tweets
✅ REST API with modular architecture
✅ Secure and scalable codebase

📂 Project Structure
<img width="155" height="242" alt="image" src="https://github.com/user-attachments/assets/94af06ff-d7a0-4b19-a715-1e8114449ae6" />


⚙️ Tech Stack

Backend Framework: Node.js + Express

Database: MongoDB + Mongoose

Authentication: JWT (JSON Web Tokens)

File Storage: AWS S3 (via Multer-S3)

Other Tools: dotenv, bcrypt, error handling utilities

🔑 API Features
Authentication

POST /api/v1/signup → Register a new user

POST /api/v1/login → Login and receive JWT

Tweets

POST /api/v1/tweets → Create a tweet (max 250 chars, optional image)

GET /api/v1/tweets?page=1&limit=10 → Fetch paginated tweets

Likes

POST /api/v1/likes/toggle → Like/Unlike a tweet or comment

Comments

POST /api/v1/comments → Add a comment to a tweet or another comment

🛠️ Installation
Prerequisites

Node.js & npm installed

MongoDB (local or remote)

AWS account (for S3 bucket setup)

Steps

1️⃣ Clone the repo

git clone https://github.com/<your-username>/twitter-backend.git
cd twitter-backend


2️⃣ Install dependencies

npm install


3️⃣ Configure environment variables → Create a .env file:

MONGODB_URI=<your-mongodb-uri>
JWT_SECRET=<your-jwt-secret>
AWS_REGION=<your-aws-region>
AWS_SECRET_ACCESS_KEY=<your-aws-secret>
ACCESS_KEY_ID=<your-aws-id>
BUCKET_NAME=<your-bucket-name>


4️⃣ Run the server

npm start


Server runs at: http://localhost:3000
