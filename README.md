# ManasMitra: An AI-Powered Mental Wellness Companion

ManasMitra is a confidential and empathetic mental wellness application designed to support users on their well-being journey. Powered by AI, it provides a safe space for self-reflection, personalized encouragement, and access to supportive resources.

## Key Features

- **Dashboard**: A welcoming home screen that provides a personalized greeting and a unique, AI-generated daily affirmation to start the day on a positive note.
- **Daily Check-in**: An intuitive, multi-step flow that allows users to log their mood and feelings. The app's AI assistant provides an empathetic, personalized response and suggests a relevant wellness resource based on the user's input.
- **Voice Agent**: An interactive voice-powered AI companion that provides empathetic conversation through speech-to-text and text-to-speech technology.
- **Mindfulness Sessions**: Interactive guided meditation, breathing exercises, body scans, and mindful moments with customizable duration and experience levels.
- **Progress Tracking**: A visual representation of the user's mood trends over time, helping them recognize patterns and celebrate their wellness journey.
- **Resource Hub**: A curated collection of articles, exercises, and guides on topics like guided meditation, breathing techniques, and emotional awareness.
- **Anonymous Support Forum**: A safe and anonymous community space where users can share their experiences, offer support, and connect with others who may be facing similar challenges.

## Tech Stack

This application is built with a modern, component-driven, and AI-first technology stack:

