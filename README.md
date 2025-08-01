A lightweight Chrome extension that integrates ChatGPT directly into your browser experience — enabling you to send selected webpage content to ChatGPT using modular plugins like "Default", "Gangster", or "Image".



🚀 Features
🧠 Access ChatGPT directly on any website

🧩 Use modular plugins to change prompt behavior (fun, creative, or image-based)

⚡ Real-time responses from ChatGPT displayed in-page

🔐 API key protected with environment variables



🛠️ Tech Stack
Layer	Tech Used
Frontend    	Chrome Extension APIs, Vanilla JS
Backend	      Node.js, Express, chatgpt (npm)
Security	    dotenv-safe, CORS
Plugins      	Modular JavaScript plugin architecture



⚙️ How It Works
User installs the extension and visits any webpage.

content.js is injected into the page and monitors for user interactions.

User selects text and a plugin (e.g., Gangster.js) modifies the prompt.

The prompt is sent to a Node.js server running locally or remotely.

Server uses the ChatGPT API via the chatgpt npm package.

GPT response is sent back and injected directly into the page.



🧑‍💻 Local Setup

1. Clone the Repo
   
   git clone https://github.com/aditi02verma/gpt-chrome-extension.git

   cd gpt-chrome-extension

2. Install Backend Dependencies

   npm install

3.  Configure Environment

    Create a .env file based on .env.example:

    OPENAI_API_KEY=your-openai-api-key



4. Start the Server
   npm start



5. Load the Chrome Extension

   Go to chrome://extensions/

   Enable Developer Mode

   Click Load Unpacked

   Select the /extension folder




 
 Demo:



https://github.com/user-attachments/assets/6e30aa25-8648-4821-9efc-95719a5e3905


