
---

## 📄 Strategy Variants

### 1️⃣ Basic Version
- Trades purely based on **first 5-minute candle direction**
- No higher-timeframe bias
- No VWAP filter

**Files**
- `asia_1h_first5m_bais.pine`
- `london_1h_first5m_bais.pine`
- `NY_1h_first5m_bais.pine`

---

### 2️⃣ VWAP Filter Version
Adds **VWAP-based directional confirmation**:

- Long trades → first 5m candle must close **above VWAP**
- Short trades → first 5m candle must close **below VWAP**

This helps filter low-quality trades during choppy conditions.

**Files**
- `asia_1h_first5m_vwap.pine`
- `london_1h_first5m_vwap.pine`
- `ny_1h_first5m_vwap.pine`

---

## 📊 Backtesting Instructions

1. Open **TradingView**
2. Set chart timeframe to **5 minutes**
3. Paste the desired `.pine` script into the Pine Editor
4. Make sure chart timezone is **UTC+5 (Asia/Karachi)** or leave default (script enforces timezone internally)
5. Run Strategy Tester

---

## ⚠️ Important Notes

- These strategies are **for research and educational purposes only**
- Results vary by:
  - Instrument
  - Session volatility
  - Spread & commissions
- Not optimized for live trading without additional risk filters

---

## 🚀 Future Improvements (Planned)

- Unified master strategy with session toggles
- Volatility & range filters
- Daily drawdown limits
- Session-based performance metrics
- Liquidity sweep & HTF bias integration

---

## 📜 License

This project is released under the **MIT License**.  
You are free to use, modify, and distribute with attribution.

---

## 👤 Author

**Basit Ali**

Developed and structured as part of a systematic intraday trading research project.

