# NextAI

NextAI is a full-stack PDF question-answering application. Users can upload a PDF, ask questions about its contents by typing or speaking, and receive text or spoken answers.

## Project structure

```text
nextai/
|-- public/                    # Static frontend files
|-- src/
|   |-- components/
|   |   |-- ChatComponent.js   # Text and voice questions
|   |   |-- PdfUploader.js     # PDF upload interface
|   |   `-- RenderQA.js        # Question and answer display
|   `-- App.js                 # Main React application
|-- server/
|   |-- chat.js                # PDF retrieval and question answering
|   |-- server.js              # Express server and upload routes
|   |-- package.json
|   `-- package-lock.json
|-- package.json
`-- package-lock.json
```

## Prerequisites

- Node.js 18 or later
- npm
- [OpenAI API key](https://platform.openai.com/api-keys)

## Setup

Install the frontend dependencies:

```bash
npm install
```

Install the backend dependencies:

```bash
cd server
npm install
```

Create `server/.env`:

```env
REACT_APP_OPENAI_API_KEY=your_openai_api_key
```

Create a `server/uploads` folder.

## Run the project

Run the frontend and backend together from the project root:

```bash
npm run dev
```

- Frontend: [http://localhost:3000](http://localhost:3000)
- Backend: [http://localhost:5001](http://localhost:5001)

Run only the frontend:

```bash
npm start
```

Run only the backend:

```bash
cd server
npm start
```
