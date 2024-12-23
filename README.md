# Financial Research Q&A Application
A comprehensive Question and Answer application powered by Retrieval-Augmented Generation (RAG), leveraging a knowledge base of financial research papers. This project allows users to ask questions related to trading strategies and behavioral finance and receive accurate, context-aware answers.

## Setup Instructions
### Prerequisites
Docker and Docker Compose installed on your machine.
An OpenAI API Key. Sign up at OpenAI to obtain one.
 - Clone the Repository : 
```bash
git clone https://github.com/yourusername/investiq-qna-rag.git
cd investiq-qna-rag
```
 - Set Up Environment Variables : Create a .env file in the root directory with the following content:
```env
# PostgreSQL Configuration
DB_HOST=db
DB_PORT=5432
DB_NAME=your_database_name
DB_USER=your_username
DB_PASSWORD=your_password

# Elasticsearch Configuration
ELASTICSEARCH_HOST=elasticsearch
ELASTICSEARCH_PORT=9200

# OpenAI API Key
OPENAI_API_KEY=your_openai_api_key
```
Note: Replace the placeholders with your actual credentials.
 - Prepare Data : Place your financial research papers (PDF format) in the data/ directory.

 - Build and Run the Application : Use Docker Compose to build and start all services:
```bash
docker-compose up --build
```
 - Access the Application : Open your web browser and navigate to:
```
http://localhost:8501
```

volumes:
  pgdata:
  esdata: -->
