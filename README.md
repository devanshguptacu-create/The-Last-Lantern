
# 🕯️ The Last Lantern
### An Offline-First AI Storytelling Experience

**The Last Lantern** is an AI-powered storytelling project built for the **Ghost in the Machine** challenge. It explores how artificial intelligence can be used for creative storytelling, personal memories, and folklore.

The idea behind this project is simple: create a space where users can generate mysterious stories, turn meaningful memories into written tributes, and explore legends through AI.

Unlike applications that depend entirely on paid cloud APIs, The Last Lantern uses a locally running open-weight AI model through Ollama.

---

## ✨ Features

### 1. Haunted Archives
Generate mysterious, atmospheric stories inspired by supernatural themes, forgotten places, and unexplained events.

### 2. Memory Lantern
Turn personal memories and meaningful experiences into thoughtful written tributes. This feature is designed for remembrance and storytelling, not communication with deceased people.

### 3. Forgotten Legends
Explore folklore-inspired stories based on myths, traditions, mysterious characters, and legendary places.

### Additional Features
- Local AI story generation
- Three different storytelling modes
- Multiple language options
- Adjustable story length
- Save stories in your browser
- Copy and download generated stories
- Ambient background sound
- Responsive interface

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| CSS3 | Styling and responsive design |
| JavaScript | Application functionality |
| Ollama | Local AI model runtime |
| Qwen 2.5 3B | Story generation |
| LocalStorage | Saving stories in the browser |

---

## 🧠 How It Works

The application connects directly to a locally running Ollama instance.

1. The user selects a storytelling mode.
2. They enter a topic, idea, or memory.
3. JavaScript prepares the prompt.
4. The prompt is sent to the local Ollama API.
5. The selected AI model generates a story.
6. The generated story appears in the application.

All story generation happens through the local model rather than a paid cloud AI API.

---

## 📂 Project Structure

```text
The-Last-Lantern/
│
├── index.html
├── style.css
├── script.js
└── README.md
```

---

## ⚙️ Installation & Setup

### Prerequisites

Before running the project, make sure you have:

- A computer running Windows, Linux, or macOS
- [Ollama](https://ollama.com/) installed
- [Visual Studio Code](https://code.visualstudio.com/)
- VS Code Live Server extension

### Step 1: Clone the Repository

```bash
git clone https://github.com/devanshguptacu-create/The-Last-Lantern.git
```

### Step 2: Open the Project

```bash
cd The-Last-Lantern
```

Open the folder in Visual Studio Code.

### Step 3: Download the AI Model

Open your terminal and run:

```bash
ollama pull qwen2.5:3b
```

### Step 4: Start Ollama

```bash
ollama serve
```

If Ollama is already running in the background, you don't need to start it again.

### Step 5: Configure Browser Access

The frontend connects directly to Ollama, so browser access must be allowed through Ollama's `OLLAMA_ORIGINS` configuration.

For example, if Live Server runs at:

```text
http://127.0.0.1:5500
```

Allow that origin in Ollama's configuration and restart Ollama.

### Step 6: Run the Project

Open `index.html` using VS Code Live Server.

Make sure Ollama is running and the model is available.

You're ready to generate your first story!

---

## 🔓 Why Open Innovation?

I chose an open-weight model because I wanted to experiment with AI beyond the usual paid API approach.

Tools like Ollama make it possible to run models locally and understand how AI applications work behind the scenes.

Open innovation matters because it gives developers the freedom to experiment, learn, modify existing tools, and build applications without depending entirely on closed platforms.

For this project, it also means that personal story prompts can be processed locally instead of being sent to a third-party cloud AI service.

---

## 🔐 Privacy

- Story generation runs through a local Ollama instance.
- Saved stories are stored in browser LocalStorage.
- No cloud database is configured in this project.
- Users should avoid entering sensitive personal information into AI prompts.

---

## 🚧 Current Limitations

- Ollama must be installed and running locally.
- The required model must be downloaded before generation.
- Performance depends on the computer's available hardware.
- Browser access requires correct Ollama CORS configuration.
- Saved stories remain in the browser where they were created.

---

## 🚀 Future Improvements

Some features I would like to explore in future versions:

- More open-weight AI models
- Better storytelling controls
- Export stories as PDF
- More folklore and language options
- Improved memory organization
- A more detailed local story library

---

## 🎯 Challenge

**Event:** Ghost in the Machine  
**Theme:** Build something with open-source AI at its core.

This project explores local AI, open-weight models, and creative applications of artificial intelligence.

---

## 👨‍💻 Developer

**Kaushik Devansh Gupta**

B.Tech CSE | AI & ML Enthusiast

GitHub: [@devanshguptacu-create](https://github.com/devanshguptacu-create)

---

## 📜 License

This project can be released under the MIT License. If you choose MIT, add a `LICENSE` file containing the official MIT license text.

---

*Built with curiosity, creativity, and open AI.*
