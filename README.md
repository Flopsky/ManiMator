# ManiMator - Scientific Text to Video Explainer

ManiMator is an AI-powered platform that transforms scientific text into engaging, Feynman-style video explanations using Manim animations and Kokoro TTS.

## Features

- 📝 Input any scientific text
- 🎥 Generate Feynman-style video explanations
- 🤖 Powered by Gemini (OpenDeepWiki) for intelligent content generation
- 🎬 High-quality Manim animations (3Blue1Brown style)
- 🗣️ Natural voice synthesis with Kokoro TTS
- 💻 Modern web interface built with Next.js and ChatCN

## Tech Stack

- **Frontend**: Next.js 14, ChatCN, TailwindCSS
- **Backend**: Python FastAPI
- **Video Engine**: Manim
- **TTS**: Kokoro
- **AI**: Gemini (OpenDeepWiki)
- **Styling**: TailwindCSS

## Project Structure
```t
ManiMator/
├── frontend/ # Next.js frontend application
├── backend/ # Python FastAPI backend
│ ├── api/ # API routes and services
│ ├── video_engine/ # Manim and Kokoro integration
│ └── gemini/ # Gemini AI integration
└── docs/ # Project documentation
```

## Setup

### Prerequisites

- Python 3.9+
- Node.js 18+
- FFmpeg
- LaTeX (for Manim)

### Backend Setup

1. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your API keys
```

### Frontend Setup

1. Install dependencies:
```bash
cd frontend
npm install
```

2. Start the development server:
```bash
npm run dev
```

## Environment Variables

Create a `.env` file with the following variables:

```env
GEMINI_API_KEY=your_gemini_api_key
```

## Usage

1. Start the backend server:
```bash
cd backend
uvicorn main:app --reload
```

2. Start the frontend development server:
```bash
cd frontend
npm run dev
```

3. Open `http://localhost:3000` in your browser

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.