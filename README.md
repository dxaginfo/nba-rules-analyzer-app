# RuleBook Bot - NBA Rules Analyzer

An AI-powered NBA rules chatbot that helps users understand complex basketball rules through a simple conversational interface.

## Project Overview

The RuleBook Bot is designed to make the complex NBA rulebook more accessible to fans, referees, players, and coaches. By providing a conversational interface, users can quickly get clear explanations of NBA rules and officiating standards without having to search through lengthy documentation.

### Key Features

- **Natural Language Rule Queries**: Ask about any NBA rule in plain English
- **Officiating Explanations**: Get explanations for common referee decisions
- **Visual Examples**: View diagrams illustrating rule applications
- **Rule Citation**: Receive exact references to official NBA rulebook sections
- **Keyword Search**: Find rules related to specific basketball terms or situations
- **Mobile-Friendly Design**: Access rule information on any device

## Technology Stack

- **Frontend**: React with TypeScript
- **UI Framework**: Tailwind CSS
- **Backend**: Node.js with Express
- **Database**: MongoDB (for storing query history and user feedback)
- **NLP/AI**: Pretrained language model fine-tuned on NBA rulebook content
- **Deployment**: Docker, AWS/Vercel

## Architecture

The application follows a client-server architecture:

1. **Frontend (React/TypeScript)**
   - Chat interface with message history
   - Rule visualization components
   - Responsive design for all devices
   - Accessibility features

2. **Backend API (Node.js/Express)**
   - RESTful endpoints for rule queries
   - Authentication for saved history (optional)
   - Rule database management
   - Query logging and analytics

3. **AI Component**
   - Pre-trained NLP model fine-tuned on NBA rulebook
   - Context management for multi-turn conversations
   - Rule citation and reference extraction
   - Confidence scoring for responses

4. **Database (MongoDB)**
   - NBA rulebook structured data
   - User query history (optional)
   - Feedback and improvement suggestions
   - Usage analytics

## Getting Started

### Prerequisites
- Node.js (v14+)
- npm or yarn
- MongoDB (local or Atlas)

### Installation

1. Clone the repository
```bash
git clone https://github.com/dxaginfo/nba-rules-analyzer-app.git
cd nba-rules-analyzer-app
```

2. Install dependencies
```bash
# Install frontend dependencies
cd client
npm install

# Install backend dependencies
cd ../server
npm install
```

3. Set up environment variables
```bash
# In the server directory, create a .env file with:
PORT=5000
MONGODB_URI=mongodb://localhost:27017/nba-rules
# Add any API keys required for the AI model
```

4. Start the development servers
```bash
# Start backend
cd server
npm run dev

# In a new terminal, start frontend
cd client
npm start
```

5. Open your browser to `http://localhost:3000`

## Project Status

This application is currently in active development. Initial MVP features are being implemented.

## License

MIT

## Acknowledgments

- NBA for public rulebook information
- Basketball officials who contribute expertise
- Open source AI and NLP communities