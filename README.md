🤖 AI Agent (Browser-Based, Agentic)

A lightweight AI Agent built using HTML, CSS, and JavaScript that runs directly in the browser using the OpenRouter API.

✔ No frameworks
✔ No build tools
✔ Controlled agent steps (no infinite loops)
✔ Beginner-friendly

🚀 Features

🧠 Step-based agentic execution

🔒 Protection against infinite API calls

🎯 One-click agent run

🌐 Uses OpenRouter (free models supported)

💻 Runs locally in browser

📁 Project Structure
ai-agent/
│
├── index.html
└── README.md

🧩 Tech Stack

HTML

CSS

JavaScript (Vanilla)

OpenRouter API

🔑 Prerequisites

Modern browser (Chrome / Edge)

Internet connection

OpenRouter API key (FREE)

🔐 Getting an OpenRouter API Key

Go to 👉 https://openrouter.ai

Sign up / log in

Open API Keys

Create a new key

Copy the key

⚠️ Never commit your API key to GitHub

🛠️ Setup Instructions
1️⃣ Clone the Repository
git clone https://github.com/your-username/ai-agent.git
cd ai-agent

2️⃣ Add Your API Key

Open index.html and replace:

const OPENROUTER_API_KEY = "PASTE_YOUR_KEY_HERE";


With:

const OPENROUTER_API_KEY = "sk-or-xxxxxxxxxxxxxxxx";

3️⃣ Run the Project (IMPORTANT)
❌ Do NOT open by double-clicking the file

This will cause CORS errors.

✅ Recommended Options
▶ Option A: VS Code (Best)

Open folder in VS Code

Install Live Server extension

Right-click index.html

Click Open with Live Server

App runs at:

http://127.0.0.1:5500

▶ Option B: Python
python -m http.server 5500


Open:

http://localhost:5500

▶ Option C: Node.js
npx serve .

🧠 How to Use

Open the app in browser

Enter your task (example):

Create a 6-month AI roadmap for SDET


Click Run Agent

Agent executes step-by-step

Output appears below

⚙️ Configuration

Inside index.html:

const MODEL = "mistralai/mistral-7b-instruct:free";
const MAX_STEPS = 3;

Variable	Description
MODEL	OpenRouter supported model
MAX_STEPS	Maximum agent reasoning steps
🛑 Safety Controls

Prevents duplicate runs

Step-limited agent loop

Button disabled during execution

No recursive or interval calls

🐛 Common Issues
❓ Blank screen

✔ Run via local server
✔ Check browser console (F12)

❓ API errors (401 / 403)

✔ Invalid or missing API key
✔ Key not pasted correctly

❓ Too many API calls

✔ Do not refresh repeatedly
✔ Keep MAX_STEPS reasonable

🔒 Security Note

This project runs entirely in the browser.

API key is visible in source

❌ Do NOT deploy publicly with key

✅ Use backend proxy for production

📦 Sharing With Others

Before sharing:

Remove your API key

Ask users to add their own key

🧠 Future Improvements

Backend proxy (Node / Python)

Planner + Executor agent

Tool calling

Memory (localStorage / DB)

UI enhancements

👨‍💻 Author

Shivam Shukla
YouTube: Technical Vartalap
