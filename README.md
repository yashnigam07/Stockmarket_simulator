# TradePulse 2049

A futuristic stock and crypto trading simulator built with HTML, CSS, and JavaScript. Powered by real-time data from Alpha Vantage, TradePulse 2049 lets you trade stocks (AAPL, GOOGL, TSLA) and cryptocurrencies (BTC, ETH) with advanced features like limit orders, short selling, and portfolio analytics—all in a sleek, customizable UI.

**[Live Demo](https://yashnigam07.github.io/Stockmarket_simulator/)**

## Features

- **Real-Time Data:** Fetches live prices via Alpha Vantage API (falls back to simulation after rate limits).
- **Trading Options:** Market, limit, stop-loss, take-profit, short selling, and OCO orders.
- **Portfolio Tracking:** Monitor cash, stock holdings, total value, and profit/loss.
- **Charts:** Interactive price history, EMA, RSI, Bollinger Bands, and portfolio allocation visuals using Chart.js.
- **Sentiment & Analytics:** Vote on bullish/bearish sentiment, view Sharpe Ratio, Beta, and volatility.
- **Themes:** Light, Dusk, Morning, Dark, and System Default modes.
- **Extras:** Holo-dashboard toggle, sound effects, undo trades, export/import portfolio, and AI trend prediction.

## Screenshots

![TradePulse 2049 Interface](SS.png)  
*Caption: Main simulator interface with live price chart and trading panel.*

## Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Edge, etc.).
- An [Alpha Vantage API key](https://www.alphavantage.co/support/#api-key) (free tier available).

### Installation
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yashnigam07/Stockmarket_simulator.git
   cd Stockmarket_simulator
   ```

2. **Set Up API Key:**
   - Open `index.html` and ensure the `API_KEY` constant is set:
     ```javascript
     const API_KEY = "VINMFIYFJ1P087M1"; // Replace with your Alpha Vantage API key
     ```

3. **Run Locally:**
   - Use a local server to avoid CORS issues:
     ```bash
     python -m http.server 8000
     ```
   - Open `http://localhost:8000` in your browser.

4. **Deploy (Optional):**
   - Push to GitHub Pages or another static hosting service. Ensure API calls work over HTTPS.

## Usage
1. Select a stock or crypto from the dropdown (e.g., AAPL, BTC).
2. Use the trading panel to buy/sell with customizable order types.
3. Monitor your portfolio, view charts, and adjust settings via the header controls.
4. Explore advanced features like sentiment voting, news, and AI predictions.

## Project Structure
```
Stockmarket_simulator/
├── index.html       # Main file with HTML, CSS, and JS
├── SS.png           # Screenshot of the simulator
├── README.md        # This file
└── (Optional assets) # Add more screenshots or sound files if needed
```

## Dependencies
- [GSAP](https://greensock.com/gsap/) - Animations
- [Chart.js](https://www.chartjs.org/) - Charts
- [Font Awesome](https://fontawesome.com/) - Icons (embedded subset)
- [Google Fonts](https://fonts.google.com/) - Poppins & Orbitron

## Limitations
- Alpha Vantage free tier limits: 5 API calls/minute, 500/day. Simulation kicks in after limits.
- GitHub Pages may block API calls due to CORS unless configured properly.
- Single-file structure; split into separate files for larger-scale development.

## Contributing
1. Fork the repo.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit changes (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-name`).
5. Open a Pull Request.

## License
© 2025 Yash Nigam. Licensed under the [MIT License](LICENSE).

## Acknowledgments
- Built by [yashnigam07](https://github.com/yashnigam07).
- Powered by [Alpha Vantage](https://www.alphavantage.co/).
- Inspired by futuristic trading platforms.

