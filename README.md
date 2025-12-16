# 🎬 Cinema Aggregator Backend

This project aggregates movie showtimes from multiple cinema providers in Cambodia:
- Legend Cinema
- Major Cineplex
- Prime Cineplex

Showtime data is scraped, normalized into a unified structure, stored in a database, and exposed via a FastAPI API for frontend consumption.

---

## 📁 Project Structure

cinemesh-cinema/
├── scraper/
│ ├── legend_scraper.py
│ ├── major_scraper.py
│ ├── prime_scraper.py
│
├── crud.py
├── database.py
├── models.py
├── schemas.py
├── seed_from_json.py
├── python_run_all.py
├── main.py
├── requirements.txt
├── README.md
├── .gitignore


---

## 🚀 Features

- Scrapes showtimes from:
  - **Legend Cinema** (Playwright)
  - **Major Cineplex** (HTTP API)
  - **Prime Cineplex** (Selenium)
- Normalizes all providers into a unified data model
- Stores data using SQLAlchemy
- FastAPI backend for querying showtimes by movie title
- Frontend-friendly API (filtering and pagination handled client-side)

---

## 🧱 Tech Stack

- Python 3.10+
- FastAPI
- SQLAlchemy
- Playwright
- Selenium
- Requests
- SQLite (default database)

---

## 📦 Installation

### 1. Create a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate

2. Install dependencies

pip install -r requirements.txt

3. Install Playwright Browser

playwright install