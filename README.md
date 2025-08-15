MineBot

MineBot is an intelligent chatbot designed to assist with queries related to mining laws, regulations, and guidelines in India.
It uses advanced Natural Language Processing (NLP) techniques and integrated external knowledge sources to provide accurate and contextual responses.

Key Features

Mining Law Knowledge – Information on acts, regulations, circulars, and notifications relevant to India’s mining sector.

Natural Language Queries – Interact in plain language without needing predefined commands.

External Knowledge Support – Integrates sources like Wikipedia and search APIs to enhance responses.

Reasoning Framework – Uses a reasoning-based approach to choose the best possible answer path.

Easy Deployment – Runs locally or inside Docker for flexible deployment options.

Getting Started
1. Clone the Repository
git clone https://github.com/your-username/MineBot.git
cd MineBot

2. Create and Activate a Virtual Environment (optional but recommended)
python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

3. Install Dependencies
pip install -r requirements.txt

4. Configure Environment Variables

Create a .env file in the project root and add your API keys:

HUGGINGFACEHUB_API_TOKEN=your_token_here
OPENAI_API_KEY=your_token_here
SERPAPI_API_KEY=your_token_here

5. Run the Application
streamlit run app.py


Open your browser and go to:

http://localhost:8501

Troubleshooting
SWIG Error (faiss-cpu installation)

If you encounter a SWIG-related error during dependency installation:

Linux/macOS:

sudo apt-get update
sudo apt-get install swig


Windows:
Download the SWIG executable from the official website and add it to your system PATH.

Deployment

You can also run MineBot in a Docker container:

docker build -t minebot .
docker run -p 8501:8501 minebot

License

This project is intended for non-commercial and educational purposes.
You are free to use and modify it with proper attribution.
For commercial use, please obtain explicit permission.