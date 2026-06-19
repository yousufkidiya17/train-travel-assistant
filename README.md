<div align="center">

# ðŸš‚ Train Travel Assistant

### _AI-Powered Indian Railway Companion_

[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-2.0-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![AI Powered](https://img.shields.io/badge/AI-Powered-FF6F61?style=for-the-badge&logo=openai&logoColor=white)](#)
[![Indian Railways](https://img.shields.io/badge/Indian_Railways-IRCTC-FF5722?style=for-the-badge)](#)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:16213e,100:0f3460&height=120&section=header" width="100%"/>

**Train Travel Assistant** is an intelligent chatbot that helps you check **seat availability**, **PNR status**, **live train tracking**, and **fare comparison** for Indian Railways â€” all through a natural conversation interface.

[ðŸ“– **How It Works**](#-how-it-works) Â· [ðŸš€ **Quick Start**](#-quick-start) Â· [ðŸ› **Report Bug**](https://github.com/yousufkidiya17/train-travel-assistant/issues)

</div>

---

## ðŸŽ¯ Overview

> _"Your personal railway assistant â€” just ask in plain English or Hindi."_

Train Travel Assistant combines **real-time web scraping** from Indian Railways with an **AI-powered chat interface** to give you instant answers about trains, seats, fares, and schedules. No more navigating complex IRCTC forms â€” just chat and get answers.

<div align="center">

| ðŸŽ« Seat Availability | ðŸ“ PNR Status | ðŸ—ºï¸ Live Tracking |
|:---:|:---:|:---:|
| Check seats across all classes | Track booking status in real-time | Know exactly where your train is |

| ðŸ’° Fare Comparison | ðŸ“… Schedule Lookup | ðŸ¤– AI Chat |
|:---:|:---:|:---:|
| Compare fares across train types | Full route & timing details | Natural language queries |

</div>

---

## âœ¨ Features

### ðŸ¤– Intelligent Chat Interface
- **Natural language understanding** â€” ask in English or Hindi
- AI-powered **intent detection** for railway queries
- **Context-aware** follow-up conversations
- Smart **fallback** with helpful suggestions

### ðŸ” Real-Time Data Scraping
- Live data from **Indian Railways** official sources
- **Seat availability** across all classes (1A, 2A, 3A, SL, 2S)
- **PNR status** tracking with prediction
- **Route & schedule** information

### ðŸŽ¨ Clean UI Design
- Responsive chat interface
- Train-themed dark aesthetic
- Mobile-first design approach
- Quick-action buttons for common queries

---

## ðŸ—ï¸ Architecture

```
â”Œâ”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”
â”‚               TRAIN TRAVEL ASSISTANT                    â”‚
â”œâ”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”¬â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”¤
â”‚   Frontend      â”‚          Backend                      â”‚
â”‚                 â”‚                                       â”‚
â”‚  Chat UI        â”‚    Flask + Python                     â”‚
â”‚  HTML/CSS/JS    â”‚                                       â”‚
â”‚                 â”‚    â”Œâ”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”                    â”‚
â”‚                 â”‚    â”‚   AI Engine  â”‚ â† Query Parser     â”‚
â”‚                 â”‚    â””â”€â”€â”€â”€â”€â”€â”¬â”€â”€â”€â”€â”€â”€â”€â”˜                    â”‚
â”‚                 â”‚           â”‚                            â”‚
â”‚                 â”‚    â”Œâ”€â”€â”€â”€â”€â”€â–¼â”€â”€â”€â”€â”€â”€â”€â”                    â”‚
â”‚                 â”‚    â”‚  Scraper     â”‚ â† Live Railway Dataâ”‚
â”‚                 â”‚    â””â”€â”€â”€â”€â”€â”€â”¬â”€â”€â”€â”€â”€â”€â”€â”˜                    â”‚
â”‚                 â”‚           â”‚                            â”‚
â”‚                 â”‚    â”Œâ”€â”€â”€â”€â”€â”€â–¼â”€â”€â”€â”€â”€â”€â”€â”                    â”‚
â”‚                 â”‚    â”‚  Formatter   â”‚ â†’ Clean Response    â”‚
â”‚                 â”‚    â””â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”˜                    â”‚
â””â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”´â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”€â”˜
```

---

## ðŸš€ Quick Start

### Prerequisites

- **Python** 3.10+
- **pip** (Python package manager)

### Installation

```bash
# Clone the repository
git clone https://github.com/yousufkidiya17/train-travel-assistant.git
cd train-travel-assistant

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate     # Windows

# Install dependencies
pip install -r requirements.txt

# Run the application
python app.py
```

The app will be running at `http://localhost:5000` ðŸŽ‰

---

## ðŸ“ Project Structure

```
train-travel-assistant/
â”œâ”€â”€ app.py                 # Flask application & routes
â”œâ”€â”€ scraper.py             # Railway data scraping engine
â”œâ”€â”€ test_scraper.py        # Scraper test suite
â”œâ”€â”€ requirements.txt       # Python dependencies
â”œâ”€â”€ THINKER.md             # Design notes & architecture
â”œâ”€â”€ LICENSE                # MIT License
â””â”€â”€ README.md
```

---

## ðŸ› ï¸ Tech Stack

<div align="center">

| Layer | Technology | Purpose |
|-------|-----------|---------|
| **Backend** | Python 3.10, Flask | Web server & API |
| **AI** | LLM Integration | Natural language understanding |
| **Scraping** | BeautifulSoup, Requests | Railway data extraction |
| **Frontend** | HTML, CSS, JavaScript | Chat interface |

</div>

---

## ðŸ—ºï¸ Roadmap

- [x] Core chat interface
- [x] Seat availability scraping
- [x] PNR status lookup
- [x] AI-powered query parsing
- [ ] Live train GPS tracking
- [ ] Fare prediction with ML
- [ ] Multi-language support (Hindi, Tamil, Telugu)
- [ ] Telegram bot integration
- [ ] Push notifications for PNR updates

---

## ðŸ“œ License

Distributed under the **MIT License**. See [`LICENSE`](LICENSE) for more information.

---

## ðŸ‘¨â€ðŸ’» Author

**Yousuf Kidiya**

[![GitHub](https://img.shields.io/badge/GitHub-yousufkidiya17-181717?style=for-the-badge&logo=github)](https://github.com/yousufkidiya17)

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1a1a2e,50:16213e,100:0f3460&height=100&section=footer" width="100%"/>

**Made with ðŸ¤ in India**

_If you found this project useful, please consider giving it a â­!_

</div>