- **Framework**: [Next.js](https://nextjs.org/) (using the App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **UI Library**: [React](https://react.dev/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Component Library**: [ShadCN UI](https://ui.shadcn.com/)
- **Generative AI**: [Firebase Genkit](https://firebase.google.com/docs/genkit) with Google's Gemini models
- **Icons**: [Lucide React](https://lucide.dev/)
- **State Management**: React Hooks and Context API for client-side state.
- **Data Persistence**: Browser Local Storage for persisting user data like check-in history.
- **Deployment**: Configured for [Firebase App Hosting](https://firebase.google.com/docs/app-hosting).

## Getting Started

To get started with development, run the following command:

```bash
npm run dev
```

This will start the Next.js development server, and you can view the application by navigating to `http://localhost:9002` in your browser.

## Agentic AI System: Multi-Modal Mental Wellness Support

ManasMitra is built as an **agentic AI system** - a sophisticated network of specialized AI agents that work together to provide comprehensive mental wellness support. Unlike simple chatbots, our agentic system demonstrates autonomous decision-making, contextual awareness, and proactive user engagement across multiple interaction modalities.

### What Makes ManasMitra an Agentic AI?

1. **Autonomous Decision-Making**: Each AI agent makes independent decisions about how to respond based on user context
2. **Goal-Oriented Behavior**: Agents work toward the overarching goal of improving user mental wellness
3. **Multi-Agent Collaboration**: Different specialized agents handle specific tasks and contexts
4. **Proactive Engagement**: Agents don't just respond - they actively suggest resources, activities, and interventions
5. **Contextual Memory**: Maintains conversation history and user patterns across sessions
6. **Adaptive Responses**: Agents modify their behavior based on user emotional state and needs

## Voice Agent: AI-Powered Conversational Support

The Voice Agent is one of ManasMitra's most innovative features, providing users with an empathetic, voice-driven AI companion designed for mental wellness support. This feature combines advanced speech recognition, natural language processing, and text-to-speech synthesis to create a seamless conversational experience.

### How the Voice Agent Works

#### 1. **Speech Recognition & Input Processing**
- Uses the browser's native Web Speech API (`SpeechRecognition` or `webkitSpeechRecognition`)
- Provides real-time interim transcript display while listening
- Converts spoken words to text for AI processing
- Handles multiple languages (currently optimized for English)

#### 2. **AI Conversation Engine**
- **Model**: Powered by Google's Gemini 2.5 Flash model via Firebase Genkit
- **Personality**: ManasMitra - a caring, empathetic mental wellness assistant
- **Conversation Memory**: Maintains full conversation history for contextual responses
- **Response Style**: Designed to be supportive, non-clinical, and conversational (2-3 sentences per response)

#### 3. **Text-to-Speech Synthesis**
- **TTS Model**: Google's Gemini 2.5 Flash Preview TTS model
- **Voice**: Uses "Algenib" prebuilt voice configuration for warm, natural speech
- **Audio Format**: Generates PCM audio, converted to WAV format for browser compatibility
- **Playback**: Seamless audio playback through HTML5 Audio API

## Complete AI Agent Ecosystem

ManasMitra employs a sophisticated multi-agent architecture with **7 specialized AI agents**, each designed for specific mental wellness tasks:

### **1. Voice Agent** (`voice-agent-flow.ts`)
- **Purpose**: Real-time voice-based therapeutic conversations
- **Capabilities**: 
  - Speech-to-text processing and natural conversation
  - Empathetic listening and validation
  - Gentle questioning and self-reflection guidance
  - Crisis intervention with helpline recommendations
- **Technology**: Gemini 2.5 Flash + TTS integration

### **2. Chat Agent** (`chat-flow.ts`) 
- **Purpose**: Text-based conversational support with proactive feature suggestions
- **Capabilities**:
  - Deep emotional understanding and validation
  - Proactive app feature recommendations based on user state
  - Professional helpline provision for crisis situations
  - Contextual conversation flow management
- **Unique Features**: Actively suggests app features like Daily Check-in, Calm Pulse games, Resource Hub

### **3. Daily Affirmation Agent** (`daily-affirmations.ts`)
- **Purpose**: Generates personalized, uplifting daily affirmations
- **Capabilities**:
  - Contextual affirmation generation
  - Personalization based on user patterns
  - Positive psychology integration
- **Goal**: Start each day with personalized encouragement

### **4. Empathetic Response Agent** (`empathetic-response-to-daily-checkin.ts`)
- **Purpose**: Provides compassionate responses to daily mood check-ins
- **Capabilities**:
  - Emotional validation and understanding
  - Personalized feedback based on mood patterns
  - Encouraging and supportive messaging
- **Integration**: Works with Resource Recommendation Agent

### **5. Contextual Resource Recommendation Agent** (`contextual-resource-recommendation.ts`)
- **Purpose**: Intelligently recommends wellness resources based on user state
- **Capabilities**:
  - Analyzes check-in data for resource matching
  - Provides contextual explanations for recommendations
  - Bridges user needs with available resources
- **Smart Matching**: Connects specific emotional states to relevant wellness resources

### **6. Story Analysis Agent** (`story-analysis-flow.ts`)
- **Purpose**: Analyzes user-created stories for emotional insights
- **Capabilities**:
  - Creative content analysis
  - Emotional state identification through storytelling
  - Therapeutic feedback on creative expression
- **Therapeutic Value**: Uses narrative therapy principles

### **7. Choice Analysis Agent** (`choice-analysis-flow.ts`)
- **Purpose**: Analyzes user choices in interactive scenarios for psychological insights
- **Capabilities**:
  - Behavioral pattern recognition
  - Emotional tendency identification (Empathetic, Assertive, Cautious, etc.)
  - Non-judgmental personality insights
  - Encouraging self-awareness feedback
- **Application**: Used in interactive story games and decision-making exercises

### **Agent Orchestration & Collaboration**

- **Action Layer** (`actions.ts`): Coordinates between different agents
- **Error Resilience**: Each agent has graceful fallbacks to maintain user experience
- **Context Sharing**: Agents can access conversation history and user patterns
- **Unified Personality**: All agents embody "ManasMitra" - caring, empathetic, non-clinical
- **Crisis Protocol**: Multiple agents can trigger professional helpline recommendations

### **Agentic AI Architecture Benefits**

1. **Specialized Expertise**: Each agent is optimized for specific mental wellness tasks
2. **Scalable Intelligence**: New agents can be added without disrupting existing functionality  
3. **Contextual Switching**: System automatically selects appropriate agents based on user needs
4. **Collaborative Intelligence**: Agents work together (e.g., Check-in + Resource Recommendation)
5. **Continuous Learning**: Each agent can be fine-tuned independently based on user feedback

### Technical Architecture

```
User Speech Input
    ↓
Browser Speech Recognition API
    ↓
Text Transcription
    ↓
Voice Agent Flow (Gemini 2.5 Flash)
    ↓
AI Response Generation
    ↓
Text-to-Speech Flow (Gemini 2.5 Flash Preview TTS)
    ↓
Audio Generation & Playback
    ↓
User Hears Response
```

### Key Features of the Voice Agent

1. **Real-time Conversation**: Bidirectional voice communication with immediate feedback
2. **Emotional Intelligence**: AI trained specifically for mental wellness conversations
3. **Conversation Continuity**: Maintains context across multiple exchanges
4. **Privacy-First**: All conversations happen in real-time without permanent storage
5. **Accessibility**: Voice-first interface for users who prefer speaking over typing
6. **Cross-browser Compatibility**: Works with modern browsers supporting Web Speech API

### Usage Guidelines

The Voice Agent is designed with specific therapeutic principles:
- **Non-directive Approach**: Doesn't provide medical advice or diagnoses
- **Validation-Focused**: Acknowledges and validates user feelings
- **Strength-Based**: Highlights user resilience and past successes
- **Question-Guided**: Uses gentle questions to encourage self-reflection
- **Hope-Instilling**: Maintains optimistic, supportive tone throughout conversations

This sophisticated voice interaction system represents a cutting-edge approach to AI-powered mental wellness support, combining multiple AI models and advanced web technologies to create a truly empathetic digital companion.

## Key Features

- **Dashboard**: A welcoming home screen that provides a personalized greeting and a unique, AI-generated daily affirmation to start the day on a positive note.
- **Daily Check-in**: An intuitive, multi-step flow that allows users to log their mood and feelings. The app's AI assistant provides an empathetic, personalized response and suggests a relevant wellness resource based on the user's input.
- **Progress Tracking**: A visual representation of the user's mood trends over time, helping them recognize patterns and celebrate their wellness journey.
- **Resource Hub**: A curated collection of articles, exercises, and guides on topics like guided meditation, breathing techniques, and emotional awareness.
- **Anonymous Support Forum**: A safe and anonymous community space where users can share their experiences, offer support, and connect with others who may be facing similar challenges.

## Tech Stack

This application is built with a modern, component-driven, and AI-first technology stack:

- **Framework**: [Next.js](https://nextjs.org/) (using the App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **UI Library**: [React](https://react.dev/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Component Library**: [ShadCN UI](https://ui.shadcn.com/)
- **Generative AI**: [Firebase Genkit](https://firebase.google.com/docs/genkit) with Google's Gemini models
- **Icons**: [Lucide React](https://lucide.dev/)
- **State Management**: React Hooks and Context API for client-side state.
- **Data Persistence**: Browser Local Storage for persisting user data like check-in history.
- **Deployment**: Configured for [Firebase App Hosting](https://firebase.google.com/docs/app-hosting).

## Getting Started

To get started with development, run the following command:

```bash
npm run dev
```

This will start the Next.js development server, and you can view the application by navigating to `http://localhost:9002` in your browser.

since this is new It is just a prototype


## Tech Stack

This application is built with a modern, component-driven, and AI-first technology stack:

- **Framework**: [Next.js](https://nextjs.org/) (using the App Router)
- **Language**: [TypeScript](https://www.typescriptlang.org/)
- **UI Library**: [React](https://react.dev/)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Component Library**: [ShadCN UI](https://ui.shadcn.com/)
- **Generative AI**: [Firebase Genkit](https://firebase.google.com/docs/genkit) with Google's Gemini models
  - **Conversational AI**: Gemini 2.5 Flash for text generation
  - **Voice Synthesis**: Gemini 2.5 Flash Preview TTS for natural speech generation
- **Voice Technologies**: 
  - **Speech Recognition**: Web Speech API (SpeechRecognition/webkitSpeechRecognition)
  - **Audio Processing**: WAV audio encoding/decoding for cross-browser compatibility
  - **Audio Playback**: HTML5 Audio API
- **Icons**: [Lucide React](https://lucide.dev/)
- **State Management**: React Hooks and Context API for client-side state.
- **Data Persistence**: Browser Local Storage for persisting user data like check-in history.
- **Deployment**: Configured for [Firebase App Hosting](https://firebase.google.com/docs/app-hosting).

## Getting Started

To get started with development, run the following command:

```bash
npm run dev
```

This will start the Next.js development server, and you can view the application by navigating to `http://localhost:9002` in your browser.

since this is new It is just a prototype

