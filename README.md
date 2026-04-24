# 🌾 AAPLA 7/12 - Digital Agriculture Mission 2024
> *Empowering Indian farmers with real-time market data, AI-driven crop insights, and a supportive community in their native language.*

[![React](https://img.shields.io/badge/React-18-blue.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue.svg)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5.0-purple.svg)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.0-cyan.svg)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

AAPLA 7/12 is a comprehensive **Progressive Web App (PWA)** designed to revolutionize how farmers interact with agricultural data. It combines traditional farming practices with modern technology, providing actionable advice, live market rates, and community support in multiple regional languages.

## ✨ Key Features

### 🌍 100% Multilingual Interface
- Fully translated UI supporting **English, Hindi (हिंदी), and Marathi (मराठी)**.
- Language switcher instantly localizes the entire application (navigation, content, alerts, and placeholders) via `i18next`.

### 📈 Live Mandi Prices (Govt. API Integration)
- Integrated directly with the official **data.gov.in (Agmarknet)** API.
- Real-time commodity prices from APMCs across India (Maharashtra, Gujarat, MP, etc.).
- Filterable by state and categorized dynamically (Cereals, Pulses, Vegetables, Fruits, Oilseeds, Spices).
- Auto-calculates "Top Gainers" and "Top Losers" based on market trends.

### 👥 Interactive Farmer Community
- Social feed for farmers to share success stories, ask for advice, and connect.
- Post creation, dynamic "Likes", local state management, and localized verified badges (e.g., KVK Officials).

### 🩺 AI Disease Detection & Soil Health
- **Disease Scanner:** Upload leaf photos to get instant AI-simulated disease diagnostics (Early Blight, Leaf Rust, etc.) with confidence scores and treatment plans.
- **Soil Health Card:** Track Nitrogen, Phosphorus, Potassium, and pH levels to generate personalized crop advisories.

### 💧 Smart Irrigation Advisory
- Real-time, time-of-day based water management advice.
- Farm size water calculator based on specific crop needs (Wheat, Rice, Sugarcane).

### 📱 Progressive Web App (PWA)
- Installable on Android/iOS devices for a native app-like experience.
- Service workers enable faster load times and offline fallback capabilities.

## 🛠️ Technology Stack

- **Frontend Framework**: React 18, TypeScript, Vite
- **Styling**: Tailwind CSS, Shadcn UI (Radix Primitives)
- **Icons**: Lucide React
- **State & Routing**: React Router DOM, React Context API
- **Internationalization**: `i18next`, `react-i18next`
- **Authentication**: Firebase Auth (Google OAuth & Email/Password)
- **Data Integration**: Official `data.gov.in` REST API

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- Firebase Project Credentials
- data.gov.in API Key (for live Mandi prices)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/piyush-nirmal/Aapla-7-12.git
   cd Aapla-7-12
   ```

2. **Install Dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory and add your keys:
   ```env
   VITE_FIREBASE_API_KEY=your_firebase_api_key
   VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
   VITE_FIREBASE_PROJECT_ID=your_project_id
   ```
   *(Note: The `data.gov.in` API key is currently managed in `src/services/mandiService.ts` for simplicity, but should be moved to `.env` for production).*

4. **Run Development Server**
   ```bash
   npm run dev
   ```

## 📂 Project Structure Highlights
- `/src/i18n/locales` - Contains comprehensive language dictionaries (`en.ts`, `hi.ts`, `mr.ts`).
- `/src/services` - Contains API integration logic (e.g., `mandiService.ts`).
- `/src/pages` - Standalone page components (Dashboard, Market, Soil, Disease, Community).
- `/src/components/ui` - Reusable Shadcn UI components.

## 🤝 Contributing
Contributions are always welcome! 
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---
<div align="center">
  <b>Built with ❤️ for Indian Farmers.</b>
</div>
