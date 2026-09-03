☕ Coffee Barista RAG Agent
A virtual barista that knows the menu inside out. It recommends drinks and pastries tailored to your taste, checks for allergens, and keeps track of your order conversationally.

Built with Streamlit, Google Cloud, and Gemini using a lightweight RAG setup over a local JSON knowledge base.

## Try the Live Demo-
https://coffee-barista-187296313183.us-central1.run.app

# What It Does
Menu-Grounded Recommendations: Queries a local JSON menu to suggest drinks, roasts, and bakery items based on mood, flavor profile, or dietary preferences.

Allergen & Dietary Checks: Flags dairy, nuts, gluten, and other allergens before you place an order.

Conversational Memory: Remembers what you asked earlier in the chat so you can refine orders naturally without repeating yourself.

Fast & Lightweight: Uses a structured JSON retrieval approach without the overhead of a heavy vector database for a small shop menu.

# Tech Stack
Frontend: Streamlit

Model & Orchestration: Gemini via Google Agent Development Kit (ADK)

Cloud Infrastructure: Google Cloud Vertex AI & Google Cloud Run

Language: Python 3.10+


# Getting Started

1. Clone the repo
Bash
git clone https://github.com/your-username/coffee-barista-rag.git
cd coffee-barista-rag
2. Set up a virtual environment
Bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
3. Install dependencies
Bash
pip install -r requirements.txt
4. Configure environment variables
Create a .env file in the root directory:

Code snippet
GOOGLE_API_KEY=your_gemini_api_key_here
5. Launch the app
Bash
streamlit run app.py
The app will start locally at http://localhost:8501.

# Deployment
This app is containerized and deployed to Google Cloud Run using Google Cloud Vertex AI for model hosting. Secrets and environment variables are managed directly in cloud Run settings to keep credentials off public branches.