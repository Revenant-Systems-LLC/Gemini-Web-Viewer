# Iris: A Portal For Gemini To "See" The Web In Real Time  (Powered by Gemini)

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Version: 1.0](https://img.shields.io/badge/Version-1.0-blue.svg)
![Powered by: Google Gemini](https://img.shields.io/badge/Powered%20by-Google%20Gemini-blueviolet.svg)

Iris is a sophisticated Tampermonkey userscript that embeds a conversational AI assistant directly into your browser. It allows you to have intelligent, context-aware conversations about the content of any webpage you visit, powered by Google's Gemini API.

---

## Features

* **Context-Aware Conversations**: Automatically reads the main text of a webpage to provide relevant answers.
* **Conversational Memory**: Remembers previous questions and answers for natural, follow-up interactions.
* **Selected Text Analysis**: Highlight any text on a page to focus the conversation specifically on that snippet.
* **Polished & Draggable UI**: A clean, modern chat interface that you can move anywhere on the screen.
* **Secure API Key Management**: Uses a local Node.js proxy server to keep your Google Gemini API key completely secure and off the client-side.
* **Markdown Rendering**: Displays formatted responses, including code blocks, lists, and emphasis.
* **AI Model Selection**: Easily switch between different Gemini models (e.g., 1.5 Flash, 1.5 Pro) directly from the UI.

---

## Project Motivation

This project was born from a simple idea: to give a large language model "eyes" to see the web. I wanted to break the barrier of the isolated chat window and create a tool that could perceive and discuss the content I was actively browsing. Iris is the result—a seamless bridge between the user, the web, and the power of generative AI.

---

## Technology Stack

**Frontend**: JavaScript (ES6+), Tampermonkey
**Backend Proxy**: Node.js, Express.js
**AI**: Google Gemini API

---

## 🚀 Installation & Setup

This project has two components that need to be set up: the **Backend Proxy** (to handle the API key) and the **Userscript** (the tool itself).

### Part 1: The Backend Proxy (API Server)

The proxy server runs locally on your machine to securely manage your API key.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Revenant-Systems-LLC/Gemini-Web-Viewer.git](https://github.com/Revenant-Systems-LLC/Gemini-Web-Viewer.git)
    ```
2.  **Navigate to the proxy directory:**
    ```bash
    cd Gemini-Web-Viewer/proxy
    ```
3.  **Install dependencies:**
    ```bash
    npm install
    ```
4.  **Create your environment file:** Copy the example file.
    ```bash
    cp .env.example .env
    ```
5.  **Add your API Key:** Open the new `.env` file in a text editor and replace `YOUR_API_KEY_HERE` with your actual Google Gemini API key.

6.  **Start the server:**
    ```bash
    node server.js
    ```
    The server will now be running on `http://localhost:3000`. You must keep this server running in the background while using the userscript.

### Part 2: The Userscript (Frontend)

1.  Install the [Tampermonkey](https://www.tampermonkey.net/) browser extension for your browser (Chrome, Firefox, Edge, etc.).
2.  Make sure your local proxy server from Part 1 is running.
3.  Navigate to the [`iris-web-viewer.user.js`](https://github.com/Revenant-Systems-LLC/Gemini-Web-Viewer/blob/main/iris-web-viewer.user.js) file in this repository.
4.  Click the **"Raw"** button at the top right of the file view.
5.  Tampermonkey will open a new tab and prompt you to install the script. Click **"Install."**

### Part 2: The Userscript (Frontend)

1.  Install the [Tampermonkey](https://www.tampermonkey.net/) browser extension for your browser (Chrome, Firefox, Edge, etc.).
2.  Make sure your local proxy server from Part 1 is running.
3.  Navigate to the [`iris-web-viewer.user.js`](https://github.com/Revenant-Systems-LLC/Gemini-Web-Viewer/blob/main/iris-web-viewer.user.js) file in this repository.
4.  Click the **"Raw"** button at the top right of the file view.
5.  Tampermonkey will open a new tab and prompt you to install the script. Click **"Install."**

---

## Usage

Once installed and with the proxy running, a star icon (✧) will appear in the bottom-right corner of any webpage.

* **Click the icon** to open the Iris chat window.
* **Ask a question** about the page, or **highlight text** before asking to focus on a specific detail.
* **Drag the window header** to move it wherever you like.

---

## ⚖️ License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Copyright (c) 2025 Revenant Systems LLC
