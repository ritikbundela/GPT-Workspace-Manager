# GPT Workspace Manager

A Chrome extension that enhances ChatGPT with a prompt index sidebar, context transfer between chats, and AI-powered conversation summaries.

## Features

- **Prompt Index Panel** - View all your prompts in the current chat
- **Context Transfer** - Continue conversations in new chats with AI summaries
- **Star & Rename Prompts** - Mark and customize important prompts
- **Dark/Light Mode** - Auto theme switching
- **Persistent Storage** - Saves all your customizations
### Screenshots
**Without Workspace Tool:**
![Without Tool](https://github.com/ritikbundela/GPT-Workspace-Manager/raw/main/icons/without%20workspace%20tool.png)

**With Workspace Manager:**
![With Tool](https://github.com/ritikbundela/GPT-Workspace-Manager/raw/main/icons/with%20workspace%20tool.png)

## Installation

1. Clone this repository
2. Get a free [Groq API key](https://console.groq.com/)
3. Open `inject.js` and replace `YOUR_API_KEY_HERE` with your actual API key
4. Open Chrome → `chrome://extensions/`
5. Enable "Developer mode"
6. Click "Load unpacked" and select this folder

## Usage

- Click the hamburger menu icon (☰) in bottom-right corner on ChatGPT
- View and navigate your prompts
- Star important prompts with ⭐
- Rename prompts with ✏️
- Use "New Chat with Context" to transfer conversation context


### Using "New Chat with Context"

This feature transfers your conversation context to a new chat using AI-powered summarization:

1. **Click "New Chat with Context"** button in the panel
   - Wait for the AI to generate a summary (may take a few seconds)
   - A new ChatGPT tab will open automatically

2. **In the new tab, click the extension icon (☰) twice**
   - First click: Opens the panel
   - Second click: Closes the panel
   - This activates the extension in the new tab

3. **Click "Paste Context" button** that appears at the top
   - Press `Ctrl+V` (or `Cmd+V` on Mac) to paste the context
   - The AI-generated summary will appear in the input box
   - Press Enter to send and continue your conversation

**Note:** You must click the hamburger icon twice in the new tab to initialize the extension before the "Paste Context" button appears.

## Privacy

- All data stored locally in Chrome storage
- API calls only to Groq (for context summaries)
- No third-party tracking
- Open source

## Troubleshooting

**"Paste Context" button not appearing?**
- Make sure you clicked the extension icon (☰) twice in the new tab
- Refresh the page and try again

**Context transfer not working?**
- Verify your Groq API key is correct in `inject.js`
- Check browser console (F12) for error messages


## License

MIT License - See LICENSE file
