# 🚂 Train Travel Assistant

<div align="center">

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.30+-red.svg)](https://streamlit.io/)
[![Playwright](https://img.shields.io/badge/Playwright-1.40+-yellow.svg)](https://playwright.dev/)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)](#)
[![Platform](https://img.shields.io/badge/Platform-Web-brightgreen.svg)](#)
[![Last Updated](https://img.shields.io/badge/Last_Updated-March_2026-orange.svg)](#)

*A powerful train availability checker with AI-powered chat interface for Indian Railways*

</div>

---

## 📋 Table of Contents

- [Features](#features)
- [Quick Start](#quick-start)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Tech Stack](#tech-stack)
- [API Reference](#api-reference)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

---

## ✨ Features

### Core Features

| Feature | Description |
|---------|-------------|
| 🚂 **Train Search** | Search trains between any two stations in India |
| 📅 **Date Selection** | Check availability up to 120 days in advance |
| 🎫 **Seat Availability** | Real-time seat availability status (CNF, WL, Regret) |
| 💺 **Class Information** | View availability for all coach classes (SL, CC, 3E, 3A, 2A, 1A) |
| 💰 **Price Display** | View fare information for each class |
| 📱 **Responsive UI** | Beautiful, mobile-friendly interface |

### Advanced Features

- **AI Chat Interface** - Interact in Hinglish with AI agent
- **Multiple Station Codes** - Support for all major Indian railway stations
- **Popular Routes** - Quick access to commonly searched routes
- **Real-time Scraping** - Live data from ConfirmTkt.com

---

## 🚀 Quick Start

### Prerequisites

- Python 3.11 or higher
- pip or conda package manager

### Installation

```bash
# Clone the repository
git clone https://github.com/yousufkidiya17/train-travel-assistant.git
cd train-travel-assistant

# Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Run the Application

```bash
# Start the Streamlit app
streamlit run app.py
```

The application will open in your default browser at `http://localhost:8501`

---

## 📖 Usage

### Using the Web Interface

1. **Select Source Station** - Choose your departure station from the dropdown
2. **Select Destination Station** - Choose your arrival station
3. **Pick Travel Date** - Select your travel date (up to 120 days ahead)
4. **Click Search** - Click the "Search Trains" button
5. **View Results** - See all available trains with their availability status

### Understanding Status Codes

| Status | Meaning | Icon |
|--------|---------|------|
| **CNF** | Confirmed | ✅ |
| **WL** | Waitlist | ⏳ |
| **Regret** | No seats available | ❌ |
| **Check** | Please check manually | ⚠️ |

---

## 📁 Project Structure

```
train-travel-assistant/
├── app.py                  # Main Streamlit application
├── scraper.py              # Web scraping module
├── test_scraper.py        # Testing module
├── requirements.txt       # Python dependencies
├── output.txt            # Sample output data
├── LICENSE               # MIT License
├── README.md            # This file
└── .gitignore           # Git ignore patterns
```

---

## 🛠 Tech Stack

### Backend

| Technology | Purpose |
|------------|---------|
| **Python 3.11+** | Programming language |
| **Playwright** | Web automation & scraping |
| **asyncio** | Asynchronous operations |

### Frontend

| Technology | Purpose |
|------------|---------|
| **Streamlit** | Web UI framework |
| **Pandas** | Data manipulation |
| **CSS** | Custom styling |

### Data Sources

- **ConfirmTkt.com** - Indian railway booking platform

---

## 🔧 API Reference

### TrainScraper Class

```python
class TrainScraper:
    async def search_trains_async(
        self, 
        from_station: str, 
        to_station: str, 
        date: str
    ) -> dict
```

**Parameters:**
- `from_station` (str): Source station code (e.g., "NDLS")
- `to_station` (str): Destination station code (e.g., "BSB")
- `date` (str): Travel date in DD-MM-YYYY format

**Returns:**
```python
{
    "source": str,
    "destination": str,
    "date": str,
    "trains": [
        {
            "Train No": str,
            "Train Name": str,
            "Status": str
        },
        ...
    ]
}
```

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2026 Yousef Kidiya

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
```

---

## 🙏 Acknowledgments

- [ConfirmTkt](https://www.confirmtkt.com) for the railway data
- [Streamlit](https://streamlit.io) for the amazing UI framework
- [Playwright](https://playwright.dev) for web automation
- All contributors and supporters

---

<div align="center">

**Made with ❤️ by [Yousef Kidiya](https://github.com/yousufkidiya17)**

![Stars](https://img.shields.io/github/stars/yousufkidiya17/train-travel-assistant?style=social)
![Forks](https://img.shields.io/github/forks/yousufkidiya17/train-travel-assistant?style=social)

</div>
