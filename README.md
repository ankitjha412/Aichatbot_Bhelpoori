 # Bullieverse Chatbot

The **Bulliverse Chatbot** is an AI-powered assistant designed to enhance the **Bulliverse gaming platform**. It allows players to interact with the game using natural language, providing real-time, dynamic responses to game-related queries. The chatbot also integrates with the **Beyond API** to generate AI-powered content and assist with image creation, further enriching the gaming experience.

## Features
- **Game-related queries**: The chatbot can answer questions about Bulliverse, its game mechanics, and NFTs.
- **Image Generation**: The chatbot can generate images based on user prompts using the Beyond API.
- **AI-Powered Content**: Uses **meta-llama/Meta-Llama-3-8B-Instruct-Turbo** to generate intelligent responses to user input.
- **Easy Integration**: With the API routes set up, you can easily integrate new features or extend functionality.
  
## Tech Stack
- **Backend**: Node.js, Express
- **AI Integration**: Beyond API, meta-llama/Meta-Llama-3-8B-Instruct-Turbo
- **Image Generation**: Beyond API (FLUX.1-schnell)
- **API**: RESTful API
- **Authentication**: API Keys for secure access to Beyond API
- **Middleware**: Body Parser for JSON request handling

## Setup Instructions
To get the project up and running on your local machine, follow these steps:

### Prerequisites
- Node.js v16 or later
- npm or yarn

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/bullieverse-chatbot.git
   cd bullieverse-chatbot
2. **Install Dependencies: Use npm or yarn to install the required packages**:
    ```bash
    npm install
    ```
3. **Set Up API Key**:
   ```
   BEYOND_API_KEY=your-api-key-here
   ```
4. **Run the Application: Once everything is set up, start the server**:
    ```
    npm start
    ```

**How to Use**
1. Interact with the chatbot: Send a POST request to /api/chat/completions with a message asking about Bulliverse or the game mechanics.
2. Generate Images: Use the /api/images/generate endpoint to create images based on specific prompts. For example, create images for NFTs, game characters, or environments.
3. Check API Connectivity: Send a GET request to /api/test-beyond-api to ensure your server is correctly connected to the Beyond API.

```
Bulliverse-Chatbot/
│
├── backend/                  # Backend folder
│   ├── node_modules/         # Node.js dependencies
│   ├── src/                  # Source files
│   │   ├── controllers/      # Logic for handling requests
│   │   │   └── chatController.js  # Chat controller
│   │   ├── routes/           # API routes
│   │   │   └── chatRoutes.js    # Routes for handling chat requests
│   │   ├── server.js         # Server entry point
│   │   ├── app.js            # Main app file where routes are configured
│   │   └── config.js         # Configuration file (API keys, URLs)
│   ├── package.json          # Node.js project details and dependencies
│   └── .env                  # Environment variables (e.g., API keys)
│
├── frontend/                 # Frontend folder
│   ├── public/               # Public folder for static assets
│   │   └── index.html        # Main HTML file
│   ├── src/                  # Frontend source code
│   │   ├── components/       # React components
│   │   │   └── ChatComponent.js   # Component to display chat UI
│   │   ├── App.js            # Main React application file
│   │   ├── index.js          # Entry point for React app
│   │   └── style.css         # CSS file for styling the frontend
│   ├── package.json          # Frontend project details and dependencies
│   └── .gitignore            # Git ignore file
│
├── README.md                # Project documentation
└── .gitignore               # Ignore node_modules, .env, etc.

```

![image](https://github.com/user-attachments/assets/fd820c70-8c6e-44d9-977b-ba18fbfed9aa)

![image](https://github.com/user-attachments/assets/7e2496bf-01ee-4768-b147-9663b377ae21)

![image](https://github.com/user-attachments/assets/db49c570-d39c-48d5-842d-c60bc84a7141)
