# GENUSS Solar & Batteries Landing Page

Official Black Friday promotional landing page for **GENUSS Electronics & Solar Energy Limited** ("*It's Black Friday - Freed From Desire*").

Designed for high conversion, high urgency, and direct WhatsApp sales in the Nigerian solar market.

---

## 🚀 Quick Start

### Option 1: Direct File Opening
Double-click `index.html` in your browser (Google Chrome, Microsoft Edge, Safari, Firefox). All CSS, icons, and interactive scripts work out of the box with zero installation required!

### Option 2: Local HTTP Server (Recommended)
Run the lightweight built-in Node server:
```bash
node server.js
```
Then open:
👉 **[http://localhost:8080](http://localhost:8080)**

---

## ✨ Features & Architecture

1. **High-Converting Ad Overlay Modal**:
   - Matches Black Friday 1:1 / 4:5 social media banner aesthetics.
   - Showcases the featured Eastman 220Ah starter combo with a direct call to action.
   - Dismissible via button, background click, or `Esc` key.

2. **Official Reassurance & Trust Bar**:
   - Free delivery across Lagos & Ibadan.
   - 90-day return & replacement support.
   - 100% secure payment guarantees.
   - 24/7 dedicated solar support.

3. **Hero Section with Dynamic Ticker**:
   - Bold typography with gold gradient highlights.
   - Rotating live deal spotlight ticker.
   - Featured bundle spotlight card with product breakdown.

4. **Rotating Flash Deals Banner**:
   - Active countdown timer (`04:00:00`).
   - "Claimed: 84% — Only 3 units left" urgency progress bar.
   - Deal switcher with previous/next controls.

5. **Generator Fuel vs Solar ROI Calculator**:
   - Interactive slider from ₦30,000/mo to ₦600,000/mo.
   - Calculates 1-year and 3-year fuel waste, daily generator runtime, and solar payback timeline (~8 - 14 months).

6. **Tiered Product Catalog**:
   - **Starter (Budget / Basic)**: 1kVA - 1.5kVA systems for apartments and essential appliances.
   - **Standard (Middle Class)**: 5kVA hybrid systems with lithium batteries for homes and offices with ACs and freezers.
   - **Luxury & Enterprise**: 12kW - 20kW heavy-duty microgrids for duplexes, mansions, clinics, and factories.
   - **Batteries Only**: 220Ah tall tubular batteries and 10kWh wall-mounted LiFePO4 packs.
   - Integrated search across product names, specifications, descriptions, and powered appliances.

7. **Interactive Power Load Estimator (System Sizer)**:
   - 10 common appliances with quantity increment/decrement (`-` `[count]` `+`).
   - Live continuous wattage calculation.
   - Tailored tier recommendation with auto-scroll and highlight animation.

8. **Product Detail Modal**:
   - Full component specifications and appliance capabilities.
   - Rating stars with verified buyer feedback.
   - Direct pre-formatted WhatsApp order buttons.

9. **Installation Assessment & Quote Modal**:
   - Lead capture form for customer name, phone/WhatsApp, state/city, and appliance details.

10. **Frequently Asked Questions (FAQ)**:
    - Expandable accordion addressing delivery, warranties, payment, and installation.

11. **Social Proof & Urgency**:
    - Floating WhatsApp button with pulsing live status indicator.
    - Subtle recent purchase toast alerts (Lekki, Ibadan, VI, Abuja).

---

## 🛠️ Configuration & Customization

### Updating WhatsApp Operator Number
To change the receiving WhatsApp phone number, edit `WHATSAPP_OPERATOR_NUMBER` in `index.html`:
```javascript
const WHATSAPP_OPERATOR_NUMBER = '2348033057945'; // Format: CountryCode + Number (without + or 0)
```

### Adding or Modifying Products
Edit the `products` array inside `index.html` (lines ~825). Each item contains:
- `id`: Unique identifier
- `name`: Display title
- `tier`: `'starter'`, `'mid'`, `'luxury'`, or `'batteries'`
- `price`: Sale price in Naira
- `originalPrice`: Pre-sale price in Naira
- `badge`: Display tag
- `powers`: Array of appliances powered
- `specs`: Array of included hardware components
- `deliveryNote`: Delivery badge text
- `imageType`: `'starter'`, `'luxury'`, `'inverter'`, `'battery'`, or `'lithium_mid'`
- `reviews`: Array of customer reviews

---

## 📁 Project Structure

```
GENUSS/
├── index.html                           # Primary production-ready landing page
├── genuss_black_friday_platform_ad.html  # Synchronized landing page source
├── server.js                            # Zero-dependency local Node.js HTTP server
├── package.json                         # Project metadata and start scripts
├── README.md                            # Documentation and usage guide
├── assets/
│   ├── top-seller-starter.png           # Eastman 220Ah Combo visual
│   └── top-seller-luxury.png            # DEYE 12kW System visual
└── .vscode/
    └── launch.json                      # VS Code debugging and browser launch config
```

