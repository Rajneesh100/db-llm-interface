# AI Chat Frontend

A modern React-based chat interface for the AI multi-agent system.

## Features

- 🎨 **Modern UI**: Clean, responsive design with gradient backgrounds
- 💬 **Real-time Chat**: Instant messaging with AI assistant
- 📱 **Mobile Friendly**: Responsive design that works on all devices
- ⚡ **Auto-scroll**: Messages automatically scroll up as new ones arrive
- 🔄 **Loading States**: Visual feedback with typing indicators
- 🎯 **Order Management**: Specialized for database and order queries

## Project Structure

```
frontend/
├── public/
│   └── index.html
├── src/
│   ├── App.js          # Main chat component
│   ├── App.css         # Styling for the chat interface
│   ├── index.js        # React entry point
│   └── index.css       # Global styles
└── package.json        # Dependencies and scripts
```

## Getting Started

### Prerequisites

- Node.js (version 14 or higher)
- npm or yarn

### Installation

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Open your browser and go to `http://localhost:5600`

### Backend Setup

Make sure the Flask backend is running on `http://localhost:4500`:

```bash
cd backend
pip install -r requirements.txt
python app.py
```

## Usage

1. **Start Chatting**: Type your message in the input field at the bottom
2. **Send Messages**: Press Enter or click the send button
3. **Order Queries**: Ask about orders, line items, or database operations
4. **Auto-scroll**: New messages automatically appear at the bottom

## API Endpoints

The frontend communicates with these backend endpoints:

- `POST /api/chat` - Send message to AI agent
- `GET /api/health` - Health check endpoint

## Styling Features

- **Gradient Backgrounds**: Beautiful purple-blue gradients
- **Message Bubbles**: Distinct styling for user vs AI messages
- **Smooth Animations**: Hover effects and smooth scrolling
- **Typing Indicator**: Animated dots while AI is responding
- **Responsive Design**: Adapts to different screen sizes

## Customization

### Colors
The main color scheme uses these CSS variables:
- Primary gradient: `#667eea` to `#764ba2`
- Background: `#f5f5f5`
- Message bubbles: Gradient for user, light gray for AI

### Message Styling
- User messages: Right-aligned with gradient background
- AI messages: Left-aligned with light background
- Timestamps: Small, subtle text below each message

## Troubleshooting

### Common Issues

1. **CORS Errors**: Make sure the Flask backend has CORS enabled
2. **Connection Refused**: Ensure the backend is running on port 4500
3. **Styling Issues**: Clear browser cache and restart the dev server

### Development Tips

- Use browser dev tools to inspect network requests
- Check the console for any JavaScript errors
- Ensure both frontend (port 5600) and backend (port 4500) are running

## Production Build

To create a production build:

```bash
npm run build
```

This creates an optimized build in the `build/` folder that can be deployed to any static hosting service.
