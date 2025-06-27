AI Code Reviewer Application

This project provides a simple web application that allows users to submit code snippets for review by an AI model. The backend, built with Node.js and Express, serves as an API gateway to the Google Gemini AI model, which acts as a senior code reviewer. The frontend, a React application, provides a user interface for code input and displaying AI-generated reviews.

🌟 Features
Code Input Editor: An intuitive editor for writing or pasting code snippets.

AI-Powered Code Review: Leverage Google Gemini to get comprehensive code reviews.

Detailed Feedback: The AI provides constructive feedback, identifies issues, suggests improvements, and offers refactored code examples.

Markdown Formatting: Reviews are presented in a readable Markdown format with syntax highlighting.

🚀 Technologies Used
Backend
Node.js: JavaScript runtime environment.

Express.js: Web framework for Node.js.

@google/generative-ai: Google's official Node.js library for interacting with the Gemini API.

cors: Middleware to enable Cross-Origin Resource Sharing.

dotenv: For loading environment variables.

Frontend
React: A JavaScript library for building user interfaces.

react-simple-code-editor: A simple, flexible code editor for React.

prismjs: A lightweight, extensible syntax highlighter.

react-markdown: A React component to render Markdown.

rehype-highlight: A rehype plugin to highlight code blocks in Markdown.

axios: Promise-based HTTP client for the browser and Node.js.

CSS: For styling.

🛠️ Setup Instructions
Follow these steps to get the project up and running on your local machine.

Prerequisites
Node.js (LTS version recommended)

npm or Yarn

1. Clone the Repository
git clone <repository-url> # Replace <repository-url> with your repository URL
cd <project-folder>

2. Backend Setup
Navigate to the backend directory:

cd backend

Install dependencies:

npm install
# or
yarn install

Create a .env file in the backend directory and add your Google Gemini API key:

GOOGLE_GEMINI_KEY=YOUR_API_KEY_HERE

Note: You can obtain a Google Gemini API key from the Google AI Studio.

Start the backend server:

npm start
# or
node app.js

The backend server will run on http://localhost:3000.

3. Frontend Setup
Open a new terminal, navigate back to the root project directory, and then go into the frontend directory:

cd ../frontend

Install dependencies:

npm install
# or
yarn install

Start the frontend development server:

npm run dev
# or
yarn dev

The frontend application will typically open in your browser at http://localhost:5173 (or another port if 5173 is in use).

💡 Usage
Open the frontend application in your browser (e.g., http://localhost:5173).

Paste or type your JavaScript code into the code editor on the left.

Click the "Review" button.

The AI-generated code review will appear on the right side of the screen, formatted with Markdown and syntax highlighting.

📞 API Endpoints (Backend)
GET /: Returns "Hello World" to confirm the server is running.

POST /ai/get-review:

Body: JSON object with a code property:

{
  "code": "function sum(a, b) { return a + b; }"
}

Response: The AI-generated code review as a string.

🤝 Contributing
Contributions are welcome! Please feel free to submit issues or pull requests.

📄 License
This project is open-sourced under the MIT License.
