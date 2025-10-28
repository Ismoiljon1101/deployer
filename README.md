
# 🚀 Auto Deploy with GitHub Webhook + PM2

> Free and simple self-hosted deployment system — whenever you push to **master**, your server automatically pulls the latest code, builds it, and restarts with **PM2**.
> No CI/CD bloat, no manual SSH, no clicks. Just push → deploy → done.

---

## ⚙️ Features

- 🔁 **Automatic Deployment** — trigger deploys from any `master` push.
- 🔒 **Secure Webhook** — only responds to valid GitHub events.
- 🧠 **Self-Contained** — runs on your own server (works great on Raspberry Pi, VPS, or cloud instance).
- 🕹️ **Daemonized with PM2** — keeps your app + webhook alive 24/7.
- 🧰 **Fully Customizable** — edit scripts for your stack (Node, Python, Go, etc).

---

## 🧩 How It Works

1. Push code to the `master` branch on GitHub.
2. GitHub sends a webhook to your server.
3. The server runs `deploy.sh`:
   - Pulls latest code
   - Installs dependencies
   - Builds project
   - Restarts app via PM2
4. Logs everything to `/var/log/deploy.log`.

---

## 🧱 Setup Guide

### 1. Clone this repo on your server

```bash
https://github.com/Ismoiljon1101/deployer
```
