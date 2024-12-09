# US Accounting Chatbot

A specialized chatbot application that provides expert assistance for US accounting-related queries. Built with React, FastAPI, MongoDB, and OpenAI's GPT-4.

## Features

- 💬 Real-time chat interface with a modern, responsive design
- 🧠 AI-powered responses specifically trained for US accounting topics
- 📊 MongoDB integration for chat history persistence
- ⚡ Fast and efficient FastAPI backend
- 🔒 Input validation and topic filtering
- 💎 Clean and intuitive user interface
- 📱 Mobile-responsive design

## Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Lucide React (for icons)
- Modern JavaScript (ES6+)

### Backend
- FastAPI
- OpenAI GPT-4
- MongoDB
- Python 3.8+

## Getting Started

### Prerequisites

- Node.js 14+ and npm
- Python 3.8+
- MongoDB
- OpenAI API key

### Installation

1. Clone the repository:
```bash
git clone https://github.com/finboard-dev/accounting-chatbot.git
cd accounting-chatbot
```

2. Set up the frontend:
```bash
cd frontend
npm install
```

3. Set up the backend:
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

4. Create environment variables:

Create a `.env` file in the backend directory:
```env
OPENAI_API_KEY=your_openai_api_key
MONGODB_URL=your_mongodb_url
```

### Running the Application

1. Start MongoDB:
```bash
mongod
```

2. Start the backend server:
```bash
cd backend
uvicorn main:app --reload
```

3. Start the frontend development server:
```bash
cd frontend
npm start
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend: http://localhost:8000
- API Documentation: http://localhost:8000/docs

## Project Structure

```
accounting-chatbot/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   └── ChatInterface.js
│   │   ├── App.js
│   │   └── index.js
│   ├── package.json
│   └── tailwind.config.js
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   └── .env
├── .gitignore
└── README.md
```

## API Documentation

### POST /chat
Handles chat messages and returns AI-generated responses.

Request body:
```json
{
  "message": "string",
  "session_id": "string (optional)"
}
```

Response:
```json
{
  "response": "string"
}
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenAI for providing the GPT-4 API
- FastAPI for the efficient backend framework
- React team for the frontend framework
- MongoDB team for the database solution