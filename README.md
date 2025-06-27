### AI Code Reviewer Application


This project is a web application for AI-powered code reviews, featuring a Node.js/Express backend connecting to Google Gemini, and a React frontend for user interaction.



<img width="1438" alt="Screenshot 2025-06-19 at 7 11 19 PM" src="https://github.com/user-attachments/assets/0eb7b863-3251-4c94-aeb5-f10ca8f2bc86" />




### 🌟 Features


### AI-Powered Code Review: 

Comprehensive reviews using Google Gemini.

### Detailed Feedback: 

Criticism, improvements, and refactored examples.

Markdown Formatting: Reviews displayed with syntax highlighting.

### 🚀 Technologies Used :

Backend: Node.js, Express.js, @google/generative-ai, cors, dotenv.

Frontend: React, react-simple-code-editor, prismjs, react-markdown, rehype-highlight, axios, CSS.

### 🛠️ Setup Instructions: 

Prerequisites: Node.js, npm/Yarn.

1. Clone: git clone <repository-url>

2. Backend Setup:

cd backend

npm install (or yarn install)

Create .env with GOOGLE_GEMINI_KEY=YOUR_API_KEY_HERE.

npm start (or node app.js). Runs on http://localhost:3000.

3. Frontend Setup:

cd ../frontend

npm install (or yarn install)

npm run dev (or yarn dev). Opens in browser (e.g., http://localhost:5173).

### 💡 Usage

Open frontend in browser.

Paste code into the editor.

Click "Review".

See AI review on the right.

📞 API Endpoints (Backend)
GET /: "Hello World".

POST /ai/get-review:

Body: { "code": "..." }

Response: AI review string.

🤝 Contributing
Welcome issues and pull requests.

📄 License
MIT License.
