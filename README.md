# 📝 To-Do List App (Serverless)

A simple serverless To-Do list app using AWS services.

## ⚙️ Tech Stack
- 💾 **DynamoDB** – Stores task data
- 🧠 **AWS Lambda** – Handles CRUD operations
- 🌐 **API Gateway** – Connects frontend to backend
- ☁️ **Amazon S3** – Hosts the frontend (HTML, CSS, JS)

## 🚀 How It Works
- ➕ Add Task → `POST` → Lambda adds to DynamoDB
- 📄 View Tasks → `GET` → Lambda returns all tasks
- ❌ Delete Task → `DELETE` → Lambda deletes from DB

## 📂 Files
- `To-do-Lambda-Function.py` – Lambda backend (Python)
- `FrontEnd/` – Upload to S3 (update `apiUrl` in `script.js`)
- `Bucket-Policy.txt` – Set S3 access (replace bucket name)
- `API Gateway/` – Mapping templates for methods

## ✅ Steps
1. Deploy Lambda function
2. Set up API Gateway (GET, POST, DELETE, PUT)
3. Upload `FrontEnd/` to S3
4. Update `apiUrl` in `script.js`

## 🔗 Demo
👉 [Live App Link](http://todo-bucket-list.s3-website.ap-south-1.amazonaws.com/) *(Replace with your S3 website URL)*
