# 🟢 Nbot – Minecraft Server Uptime Bot

**Nbot** is a simple Node.js bot built to keep your **Minecraft server online 24/7** ⛏️.
It works by making sure there’s always a "virtual player" connected, so your server never goes into idle/offline mode. Perfect for free-tier or auto-sleep hosting services where inactivity shuts down the server.

> ⚠️ **Note:** This project has not been updated in over **4 years** and may no longer be fully compatible with the latest **Minecraft** or **Node.js** versions. Use at your own risk.

---

## ✨ Features

* 🟩 Keeps your Minecraft server **running 24/7**
* 👤 Simulates a player being online at all times
* ⚡ Lightweight & easy to set up (just Node.js + config)
* ☁️ Can be deployed locally or to platforms like **Heroku, Railway, Render, etc.**
* 🔧 Customizable via `config.json`

---

## 🛠 Requirements

* [Node.js](https://nodejs.org/) (old versions are safer due to lack of updates)
* npm (comes with Node.js)
* A Minecraft server (Java Edition or compatible hosting service)
* Deployment option: **Heroku** / **Railway** / **Render** / VPS / Local machine

---

## 🚀 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/haddybhaiya/Nbot.git
   cd Nbot
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Edit `config.json` with your Minecraft server details (IP, port, username, etc.).

---

## ⚙️ Configuration

Inside `config.json`, set up values like:

```json
{
  "server_ip": "your.server.ip",
  "server_port": 25565,
  "username": "BotPlayer123"
}
```

* **server\_ip** → Your Minecraft server address
* **server\_port** → Usually `25565` unless changed
* **username** → The bot’s Minecraft username (must be unique)

---

## ▶️ Usage

Start the bot with:

```bash
node index.js
```

Now your bot will connect to your server and keep it alive ✅

### Deploying to Heroku (example)

1. Push your repo to Heroku:

   ```bash
   git push heroku main
   ```

2. The `Procfile` is already included:

   ```
   worker: node index.js
   ```

3. Your bot will run automatically and keep your Minecraft server online 🎉

---

## 📂 Project Structure

| File           | Description                    |
| -------------- | ------------------------------ |
| `index.js`     | Main entry point, bot logic    |
| `config.json`  | Minecraft server settings      |
| `package.json` | Dependencies & scripts         |
| `Procfile`     | Heroku deployment instructions |

---

## ⚠️ Status of This Project

* Last updated: **4+ years ago**
* May not support modern **Minecraft authentication**, **protocols**, or **Node.js versions**
* Still useful as a **reference project** or for running on older setups

---

## 🤝 Contributing

Pull requests are welcome! If you’ve got ideas to improve stability or add features (like multiple-server support, auto-reconnect, or status pings), feel free to fork and submit.

---

## 📜 License

Currently **unlicensed** — feel free to use and modify for personal projects.

---

💡 With **Nbot**, you’ll never worry about your Minecraft server going offline again.
Happy mining & crafting! ⛏️🔥


