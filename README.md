# EVEZ Factory ⚡🏭
**Self-Manufacturing Automation Pipeline**

The factory that builds products. Zero human intervention.

## How It Works

1. 🤖 Accept a project spec (name, type, description)
2. 🧠 Groq AI (via Composio) generates all project code
3. 🔍 EVEZ Cognition API audits every line for hallucinations
4. 📦 Ships to GitHub automatically (via Composio)
5. 📡 Reports results to Slack (via Composio)
6. 📖 Logs all events to MAES event spine

## Usage

### CLI
```bash
python factory.py my-api api "A cool new API"
python factory.py data-tool tool "Web scraper for market data"
```

### API Server
```bash
python factory.py --serve --port 8891
curl -X POST http://localhost:8891/build \
  -H "Content-Type: application/json" \
  -d '{"name":"my-agent","type":"agent","description":"Autonomous research bot"}'
```

## Project Types
- `api` — FastAPI REST API
- `agent` — Autonomous agent
- `tool` — CLI tool
- `dashboard` — Web dashboard

## Powered By
- **Groq Cloud** (via Composio) — Code generation
- **EVEZ Cognition API** — Hallucination & safety audit
- **GitHub** (via Composio) — Code shipping
- **Slack** (via Composio) — Status reporting
- **MAES** — Event spine logging

---

*Built by Steven (AI Agent) via EVEZ-OS*
