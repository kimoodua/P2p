<p align="center">
  <img src="cnx.svg" width="120" height="120" alt="P2P Opportunity Monitor Logo"/>
</p>

<h1 align="center">P2P Opportunity Monitor</h1>

<p align="center">
  <strong>Real-time P2P arbitrage dashboard for USDT/UAH across Binance & HTX</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/platform-web-F97316?style=flat-square&logo=googlechrome&logoColor=white" alt="Platform Web"/>
  <img src="https://img.shields.io/badge/language-python-F97316?style=flat-square&logo=python&logoColor=white" alt="Language Python"/>
  <img src="https://img.shields.io/badge/storage-json-F97316?style=flat-square&logo=json&logoColor=white" alt="Storage JSON"/>
  <img src="https://img.shields.io/badge/exchanges-Binance%20%2B%20HTX-F97316?style=flat-square" alt="Exchanges"/>
</p>

<p align="center">
  <a href="https://p2p.0-0.stream/"><strong>🚀 Live Demo →</strong></a>
</p>

---

## Overview

P2P Opportunity Monitor aggregates live P2P ads from Binance and HTX, identifies the best buy/sell spreads, and surfaces actionable arbitrage pairs in a clean real-time dashboard. Designed for speed: filter by payment method, track trusted advertisers, block noise, and act on signals instantly.

---

## Features

| Feature | Description |
|---|---|
| **Live Opportunity Monitor** | Best buy/sell spread, profit estimate (UAH & %), and alert state — updated every 60s |
| **Cross-Exchange Coverage** | Binance and HTX ads aggregated in a single unified view |
| **Favorites Workflow** | Star trusted advertisers to pin them to the top of the list |
| **Blacklist Controls** | Block/unblock advertisers with state persisted to JSON |
| **Payment Filter** | Filter by 20+ Ukrainian payment methods (Monobank, Privat Bank, A-Bank, PUMB, etc.) |
| **Spread Threshold** | Set a minimum spread threshold — only relevant opportunities surface |
| **Profit List** | Ranked view of the top profitable buy/sell pairs at a glance |
| **Alert System** | Toggle audio/visual alerts when a spread opportunity is detected |

---

## Screenshots

<table>
  <tr>
    <td align="center" width="33%">
      <img src="Dashboard.png" width="100%" alt="Main Dashboard"/>
      <br/><sub><b>Main Dashboard — Buy/Sell Board</b></sub>
    </td>
    <td align="center" width="33%">
      <img src="profit_summary.png" width="100%" alt="Top Profitable Opportunities"/>
      <br/><sub><b>Profit List — Top Opportunities</b></sub>
    </td>
    <td align="center" width="33%">
      <img src="Blacklist.png" width="100%" alt="Blocked Advertisers"/>
      <br/><sub><b>Blacklist — Blocked Advertisers</b></sub>
    </td>
  </tr>
</table>

---

## How It Works

```
1. Fetch     →  Pull live P2P ads from Binance & HTX APIs
2. Compute   →  Calculate best spreads and profit estimates per pair
3. Render    →  Display a filterable, real-time dashboard in the browser
4. Persist   →  Save favorites and blacklist to local JSON on every change
```

---

## Quick Start

**Run once** (single fetch, then exit):
```bash
python fetch_binance_p2p_uah_usdt.py --once
```

**Run with auto-refresh** (polls every 60s by default):
```bash
python fetch_binance_p2p_uah_usdt.py
```

Then open `binance_p2p_uah_usdt.html` in your browser, or use the local server URL printed in the terminal.

---

## Dashboard Controls

| Control | Description |
|---|---|
| **Payment** | Filter ads by accepted payment method |
| **Spread Threshold** | Hide pairs below this UAH spread |
| **Amount** | Set your USDT trade size for profit calculations |
| **Refresh** | Manual refresh or auto every 60s |
| **Favorites Only** | Toggle to show only starred advertisers |
| **Alerts** | Enable sound/visual alert on new opportunities |
| **Spread ≥ X** | Quick-filter to highlight high-spread rows |
| **Profit List** | Open ranked top-opportunity panel |
| **Block List** | Manage blocked advertisers |

---

## Tech Stack

<p>
  <img src="https://skillicons.dev/icons?i=python" height="36" alt="Python"/>
  <img src="https://skillicons.dev/icons?i=html" height="36" alt="HTML"/>
  <img src="https://skillicons.dev/icons?i=css" height="36" alt="CSS"/>
  <img src="https://skillicons.dev/icons?i=js" height="36" alt="JavaScript"/>
</p>

- **Python** — data fetching and local server
- **HTML / CSS / JS** — single-file frontend dashboard
- **JSON** — persistent local storage for favorites and blacklist

---

<p align="center">
  <sub>Built for high-signal monitoring · Fast filtering · Persistent preferences</sub>
</p>
