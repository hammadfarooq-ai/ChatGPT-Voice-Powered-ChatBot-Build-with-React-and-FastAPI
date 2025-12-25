# ChatGPT Voice-Powered ChatBot

A modern, voice-powered chatbot application built with React and FastAPI. This project enables users to interact with ChatGPT through voice input and receive AI-generated responses with text-to-speech capabilities.

## 🚀 Features

- **Voice Input**: Record and send voice messages to the chatbot
- **AI-Powered Responses**: Get intelligent responses from ChatGPT (OpenAI GPT)
- **Text-to-Speech**: Listen to AI responses using Eleven Labs voice synthesis
- **Modern UI**: Beautiful, responsive interface built with React and TailwindCSS
- **Real-time Communication**: Seamless interaction between frontend and backend
- **TypeScript Support**: Fully typed codebase for better development experience

## 🛠️ Tech Stack

### Frontend
- **React 18.2.0** - UI library
- **TypeScript** - Type-safe JavaScript
- **Vite** - Fast build tool and dev server
- **TailwindCSS** - Utility-first CSS framework
- **Axios** - HTTP client for API requests
- **react-media-recorder** - Voice recording functionality

### Backend
- **FastAPI** - Modern Python web framework
- **OpenAI API** - ChatGPT integration
- **Eleven Labs API** - Text-to-speech synthesis

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v16 or higher) and **npm/yarn**
- **Python** (v3.8 or higher) and **pip**
- **OpenAI API Key** - Get yours at [OpenAI Platform](https://platform.openai.com/account/api-keys)
- **OpenAI Organization ID** - Available at [OpenAI Org Settings](https://platform.openai.com/account/org-settings)
- **Eleven Labs API Key** - Subscribe and get your key at [Eleven Labs](https://beta.elevenlabs.io/subscription)

## 📦 Installation

### 1. Clone the Repository

```bash
git clone <repository-url>
cd ChatGPT-Voice-Powered-ChatBot-Build-with-React-and-FastAPI
```

### 2. Frontend Setup

Navigate to the frontend directory (Section 3):

```bash
cd Section\ 3
```

Install dependencies:

```bash
npm install
# or
yarn install
```

### 3. Backend Setup

Create a virtual environment (recommended):

```bash
python -m venv venv
```

Activate the virtual environment:

**Windows:**
```bash
venv\Scripts\activate
```

**macOS/Linux:**
```bash
source venv/bin/activate
```

Install Python dependencies:

```bash
pip install fastapi uvicorn openai python-dotenv elevenlabs
```

## ⚙️ Configuration

### Environment Variables

Create a `.env` file in the backend directory with the following variables:

```env
OPENAI_API_KEY=your_openai_api_key_here
OPENAI_ORG_ID=your_openai_org_id_here
ELEVEN_LABS_API_KEY=your_elevenlabs_api_key_here
```

### Frontend Configuration

Update the API endpoint in your frontend code to point to your FastAPI backend (typically `http://localhost:8000`).

## 🚀 Running the Application

### Start the Backend Server

Navigate to your backend directory and run:

```bash
uvicorn main:app --reload --port 8000
```

The API will be available at `http://localhost:8000`

### Start the Frontend Development Server

In the frontend directory (Section 3), run:

```bash
npm run dev
# or
yarn dev
```

The frontend will be available at `http://localhost:5173` (or the port shown in the terminal)

## 📁 Project Structure

```
ChatGPT-Voice-Powered-ChatBot-Build-with-React-and-FastAPI/
│
├── Section 3/                    # Main frontend application
│   ├── src/
│   │   ├── components/           # React components
│   │   ├── App.tsx               # Main app component
│   │   └── main.tsx              # Entry point
│   ├── package.json              # Frontend dependencies
│   └── vite.config.ts            # Vite configuration
│
├── React Crash Course/            # Tutorial/example project
│   └── src/                      # Example React components
│
├── Section 2/                     # Additional resources
│   └── Random Org URL.txt        # API reference
│
├── Presentation/                  # Project documentation
│   └── RachelChat.pdf            # Presentation slides
│
├── API Keys.txt                   # API key setup instructions
├── LICENSE                        # MIT License
└── README.md                      # This file
```

## 🎯 Usage

1. **Start both servers** (backend and frontend) as described above
2. **Open your browser** and navigate to the frontend URL
3. **Click the record button** to start recording your voice message
4. **Speak your question** or message
5. **Stop recording** to send the audio to the backend
6. **Wait for the AI response** - you'll see the text response and hear the audio playback

## 🔧 API Endpoints

The FastAPI backend should expose the following endpoints:

- `POST /chat` - Send voice message and receive AI response
- `POST /text-to-speech` - Convert text to speech
- `GET /health` - Health check endpoint

## 🧪 Development

### Frontend Development

```bash
cd Section\ 3
npm run dev        # Start dev server
npm run build      # Build for production
npm run start      # Preview production build
```

### Backend Development

```bash
uvicorn main:app --reload    # Development with auto-reload
uvicorn main:app --host 0.0.0.0 --port 8000  # Production-like
```

## 📝 Notes

- Make sure your API keys are kept secure and never committed to version control
- The `React Crash Course` folder contains example code and is separate from the main application
- For production deployment, configure CORS settings appropriately
- Consider implementing rate limiting for API endpoints

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [OpenAI](https://openai.com/) for the ChatGPT API
- [Eleven Labs](https://elevenlabs.io/) for text-to-speech capabilities
- [FastAPI](https://fastapi.tiangolo.com/) for the excellent Python framework
- [React](https://react.dev/) and [Vite](https://vitejs.dev/) for the frontend stack

## 📚 Additional Resources

- **Discord Community**: [Code Raiders Discord](https://discord.gg/ASFBebf9ZR)
- **YouTube Tutorials**:
  - [Code Raiders Channel](https://youtu.be/IJiadKeipco)
  - [Crypto Wizards Channel](https://youtu.be/uElOqz-Htos)

## 🐛 Troubleshooting

### Common Issues

1. **CORS Errors**: Make sure your FastAPI backend has CORS middleware configured
2. **API Key Errors**: Verify your API keys are correctly set in the `.env` file
3. **Port Conflicts**: Change the port in your configuration if 8000 or 5173 are already in use
4. **Audio Recording Issues**: Ensure your browser has microphone permissions enabled

### Getting Help

If you encounter any issues:
1. Check the console for error messages
2. Verify all dependencies are installed correctly
3. Ensure API keys are valid and have sufficient credits
4. Join the Discord community for support

---

**Built with ❤️ using React and FastAPI**
