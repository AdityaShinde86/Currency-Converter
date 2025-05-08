# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

A responsive and user-friendly Currency Converter built with React, JavaScript, and REST APIs, allowing users to convert between different currencies using real-time exchange rates.

Features
Real-Time Exchange Rates: Fetches up-to-date currency conversion rates using a free REST API.

Intuitive UI: Clean and responsive design with a seamless user experience.

Custom React Hook: Encapsulates API fetching logic for reusability and maintainability.

Dynamic Currency Selection: Supports multiple currencies with dropdown selectors.

Swap Functionality: Quickly switch between source and target currencies.

Error Handling: Displays user-friendly error messages for API failures.

Technologies Used
Frontend: React, JavaScript, HTML, CSS

API: ExchangeRate-API (or any free currency API)

State Management: React Hooks (useState, useEffect, custom hooks)

Styling: CSS (Flexbox/Grid for responsive layouts)

How It Works
User Input:

Select the source currency (e.g., USD).

Enter the amount to convert.

Choose the target currency (e.g., EUR).

API Fetching:

A custom React hook (useCurrencyConverter) fetches real-time exchange rates.

The app dynamically updates the converted amount.

Result Display:

Shows the converted value instantly.

Provides a swap button to reverse currencies quickly.

Code Structure
plaintext
currency-converter/
├── src/
│   ├── components/
│   │   ├── CurrencyInput.js  # Handles currency selection & amount input
│   │   ├── SwapButton.js     # Swaps source & target currencies
│   │   └── ResultDisplay.js  # Shows converted amount
│   ├── hooks/
│   │   └── useCurrencyConverter.js  # Custom hook for API fetching
│   ├── App.js                # Main component
│   ├── index.js              # React entry point
│   └── styles.css            # Global styling
├── public/
│   └── index.html            # HTML template
└── package.json              # Project dependencies
Setup & Installation
Clone the repository:

bash
git clone https://github.com/yourusername/currency-converter.git
cd currency-converter
Install dependencies:

bash
npm install
Run the app:

bash
npm start
Open http://localhost:3000 to view it in your browser.

API Key Setup
To fetch real-time exchange rates, sign up for a free API key from ExchangeRate-API and replace the placeholder in the custom hook:

javascript
// Inside useCurrencyConverter.js
const API_KEY = "YOUR_API_KEY";  
const API_URL = `https://v6.exchangerate-api.com/v6/${API_KEY}/latest/USD`;
Future Enhancements
Historical Data: Add a feature to check past exchange rates.

Currency Charts: Integrate charts for trend analysis.

Offline Mode: Cache rates for limited offline functionality.

Multi-currency Comparison: Compare multiple currencies at once.
