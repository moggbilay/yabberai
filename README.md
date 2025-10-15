# Yabber App

<p align="left">
  <img src="https://raw.githubusercontent.com/moggbilay/yabberai/main/white-logo.png" alt="Yabber App Logo" width="150"/>
</p>

> An intelligent AI-powered desktop assistant for document analysis and conversation

Yabber App is a desktop application that provides specialized AI workspaces for different tasks. Built with Electron and powered by local AI models through Ollama, it offers privacy-focused AI assistance without sending your data to the cloud.

---

## Features

### AI Workspaces
Create dedicated workspaces for different purposes:
- **Arabic Writing** - Native Arabic language support with proper grammar and cultural context
- **Coding** - Programming assistance with code examples and explanations
- **Novel Writing** - Creative storytelling and narrative development
- **Academic Research** - Scholarly writing and research support
- **Mathematics** - Step-by-step problem solving and explanations
- **Custom** - Use any Ollama model for specialized tasks

### Core Capabilities
- **Document Upload** - Analyze and chat about your documents (PDF, TXT, DOCX)
- **Web Search** - Enable real-time web search for up-to-date information
- **Persistent History** - All conversations are saved locally
- **Bilingual Interface** - Full support for English and Arabic
- **Dark/Light Themes** - Choose your preferred visual style
- **Privacy First** - All processing happens locally on your machine

---

## Installation

### Step 1: Install Ollama

Ollama is required to run the AI models locally on your computer.

1. **Download Ollama**
   - Visit [ollama.ai](https://ollama.ai/)
   - Download the Windows installer
   - Run the installer and follow the setup wizard

2. **Verify Installation**
   - Open Command Prompt or PowerShell
   - Run: `ollama --version`
   - You should see the version number

3. **Download AI Models**
   
   Open Command Prompt or PowerShell and run these commands to download the AI models:

   ```bash
   # Arabic language model (Required for Arabic workspace)
   ollama pull prakasharyan/qwen-arabic:latest

   # Coding assistant (Required for Coding workspace)
   ollama pull qwen2.5-coder:1.5b

   # Creative writing (Required for Novel workspace)
   ollama pull phi3:mini

   # Academic research (Required for Academic workspace)
   ollama pull llama3.2:3b

   # Mathematics (Required for Math workspace)
   ollama pull falcon3:1b
   ```

   **Note:** You can install only the models you need. Each model is 1-3 GB in size.

4. **Verify Ollama is Running**
   - Ollama should start automatically after installation
   - Check the system tray for the Ollama icon
   - Or run: `ollama list` to see installed models

### Step 2: Install Yabber App

1. **Download the Installer**
   - Go to the [Releases](../../releases) page
   - Download `Yabber App-Setup-1.0.0.exe`

2. **Run the Installer**
   - Double-click the downloaded file
   - Windows may show a security warning - click "More info" then "Run anyway"
   - Follow the installation wizard:
     - Choose installation directory (default: `C:\Program Files\Yabber App`)
     - Select whether to create desktop shortcut
     - Click "Install"

3. **First Launch**
   - The installer will create shortcuts on your desktop and start menu
   - Launch Yabber App from the shortcut
   - **Wait 10-15 seconds** for the backend server to initialize
   - The main window will open automatically when ready

4. **Initial Setup**
   - The app will check for Ollama connectivity
   - If Ollama is not detected, you'll see a warning message
   - Ensure Ollama is running and models are downloaded

### System Requirements

- **Operating System:** Windows 10 or Windows 11 (64-bit)
- **RAM:** Minimum 8 GB (16 GB recommended for larger models)
- **Storage:** 5-10 GB free space (depending on AI models)
- **Processor:** Modern multi-core CPU (Intel i5/AMD Ryzen 5 or better)
- **Internet:** Required for web search feature and initial model downloads

---

## Usage

### Getting Started

1. **Create Your First Workspace**
   - Click the "+" button in the sidebar
   - Select a workspace type based on your task
   - Give it a descriptive name
   - Click "Create"

2. **Start a Conversation**
   - Select your workspace from the sidebar
   - Type your message in the input box at the bottom
   - Press Enter or click the Send button
   - Wait for the AI to respond

3. **Upload Documents** (Optional)
   - Click the upload icon (📎) in the toolbar
   - Select your document (supports PDF, TXT, DOCX, and more)
   - The AI will analyze the document
   - Ask questions about the document content

4. **Enable Web Search** (Optional)
   - Toggle the "🌐 Web Search" button in the toolbar
   - When enabled, the AI can search the web for current information
   - Useful for questions requiring up-to-date data

### Managing Workspaces

- **Switch Workspaces:** Click on any workspace in the sidebar
- **Delete Workspace:** Click the trash icon (🗑️) next to the workspace name
- **Search Workspaces:** Use the search box at the top of the sidebar
- **View Chat History:** All messages are automatically saved per workspace

### Settings

Click the settings icon (⚙️) in the top-right to:
- **Change Theme:** Switch between Dark and Light mode
- **Change Language:** Switch between English and Arabic
- **View Ollama Status:** Check AI model connectivity

### Keyboard Shortcuts

- `Enter` - Send message
- `Shift + Enter` - New line in message
- `Ctrl + N` - New workspace
- `Ctrl + ,` - Open settings

---

**⭐ If you find this project useful, please star the repository!**

