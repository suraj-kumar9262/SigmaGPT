# SigmaGPT

A MERN based ChatGPT replica implemented from scratch using OpenAI.

## Features

- Chat with an AI assistant (OpenAI gpt-4o-mini)
- Conversations are saved as threads and shown in the sidebar
- Open or delete old threads
- Replies are shown with Markdown and code highlighting

## Tech Stack

- **Frontend:** React, Vite, react-markdown
- **Backend:** Node.js, Express
- **Database:** MongoDB (Mongoose)
- **AI:** OpenAI API

## Project Structure

- `Backend/` : Express server, routes, models, OpenAI helper
- `Frontend/` : React app (chat window, chat messages, sidebar)

## Setup

### Backend

1. `cd Backend`
2. `npm install`
3. Create a file named `.env` inside the `Backend` folder and add two lines: `MONGODB_URI=your-mongodb-connection-string` and `OPENAI_API_KEY=your-openai-api-key`
4. `node server.js`

The server runs on port 8080.

### Frontend

1. `cd Frontend`
2. `npm install`
3. `npm run dev`

The app opens at http://localhost:5173

## Note

Never commit your `.env` file. It is already listed in `.gitignore`. An OpenAI API key with available credit is needed to get replies.
