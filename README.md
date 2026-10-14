# ClawShield · AI Hedge Fund Dashboard

## Setup

```bash
# 1. Install Python deps
pip install -r requirements.txt

# 2. Start the backend
cd backend
uvicorn main:app --reload --port 8000

# 3. Open the frontend
# Open frontend/index.html in Chrome/Edge (no server needed)
```

## Architecture

```
frontend/index.html          ← Single-file 3D dashboard (Three.js)
backend/main.py              ← FastAPI + AKShare + EDGAR endpoints
requirements.txt
```

## Data Sources

| Source   | What it provides                              | Endpoint         |
|----------|-----------------------------------------------|------------------|
| AKShare  | OHLCV, US stock daily prices                  | /api/quote/:t    |
| EDGAR    | 10-K fundamentals (revenue, EPS, ROE)         | /api/fundamentals/:t |
| Mock     | Seeded fallback when APIs unavailable         | automatic        |

## API Endpoints

| Method | Route                 | Description                        |
|--------|-----------------------|------------------------------------|
| GET    | /api/quote/:ticker    | Live OHLCV + technicals (RSI, MACD)|
| GET    | /api/fundamentals/:t  | EDGAR 10-K fundamentals            |
| GET    | /api/agents/:ticker   | 18-agent swarm signals             |
| GET    | /api/graph/:ticker    | DAG topology for 3D graph          |
| GET    | /api/surface/:ticker  | Price-vol surface grid data        |
| GET    | /api/hashmap/:ticker  | ArmorClaw policy hash map          |
| POST   | /api/verify           | ArmorClaw intent verification      |
| GET    | /api/search?q=        | Ticker search (500+ symbols)       |

## Frontend Panels

1. **Dashboard** — Live quote, 18-agent signals grid, consensus score
2. **3D Agent Graph** — Force-directed DAG with all 18 agents + data sources
3. **Price Surface** — 3D mesh of price × volatility window over 90 days
4. **Hash Map** — ArmorClaw policy rule bucket visualiser + interactive hasher
5. **Verification** — Full ArmorClaw pipeline execution with rule-by-rule animation

## Offline Mode

The frontend works fully offline with deterministic seeded mock data.
When backend is running, it switches to live AKShare/EDGAR automatically.
