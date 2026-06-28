🚀 Sandip’s LinkForge AI
✨ AI-Powered LinkedIn Post Generator | Built with Python, Streamlit, Flask, LangChain & Groq

Create polished, engaging, and professional LinkedIn posts in seconds using next-level AI.
Transform your ideas into scroll-stopping content — powered by Llama-3.3 model on Groq.

🌟 Features
🔮 AI-Generated LinkedIn Posts

Generate high-quality content based on:
Prompt/topic
Word count
Tone (professional, friendly, casual, enthusiastic, authoritative)
Template type (informative, casual, inspirational)
🎭 Tone & Style Customization
Fine-tuned control over output style for better personalization.

🔣 Smart Hashtags Generator
Automatically includes relevant hashtags to increase reach.
😀 Emoji Enhancer
Makes your posts more engaging and expressive.
🔄 Multiple Variations
Generate 1–3 variations of the same post for A/B testing.
📊 Content Analysis
Each post includes:
Word count
Character count
Sentence count

🖥️ Dual Interface
Use either:
Streamlit Web UI (Frontend)
Flask REST API (Backend)

🛠️ Tech Stack
Frontend (UI)
🌈 Streamlit
Backend
🔥 Flask REST API
AI & LLM Frameworks
🤖 LangChain
⚡ Groq Llama-3.3 70B (via ChatGroq)
🧠 Prompt Engineering

Utilities
Python 3.10+
Regex for analytics
Environment variables for secrets

📂 Project Structure
LinkForge-AI/
│
├── app.py                     # Streamlit UI & Flask API entrypoint
├── linkedin_generator.py       # Core AI generation logic
├── requirements.txt            # Python dependencies
├── .env                        # Environment variables (ignored in GitHub)
└── .streamlit/
    └── secrets.toml            # Streamlit secrets storage

🚀 Getting Started
1️⃣ Clone the Repository
git clone https://github.com/sandippatil04/Sandip-s-LinkForge.git
cd Sandip-s-LinkForge

2️⃣ Install Dependencies
pip install -r requirements.txt

3️⃣ Add Environment Variables
Create .env:
GROQ_API_KEY=your_groq_api_key_here
GROQ_MODEL=llama-3.3-70b-versatile

Create .streamlit/secrets.toml:
GROQ_API_KEY = "your_groq_api_key_here"

🖥️ Run the Streamlit App
streamlit run app.py


App will run at:
👉 http://localhost:8501

🧩 Run the Flask API
flask run


API endpoint:
👉 POST http://localhost:5000/generate

Example Request:
curl -X POST http://localhost:5000/generate \
  -H "Content-Type: application/json" \
  -d '{
    "prompt": "AI trends in 2025",
    "words": 150,
    "tone": "professional",
    "template": "informative",
    "add_hashtags": true,
    "add_emojis": true,
    "variations": 2
  }'

🎨 Screenshots

![Screenshot 1](/.github/assets/image1.png)
![Screenshot 2](/.github/assets/image2.png)
![Screenshot 2](/.github/assets/image3.png)


🔧 How It Works (Architecture)

User enters prompt in Streamlit UI

App sends request to LinkedInPostGenerator

LangChain formats prompt using PromptTemplate

Groq model generates high-quality content

Optional:

Hashtags added

Emojis added

Content analysis (regex)

Final result displayed or returned via API

🧠 Why I Built This

LinkedIn engagement is becoming crucial for:
Job seekers
Creators
Entrepreneurs
Students & professionals
But writing high-quality posts daily is hard.
So I built LinkForge AI to automate content creation with production-level AI.

🚀 Future Enhancements
Twitter/X post generator mode
Instagram caption generator
Save posts to database (SQLite/MongoDB)
User login system
Keyword extraction
SEO analyzer
Scheduled posts
Export to PDF feature

Created with ❤️ by Sandip Patil
