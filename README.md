# 🎯 MT5 Trade Panel Expert Advisor

<div align="center">

**Professional Trading Panel with Advanced Position Management for MetaTrader 5**

![MT5](https://img.shields.io/badge/Platform-MetaTrader%205-blue)
![Version](https://img.shields.io/badge/Version-2.0-success)
![License](https://img.shields.io/badge/License-Commercial-red)

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Contact](#-contact)

</div>

---

## 📋 Overview

**MT5 Trade Panel EA** is a sophisticated Expert Advisor designed for professional traders who need precise control over their trading operations. This EA provides an intuitive visual panel interface with advanced features including automatic trade management, basket-based profit protection, and comprehensive position control.

Perfect for:
- ✅ Prop firm traders
- ✅ Professional day traders
- ✅ Multi-position strategy traders
- ✅ Traders requiring precise risk management

---

## 📸 Screenshots

https://raw.githubusercontent.com/kaleemullahkhan786/MT5-Trade-Panel-Expert-Advisor/main/TradePanel.jpg

---

## ✨ Features

### 🎮 **Interactive Trading Panel**
- **Drag-and-drop interface** - Move the panel anywhere on your chart
- **Real-time input fields** - Edit parameters directly from the chart
- **Visual feedback** - Clear button states and color-coded controls
- **Responsive design** - Works seamlessly across different screen resolutions

### 📊 **Main Trade Management**
- **Risk-based lot calculation** - Automatically calculates lot sizes based on risk percentage or fixed money amount
- **Flexible Risk/Reward ratios** - Set custom R:R for precise profit targets
- **One-click trading** - Instant Buy/Sell execution with pre-configured parameters

### 🔄 **Auto-Add Trades System**
- **Distance-based additions** - Automatically add trades at fixed distance (in points) from last opened position
- **Directional consistency** - Added trades follow the initial trade direction (BUY/SELL)
- **Custom lot sizing** - Set fixed lot size or use risk-based calculation for added trades
- **Smart tracking** - References last opened trade, not just open positions
- **Duplicate prevention** - Avoids multiple entries at the same price level

### 🛡️ **Stop Loss Inheritance**
- **Automatic SL copying** - All auto-added trades inherit Stop Loss from the initial trade
- **Prop firm compliant** - Meets strict requirements for professional trading firms
- **No Take Profit for added trades** - Maintains strategy consistency

### 💰 **Basket Break-Even System**
- **Total PnL monitoring** - Continuously tracks combined profit/loss of all open positions
- **Automatic position closure** - Closes all positions when total PnL reaches threshold
- **Customizable threshold** - Set your desired profit target amount
- **Multi-trade support** - Works with any number of open positions
- **Direction independent** - Functions correctly for both BUY and SELL trades

### 🎯 **Global Stop Loss Management**
- **Visual SL setting** - Click and drag on chart to set global Stop Loss
- **Universal application** - Applies to all open positions simultaneously
- **Revert capability** - Restore original Stop Loss values when needed

### 🔒 **Position Management**
- **One-click close all** - Instantly close all positions on current symbol
- **Safe execution** - Proper MT5 trade execution with error handling
- **Partial close support** - Handles partial fills correctly

---

## 🖼️ Interface Overview

### Panel Sections

1. **Main Trade Configuration**
   - Risk input (percentage or fixed amount)
   - Risk/Reward ratio setting
   
2. **Add Trades Configuration**
   - Lot size for auto-added trades
   - Gap distance (in points) between added trades

3. **Global Stop Loss**
   - Input field for price level
   - Interactive "Set Global SL" button

4. **Basket Break-Even**
   - Profit threshold amount
   - Enable/Disable toggle button

5. **Trade Execution**
   - Buy button (blue)
   - Sell button (red)
   - Close All button

---

## 🚀 Key Capabilities

### ⚙️ **Automatic Trade Adding Logic**
```
- Monitors price movement continuously
- Adds new position when price moves beyond last opened trade by specified gap
- Maintains same direction as initial trade
- Inherits Stop Loss automatically
- No Take Profit on added trades (prop firm compliance)
```

### 💎 **Basket Break-Even Protection**
```
- Calculates total floating PnL across all positions
- Closes all positions automatically when threshold reached
- Works regardless of number of trades or direction
- Can be enabled/disabled via toggle button
- Real-time monitoring on every tick
```

### 🎛️ **Flexible Configuration**
- All settings managed through visual panel (no hardcoded values)
- Real-time updates - changes apply immediately
- Settings persist across chart restarts
- No input parameters required - fully panel-controlled

---

## 📦 Technical Specifications

### **Requirements**
- MetaTrader 5 (Build 3815 or higher)
- Windows or Mac OS
- Live/Demo trading account

### **Features**
- ✅ CTrade library integration
- ✅ Proper error handling
- ✅ No infinite loops
- ✅ CPU-efficient code
- ✅ Production-ready for live trading
- ✅ Prop firm compliant
- ✅ Memory-efficient position tracking

### **Code Quality**
- Clean, well-structured code
- Comprehensive error checking
- Safe position modification
- Proper MT5 syntax (no MT4 compatibility)
- Compiles without warnings

---

## 💼 Use Cases

### **1. Scaling In Strategies**
Add positions as price moves in your favor, with automatic SL inheritance ensuring consistent risk management across all positions.

### **2. Grid Trading**
Automatically add trades at fixed intervals, perfect for grid-based strategies with precise distance control.

### **3. Profit Protection**
Set a total PnL threshold and let the EA automatically close all positions when your profit target is reached.

### **4. Risk Management**
Use risk-based lot calculation to maintain consistent risk per trade regardless of stop loss distance.

---

## 🎯 Advantages

| Feature | Benefit |
|---------|---------|
| **Visual Panel** | No need to open EA settings - everything accessible on chart |
| **Real-time Control** | Modify parameters instantly without EA restart |
| **Basket Management** | Protect total account equity, not just individual trades |
| **Auto-Add Logic** | Automate position scaling without constant monitoring |
| **Prop Firm Ready** | Meets strict requirements for professional trading firms |
| **Error Handling** | Graceful handling of edge cases and broker restrictions |

---

## 🔧 Configuration Guide

### **Initial Setup**
1. Attach EA to your trading chart
2. Panel appears automatically on the chart
3. Configure risk parameters
4. Set basket break-even threshold (optional)
5. Enable auto-add trades if needed

### **Using Auto-Add Trades**
1. Set "Gap" value (distance in points)
2. Set "Lots" size for added trades
3. Open initial position using Buy/Sell button
4. EA automatically adds trades when price moves beyond threshold

### **Using Basket Break-Even**
1. Enter profit threshold in "Basket BE" field (e.g., 100.00)
2. Click "BreakEven" button to enable (turns green when active)
3. EA monitors total PnL continuously
4. All positions close automatically when threshold reached

---

## ⚠️ Important Notes

- **Demo Test First**: Always test on demo account before live trading
- **Risk Management**: Set appropriate risk percentages based on your strategy
- **Broker Requirements**: Ensure your broker supports all required features
- **Minimum Distance**: Respect broker's minimum stop level requirements
- **Account Type**: Works with both Standard and ECN account types

---

## 📞 Contact & Purchase

<div align="center">

### 🛒 **Interested in this EA?**

**This is a premium Expert Advisor available for purchase.**

For inquiries, pricing, and purchase information, please contact:

📧 **Email**: kaleemullahkhan.contact@gmail.com
💬 **Whatsapp**: +92 3147121270 

**Custom modifications and additional features available upon request.**

---

### 📄 License

This software is proprietary and confidential. Unauthorized copying, distribution, or modification is strictly prohibited.

© 2024 All Rights Reserved

</div>

---

## 🙏 Acknowledgments

Built with precision for professional traders who demand reliability, flexibility, and advanced position management capabilities.

---

<div align="center">

**Made with ❤️ for Professional Traders**

*Trusted by traders worldwide for reliable trading automation*

</div>
