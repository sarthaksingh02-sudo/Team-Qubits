# SIDAR Learning Companion

An AI-native learning companion platform that transforms student learning from passive to proactive by centralizing fragmented digital tools into a single, context-aware dashboard.

## Overview

SIDAR (Project Disha) addresses the core problem of students being overwhelmed by fragmented digital tools (YouTube, Discord, Google Classroom) by providing an integrated ecosystem that manages the entire academic journey through AI-powered intelligence, dynamic organization, community collaboration, and integrated utilities.

## Key Features

### AI-Powered Learning
- **Syllabus Analysis**: Upload syllabus documents (PDF/images) and automatically extract topics, descriptions, and deadlines
- **Personalized Learning Paths**: AI-generated learning sequences with curated YouTube videos and articles tailored to your syllabus
- **Interactive AI Assistant**: Multimodal support for text, voice, and image queries powered by Gemini 2.5 Flash Live and Amazon Bedrock (Claude 3.5 Sonnet)
- **Weekly AI Reports**: Automated summaries of study activities with insights and recommendations

### Smart Organization
- **Centralized Dashboard**: View learning statistics, upcoming tasks, and quick actions at a glance
- **Task Scheduler**: Automatic sync with Google Calendar and Google Classroom to manage all assignments and deadlines
- **Document Editor**: Built-in note-taking with auto-save and rich text formatting
- **Wellness Mode (Bio-Sync)**: Adjust learning goals based on health factors for a balanced approach

### Collaboration
- **Study Groups**: Create or join collaborative spaces using room codes
- **Real-Time Collaboration**: Chat, share resources, and edit documents together in real-time
- **Event Discovery**: Find nearby hackathons, workshops, and seminars with AI-powered search

### Integrated Utilities
- **Spotify Integration**: Play music within the platform to maintain focus during study sessions
- **Offline Support**: Access notes and downloaded resources without internet connectivity
- **Smart Notifications**: Timely alerts for deadlines, group messages, and AI reports

## Technology Stack

### Frontend
- React 18+ with hooks
- Tailwind CSS for styling
- Shadcn/UI component library
- Zustand for state management
- React Query for server state
- Deployed via AWS Amplify

### Backend
- AWS Lambda (serverless compute)
- Amazon API Gateway (REST & WebSocket)
- Amazon Cognito (authentication)
- Amazon DynamoDB (NoSQL database)
- Amazon S3 (file storage)
- Amazon ElastiCache (Redis for caching)

### AI Services
- Amazon Bedrock with Claude 3.5 Sonnet (complex reasoning)
- Gemini API (real-time vision and voice analysis)

### Integrations
- Google Calendar API
- Google Classroom API
- Spotify Web API
- YouTube Data API

## Architecture

SIDAR follows a cloud-native, serverless architecture with clear separation between presentation, business logic, and data layers. The system uses a dual AI approach:
- Amazon Bedrock (Claude 3.5 Sonnet) for complex reasoning tasks
- Gemini API for multimodal analysis (vision and voice)

Key architectural principles:
- Serverless AWS Lambda functions for scalability
- Real-time synchronization via WebSocket
- Progressive enhancement with offline support
- Modular integration design
- Privacy by design with end-to-end encryption

## Getting Started

### Prerequisites
- Node.js 18+ and npm
- AWS account with appropriate permissions
- Google Cloud account for API access
- Spotify Developer account

### Installation

```bash
# Clone the repository
git clone https://github.com/sarthaksingh02-sudo/Team-Qubits.git
cd Team-Qubits

# Install dependencies
npm install

# Configure environment variables
cp .env.example .env
# Edit .env with your API keys and configuration

# Run development server
npm run dev
```

### Environment Variables

```
# AWS Configuration
AWS_REGION=us-east-1
AWS_ACCESS_KEY_ID=your_access_key
AWS_SECRET_ACCESS_KEY=your_secret_key

# AI Services
BEDROCK_MODEL_ID=anthropic.claude-3-5-sonnet-20241022-v2:0
GEMINI_API_KEY=your_gemini_api_key

# Google APIs
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret

# Spotify
SPOTIFY_CLIENT_ID=your_spotify_client_id
SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
```

## Project Structure

```
.kiro/
└── specs/
    └── sidar-learning-companion/
        ├── requirements.md    # Detailed requirements and user stories
        ├── design.md         # Architecture and component design
        └── tasks.md          # Implementation tasks and milestones
```

## Development Roadmap

The project is organized into phases:

1. **Foundation Phase**: Core infrastructure, authentication, and basic UI
2. **AI Integration Phase**: Syllabus analysis, learning paths, and AI assistant
3. **Collaboration Phase**: Study groups and real-time features
4. **Integration Phase**: Third-party services (Google, Spotify)
5. **Enhancement Phase**: Wellness mode, event discovery, and AI reports
6. **Polish Phase**: Performance optimization, accessibility, and testing

## Contributing

Contributions are welcome! Please read our contributing guidelines and code of conduct before submitting pull requests.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Team

Team Qubits - Building the future of AI-powered learning

## Acknowledgments

- Amazon Bedrock for powerful AI reasoning capabilities
- Google Gemini for multimodal AI analysis
- AWS for cloud infrastructure
- Open source community for amazing tools and libraries

---

**Note**: This project is currently in active development. Features and documentation are subject to change.
