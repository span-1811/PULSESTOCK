# PulseStock — Indian Stock Market AI Analyzer v2.0
Live NSE/BSE data + Gemini AI predictions. Indian stocks only.

---

## SETUP (2 minutes)

### 1. Install Node.js dependencies
```bash
npm install
```

### 2. Start the server
```bash
node server.js
```

### 3. Open in browser
```
http://localhost:3000
```

---

## WHAT'S FIXED

| Problem | Fix |
|---------|-----|
| Demo/fake data | Live NSE prices via Yahoo Finance through backend |
| Enter ticker symbol only | Search by full company name (e.g. "Reliance", "HDFC Bank") |
| US stocks mixed in | 100% Indian market — NSE/BSE only |
| CORS errors in browser | All API calls go through Node server (no CORS issues) |
| Broken charts | Proper Chart.js with real OHLCV history from NSE |
| No OHLCV data | Open, High, Low, Volume, Market Cap shown on detail page |

---

## FEATURES

- **Live NSE prices** — Reliance, TCS, HDFC Bank, Infosys, Zomato and 60+ stocks
- **Company name search** — Type "Reliance" or "Tata" — no need to know ticker codes
- **Live Index Bar** — NIFTY 50, SENSEX, BANK NIFTY on homepage
- **Live ticker** — Top NSE stocks scrolling in real time
- **SMA Analysis** — 7-day vs 30-day moving averages
- **Gemini AI Signal** — Bullish/Bearish/Neutral with confidence %
- **OHLCV Row** — Open, High, Low, Volume, Market Cap per stock
- **Watchlist** — Saved in localStorage with live price updates
- **Top Movers** — Gainers, Losers, Volume leaders from Nifty 50

---

## GEMINI AI KEY

Your key is already embedded in `public/index.html`:
```javascript
const GEMINI_KEY = 'AIzaSyDmOxo7oXalZJxyH0NKhfdKTSNnj1v4MHs';
```
Get a free key at: https://aistudio.google.com

---

## NODE VERSION

Requires Node.js 18+ (for built-in fetch).
Check: `node --version`

If older Node: `npm install node-fetch` and the server will auto-use it.
