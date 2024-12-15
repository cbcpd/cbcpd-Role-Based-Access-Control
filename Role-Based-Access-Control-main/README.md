🌟 Job Seeking Application
Project Overview
Welcome to the Job Seeking Application! This platform enables job seekers to apply for jobs and employers to post job listings. 🚀

The app implements secure authentication mechanisms using JWT (JSON Web Tokens), allowing users to log in, register, and securely access resources based on their roles.

Job Seekers can:
📝 Register and log in to their account.
💼 Apply for jobs posted by employers.
✏️ Modify or delete their applications.

Employers can:
📝 Register and log in to their account.
📋 Post jobs.
🛠️ Modify or delete job postings.
👀 View and manage applications from job seekers.

The system ensures role-based access control (RBAC), where job seekers and employers have different access levels, ensuring that only authorized users can perform specific actions.

Key Features 🔑
Authentication & Authorization
🔐 Users (job seekers and employers) are authenticated using JWT.
👩‍💻 Only job seekers can apply for jobs and manage their applications.
👨‍💼 Only employers can post, modify, and delete job listings.
Role-Based Access Control (RBAC) 💼
Admin: Full access to manage both employers and job seekers.
Employer: Can manage job postings and view applications.
Job Seeker: Can apply for jobs and manage their applications.
Secure Password Storage 🔑
Passwords are securely hashed using bcrypt.
Database Integration (MongoDB) 🗄️
All data (user profiles, job listings, applications) is securely stored in MongoDB.


Installation and Setup ⚙️
1. Clone the Repository 🔁
First, clone this repository to your local machine using the following command:
git clone <repository_url>
cd <repository_name>
Replace <repository_url> with your actual repository URL, and <repository_name> with the name of your project folder.

2. Backend Setup (Node.js & Express) 🖥️
After cloning the repository, follow these steps to set up the backend:

Navigate to the Backend Folder:
cd backend

Install Dependencies:
Run the following command to install the necessary packages for the backend:
npm install

Setup Environment Variables 🔒:
Create a .env file in the backend directory and include the following variables:
env
MONGO_URI=<your_mongodb_connection_string>

JWT_SECRET=<your_jwt_secret_key>

PORT=4000

Replace <your_mongodb_connection_string> with your actual MongoDB URI (you can use MongoDB Atlas for a cloud database).

Replace <your_jwt_secret_key> with a secure JWT secret key (you can generate a random string).

Start the Backend Server 🚀:
To run the backend server, use the following command:
nodemon server.js


3. Frontend Setup (React) 🌐
After setting up the backend, follow these steps to set up the frontend:

Navigate to the Frontend Folder:
cd frontend

Install Dependencies:
Run the following command to install the required dependencies for the frontend
npm install

Start the Frontend Application 💻:
To start the frontend application, use:
npm run dev

4. Test the Application ✅
Now that both the frontend and backend are running:

Open your browser and go to http://localhost:5173 to test the frontend.

Ensure that the backend is running and accessible at http://localhost:4000.

