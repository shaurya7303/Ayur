Ayur – AI Medical Chatbot

Ayur is an AI-powered medical chatbot that provides general health guidance, symptom-based suggestions, and Ayurvedic wellness tips. It is built using LLMs, LangChain, Pinecone, Flask, and AWS, and designed for fast, safe and contextual responses.

✨ Features

Medical & wellness Q&A

Symptom-based guidance

Context-aware chat using LangChain

Fast semantic search with Pinecone

Flask REST API

Production-ready AWS deployment

Safety filters + medical disclaimers

🛠️ Tech Stack

LLMs (Perplexity)

LangChain for orchestration

Pinecone for vector storage

Flask for backend API

AWS (EC2 )

📁 Project Structure
Ayur/
│── app.py
│── requirements.txt
│── data/
│── model/
│── src/
│── templates/
│── setup.py
│── Dockerfile
│── README.md

⚙️ Installation
git clone https://github.com/shaurya7303/Ayur.git
cd ayur
pip install -r requirements.txt


Create a .env file:

PPLX_API_KEY=your_key
PINECONE_API_KEY=your_key
PINECONE_ENV=your_env
AWS_REGION=your_region

▶️ Run the App
python app.py


API Endpoint:

POST /chat


Example payload:

{
  "query": "I have stomach pain, what should I do?"
}

🩺 Sample Response
Mild stomach pain may be caused by gas, acidity, or digestive issues. 
Try drinking warm water and resting. 
If pain increases, persists for more than 24 hours, or is severe, please consult a doctor. 
(This is general guidance, not a medical diagnosis.)

☁️ Deployment

EC2: Flask + Gunicorn + Nginx

Serverless: AWS Lambda + API Gateway

Storage: Pinecone for vectors, S3 for assets

🔐 Safety

No personal data stored

Input validation

Built-in medical disclaimers

⚠️ Disclaimer

Ayur provides general medical guidance only.
It is not a substitute for professional medical advice or diagnosis.

📌 Future Enhancements

Voice & chat UI

Multi-language support

Fine-tuned medical LLM

User health history tracking