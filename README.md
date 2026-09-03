# Dizzy 💫

A lightweight, open-source English learning companion powered by AI.

Dizzy combines AI chat with practical English-learning features such as instant translation, Persian-to-English conversion, pronunciation help, and contextual language notes.

## ✨ Features

- 🤖 AI chat with OpenAI-compatible APIs
- 🇬🇧 English-focused learning experience
- 🇮🇷 Persian → English conversion
- 🌐 English → Persian translation
- 🔊 Persian phonetic pronunciation
- 💡 Short grammar and usage notes
- 🖱️ Select any text in an AI response to translate it
- 🖼️ Image attachments
- 📄 Text and code file attachments
- 💻 Markdown and code-block rendering
- 📋 One-click code copying
- 💬 Multiple local chat histories
- ✏️ Rename and delete conversations
- 💾 Local persistence using browser storage
- 🎨 Custom font support
- 🔌 Support for local models through compatible APIs
- ⚡ Streaming AI responses

## 🖥️ Screenshots

_Add screenshots here._

## 🚀 Getting Started

Dizzy is designed to be simple to run.

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/dizzy.git
cd dizzy
```

Then open `index.html` in your browser.

No build system or package manager is required.

## ⚙️ Configuration

Open **Settings** inside Dizzy and configure the Chat API.

### Chat API

Dizzy uses an OpenAI-compatible `/chat/completions` endpoint.

You can use compatible providers such as:

- Google AI Studio
- OpenAI-compatible hosted APIs
- Hugging Face endpoints
- Ollama
- LM Studio
- Other compatible services

You need to provide:

- Base URL
- API Key
- Model name

### Agent API

Dizzy uses a second API configuration for language-learning features such as:

- Persian → English conversion
- English → Persian translation
- Pronunciation
- Grammar and usage notes

A lightweight local model can be used for the Agent API.

For example:

```text
LM Studio
http://localhost:1234/v1

Ollama
http://localhost:11434/v1
```

## 🔐 Privacy & API Keys

Dizzy stores its settings and chat history locally in the browser.

Your API key is entered directly into the application and is used by the browser when making requests to the configured API endpoint.

**Never commit API keys or other secrets to this repository.**

For production or shared deployments, consider using a backend proxy instead of exposing API credentials in the browser.

## 🧠 How It Works

Dizzy uses two AI roles:

### Chat

The main AI handles conversations and English-learning interactions.

Responses are streamed from the configured OpenAI-compatible API and rendered as Markdown.

### Agent

The Agent handles language-specific utilities.

For example, selecting an English sentence can produce:

```json
[
  {
    "english": "Hello",
    "persian": "سلام",
    "pronunciation": "هِلو",
    "note": "common greeting"
  }
]
```

The Agent can also convert Persian input into natural English before sending it to the main chat.

## 🛠️ Technology

Dizzy currently uses:

- HTML
- CSS
- Vanilla JavaScript
- Browser Local Storage
- Fetch API
- OpenAI-compatible APIs
- Markdown rendering

The project intentionally has no frontend framework or build system.

## 🤝 Contributing

Contributions are welcome!

If you have an idea, find a bug, or want to improve Dizzy:

1. Open an Issue to discuss the change.
2. Fork the repository.
3. Create a branch for your change.
4. Make your changes.
5. Open a Pull Request.

Ideas for future improvements include:

- Better language-learning tools
- Vocabulary tracking
- Spaced repetition
- Flashcards
- Grammar exercises
- Progress tracking
- More local-model support
- Improved mobile experience
- Better Markdown rendering
- More customizable learning modes

## 🐛 Issues

Found a bug or have an idea?

Open an Issue and describe:

- What happened
- What you expected
- Steps to reproduce the problem
- Browser and environment information, if relevant

## 📌 Project Status

Dizzy is an evolving open-source project.

The current version is a lightweight prototype focused on experimenting with AI-powered English learning and local-first browser functionality.

Expect changes as the project grows.

## 📄 License

This project is licensed under the MIT License.

See the `LICENSE` file for details.

---

Made with 💫 and a lot of curiosity.