# Systematic Trading Strategy Development

This repository contains research and implementation of a systematic trading approach for cryptocurrency markets, focusing on Bitcoin orderbook analysis and algorithmic trading.

## Project Overview

This research project explores:
- Orderbook delta analysis for market inefficiency detection
- Statistical validation of trading signals
- Implementation of automated trading infrastructure
- Backtesting framework development

## Key Features

- **Data Collection**: Custom orderbook delta data collection system
- **Signal Generation**: Z-score and IQR-based outlier detection
- **Trend Identification**: Multiple versions of trend detection algorithms
- **Backtesting**: Monte Carlo simulation framework using VectorBT
- **Live Trading**: Asynchronous position management system

## Repository Structure

```
MA/
├── source/          # LaTeX source files and templates
├── imgs/           # Visualization and analysis plots
├── archieve/       # Historical documentation and research
└── build/          # Build artifacts
```

## Technical Details

- **Programming Language**: Python
- **Key Libraries**: VectorBT, Pandas, NumPy
- **Data Storage**: PostgreSQL on Railway.app
- **Exchange Integration**: Coinbase API

## Research Documentation

The main research documentation is available in `notes.pdf`, covering:
- Mathematical foundations
- Statistical analysis
- Strategy development process
- Implementation details
- Backtesting results

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

Special thanks to:
- Dr. Geoffrey Ostrin for supervision
- Various open source projects and research papers cited in the documentation

## Disclaimer

This project is for educational and research purposes only. Trading cryptocurrencies involves substantial risk of loss and is not suitable for every investor.

---
*Note: This is an academic research project. Past performance does not guarantee future results.*
