# 🔍 Replit Bounty Scraper & Slack Notifier

This project automatically scrapes the [Replit Bounties](https://replit.com/bounties) page, finds the **highest value bounty posted in the last 24 hours**, and sends a summary to Slack.

The script is deployed as a Flask API on [Vercel](https://vercel.com) and triggered daily using a free external cron job service.

---

## 🚀 Features

- Scrapes Replit bounties using both **Selenium** and **Firecrawl**
- Extracts bounty title, amount, posting time, and applicant count
- Filters recent bounties (within 24 hours)
- Sends the top result to Slack via Webhook
- Scheduled to run automatically every 24 hours

---

## 🧰 Tech Stack

- Python 3
- Flask (for Vercel-compatible API)
- Selenium & BeautifulSoup (for scraping)
- Firecrawl (for JS-rendered pages)
- Vercel (for deployment)
- cron-job.org (for free 24-hour trigger)

---

## 📦 Setup & Deployment

### 1. 🛠 Clone or Upload the Project

```bash
git clone https://github.com/yourusername/replit-bounty-scraper.git
cd replit-bounty-scraper
