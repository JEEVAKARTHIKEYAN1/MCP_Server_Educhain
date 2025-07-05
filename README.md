
# EduChain MCP Server Integration

## 📚 Project Overview

This project demonstrates how to integrate the [`educhain`](https://github.com/satvik314/educhain) library into an MCP (Modular Command Protocol) server to generate educational content dynamically. The MCP server is configured to expose tools and resources to external clients like **Claude Desktop**.

---

## 🛠️ Features

- ✅ Generate multiple-choice questions (MCQs) using the EduChain engine
- ✅ Generate a lesson plan for any given educational topic
- ✅ MCP-compliant server integration using the `mcp` SDK
- ✅ Compatible with Claude Desktop (via `claude_desktop_config.json`)
- ✅ Responses formatted as JSON for easy consumption

---

## 🎥 Demo Video

The demo video showing the MCP server in action is included in the repository:

[Download Demo Video](https://youtu.be/KC-IsJOx9fM?si=X3Y4qChzFZtL7ldG)

---

## 🗂️ Project Structure

```
mcp-server-demo/
│
├── .env # Environment variables (optional)
├── .gitignore # Git ignore rules
├── .python-version # Python version for pyenv (if used)
├── claude_desktop_config.json # Configuration file for Claude Desktop
├── educhain_engine.py # Custom EduChain wrapper functions
├── main.py # (Optional) Entry script
├── server.py # MCP server implementation
├── requirements.txt # Python dependencies
├── pyproject.toml # MCP project metadata
├── uv.lock # Dependency lockfile (uv)
└── README.md # This documentation
```

---

## ⚙️ Setup and Installation

### Clone the Repository:
```bash
git clone [your-github-repository-url]
cd MCP_Server_Educhain
```

### Install uv:
```bash
# On most systems:
pip install uv
```

### Install Dependencies:
```bash
uv add -r requirements.txt
```

### Set Up API Key:
1. Create a `.env` file in the root directory
2. Add your Google API key:
```
GOOGLE_API_KEY="your-api-key-goes-here"
```

---

## ▶️ How to Run

Start the MCP server from your terminal:
```bash
uv run mcp install server.py
```

The server will expose tools for generating MCQs, lesson plans, and flashcards via MCP.

---

## 📚 Resources

- [Educhain Library](https://github.com/satvik314/educhain)
- [MCP Documentation](https://modelcontextprotocol.io/introduction)
- [Claude Desktop Download](https://claude.ai/download)

