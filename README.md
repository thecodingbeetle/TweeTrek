🐦 TweeTrek

A scalable backend for a Twitter-like social media application, built with Node.js, Express, MongoDB, and AWS S3.

This backend powers core social features such as tweets, likes, comments, authentication, and image uploads — all designed with a clean architecture using repositories, services, and controllers.

🚀 Features

✅ User Authentication – Signup/Login with JWT

✅ Tweets – Create, read, and paginate tweets (max 250 chars per tweet)

✅ Image Uploads – Store tweet images on AWS S3

✅ Likes – Like/Unlike tweets & comments

✅ Nested Comments – Comment on a tweet or another comment

✅ Hashtag Support – Add hashtags inside tweets

✅ REST API – Modular, maintainable architecture

✅ Scalable & Secure – Clean, production-ready codebase

⚙️ Tech Stack

Backend Framework: Node.js + Express

Database: MongoDB + Mongoose

Authentication: JWT (JSON Web Tokens)

File Storage: AWS S3 (via Multer-S3)

Other Tools: dotenv, bcrypt, error handling utilities

🔑 API Endpoints
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

🛠️ Installation & Setup
Prerequisites

Node.js
 & npm installed

MongoDB
 (local or remote instance)

AWS account (for S3 bucket setup)

Steps

1️⃣ Clone the repo

git clone https://github.com/thecodingbeetle/TweeTrek.git
cd TweeTrek


2️⃣ Install dependencies

npm install


3️⃣ Configure environment variables → Create a .env file:

MONGODB_URI=
JWT_SECRET=
AWS_REGION=
AWS_SECRET_ACCESS_KEY=
ACCESS_KEY_ID=
BUCKET_NAME=


4️⃣ Run the server

npm start


👉 Server will run at: http://localhost:3000
