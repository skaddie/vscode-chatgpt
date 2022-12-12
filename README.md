<h2 align="center"><img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/iconWhite.png" height="64"><br>Ask ChatGPT</h2>
<p align="center"><strong>ChatGPT conversations in Visual Studio Code</strong></p>

[![Badge for version for Visual Studio Code extension gencay.vscode-chatgpt](https://vsmarketplacebadges.dev/version/gencay.vscode-chatgpt.png)](https://marketplace.visualstudio.com/items?itemName=gencay.vscode-chatgpt)

## 🆕 Update - 12/12/22

- You can now login with your email address and password without needing to hack into F12 Developer tools in your browser.
- 🤖 Let the extension log you in automatically on the browser with the credentials you provided.
- Simply enter your email and password when prompted by VS Code and let the extension log you in and grab the required tokens.
- OpenAPI may enforce a captcha question before login. Please follow the instructions on the screen during login to solve the captcha question.
- This extension will never attempt to store your personal information (email address + password). It's purely needed for the extension to work since the APIs we depend on are not from OpenAI official channels.

# ChatGPT as your copilot to level up your developer experience

- 🆕 Auto-login to start a ChatGPT session.
- ➡️ Export all your conversation history at once.
- 🔃 Option to clear and restart the conversation with ChatGPT.
- 🍻 Optimized for dialogue! Have a conversation with ChatGPT with follow-ups.
- 💯 Get help from ChatGPT within vs-code for implementing test cases, explaining it or finding bugs.
- 📝 Create projects/files with one click using built-in actions in the conversation view.
- ⚡ Built-in syntax highlighting for ChatGPT suggested code using the default code-font of your Visual Studio Code!
- 🖼️ Icon is generated by dall-e-2.

<img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/chatgpt-gif.gif">

# Features

The extension comes with context menu commands, copy/move suggested code into editor with one-click, conversation window and customization options for OpenAI's ChatGPT prompts.

## ChatGPT conversation window in vs-code

### 🆕 Export all your conversation history withs one click

<img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/export-convo.png">

---

### 🍻 Optimized for dialogue

<img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/conversation-mode-2.png">

---

### Edit and resend a previous prompt

<img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/edit-resend.png">

---

### Copy or insert the code ChatGPT is suggesting right into your editor.

<img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/code-actions.png">

---

### Ask free-form text questions that will be listed in the conversation window. The conversation is kept in cache until vs-code instance is closed.

<img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/rust.png">

---

# Use defaults or customize your code prompts

- `ChatGPT: Add Tests`: Write tests for you. Right click on a selected block of code, run command.
  - "default": "Implement tests for the following code",
  - "description": "The prompt prefix used for adding tests for the selected code"
- `ChatGPT: Find bugs`: Analyze and find bugs in your code. Right click on a selected block of code, run command.
  - "default": "Find problems with the following code",
  - "description": "The prompt prefix used for finding problems for the selected code"
- `ChatGPT: Optimize`: Add suggestions to your code to improve. Right click on a selected block of code, run command.
  - "default": "Optimize the following code",
  - "description": "The prompt prefix used for optimizing the selected code"
- `ChatGPT: Explain`: Explain the selected code. Right click on a selected block of code, run command.
  - "default": "Explain the following code",
  - "description": "The prompt prefix used for explaining the selected code"

## Other available commands

- `ChatGPT: Ask anything`: Free-form text questions within conversation window.
- `ChatGPT: Clear session`: Clears the current session. Useful in case of API errors.
- `ChatGPT: Clear conversation`: Clears the conversation window and resets the thread to start a new conversation with ChatGPT
- `ChatGPT: Export conversation`: Exports the whole conversation in Markdown for you to easily store and find the Q&A list.

## Customization settings

- You can configure the commands to use any prompts for the selected code!
- Opt-in to receive notification when ChatGPT sends you a message!

<img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/settings.png">

# Setup

Follow the instructions here to get your session token: https://github.com/transitive-bullshit/chatgpt-api#session-tokens

During your first interaction with the extension, you will be asked to enter your session token.

<img src="https://raw.githubusercontent.com/gencay/vscode-chatgpt/main/images/setup.png">

# Troubleshooting

- If the bot isn't responding, try clearing your cache by running the `ChatGPT: Clear session` command.
- It's possible that openai systems may experience issues responding to your queries due to high-traffic from time to time.
- If you get `ChatGPTAPI error 429`, it means that you are making Too Many Requests. Please wait and try again in a few moments

# Credits

- 💻 Open AI ChatGPT: https://chat.openai.com/
- 🖼️ Open AI Dall-E-2: https://openai.com/dall-e-2/
- 🧪 This extension uses unofficial OpenAI APIs. https://github.com/transitive-bullshit/chatgpt-api
