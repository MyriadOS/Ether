# Aeth 🤖

![image](https://github.com/user-attachments/assets/1095f6a0-3ec2-4dc7-8f59-66ccaf281342)


## ✨ Features

- 🛠️ Full-featured Discord, Twitter and Telegram connectors
- 🔗 Support for every model (Llama, Grok, OpenAI, Anthropic, etc.)
- 👥 Multi-agent and room support
- 📚 Easily ingest and interact with your documents
- 💾 Retrievable memory and document store
- 🚀 Highly extensible - create your own actions and clients
- ☁️ Supports many models (local Llama, OpenAI, Anthropic, Groq, etc.)
- 📦 Just works!

## Video Tutorials

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Use Cases

- 🤖 Chatbots
- 🕵️ Autonomous Agents
- 📈 Business Process Handling
- 🎮 Video Game NPCs
- 🧠 Trading

## 🚀 Quick Start

### Prerequisites

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Note for Windows Users:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) is required.

### Use the Starter (Recommended)

```bash
git clone https://github.com/aetheros/aether-starter.git
cd aether-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```
Once the agent is running, You should see the message to run "pnpm start:client" at the end.
Open another terminal and move to the same directory, then run the command below and follow the URL to chat with your agent.
```bash
pnpm start:client
```

Then read the [Documentation](https://aetheros.github.io/aether/) to learn how to customize your Aether.

### Manually Start Aether (Only recommended if you know what you are doing)

```bash
# Clone the repository
git clone https://github.com/aetheros/aether.git

# Checkout the latest release
# This project iterates fast, so we recommend checking out the latest release
git checkout $(git describe --tags --abbrev=0)
```

### Start Aether with Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/aetheros/aether/tree/main)

### Edit the .env file

Copy .env.example to .env and fill in the appropriate values.

```
cp .env.example .env
```

Note: .env is optional. If you plan to run multiple distinct agents, you can pass secrets through the character JSON.

### Automatically Start Aether

This will run everything to set up the project and start the bot with the default character.

```bash
sh scripts/start.sh
```

### Edit the character file

1. Open `packages/core/src/defaultCharacter.ts` to modify the default character. Uncomment and edit.

2. To load custom characters:
    - Use `pnpm start --characters="path/to/your/character.json"`
    - Multiple character files can be loaded simultaneously.
3. Connect with X (Twitter):
    - Change `"clients": []` to `"clients": ["twitter"]` in the character file to connect with X.

### Manually Start Aether

```bash
pnpm i
pnpm build
pnpm start

# The project iterates fast; sometimes you need to clean the project if you are returning to the project
pnpm clean
```

#### Additional Requirements

You may need to install Sharp. If you see an error when starting up, try installing it with the following command:

```
pnpm install --include=optional sharp
```

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=aetheros/aether&type=Date)](https://star-history.com/#aetheros/aether&Date)

