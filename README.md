# 🌤️ Klimate Weather Dashboard
A modern React weather application featuring real-time weather data, hourly/daily forecasts, location search with geolocation support, favorite cities management, and responsive design with dark/light theme support.

![React](https://img.shields.io/badge/React-19.1.1-blue?style=flat-square&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.8.3-blue?style=flat-square&logo=typescript)
![Vite](https://img.shields.io/badge/Vite-7.1.4-purple?style=flat-square&logo=vite)
![TanStack Query](https://img.shields.io/badge/TanStack%20Query-5.87.1-red?style=flat-square)

## 🚀 Live Demo
- **Application**: [https://klimate-weld-tau.vercel.app/](https://klimate-weld-tau.vercel.app/)

## 📋 Table of Contents
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [API Documentation](#-api-documentation)
- [Project Structure](#-project-structure)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

## ✨ Features
- 🌡️ **Real-time Weather Data** - Current temperature, humidity, wind speed, and conditions
- 📊 **Interactive Charts** - Hourly temperature trends using Recharts
- 🔍 **Smart Search** - City search with autocomplete and search history
- 📍 **Geolocation Support** - Automatic location detection
- ⭐ **Favorites Management** - Save and manage favorite cities
- 📱 **Responsive Design** - Works seamlessly on desktop and mobile devices
- 🌓 **Theme Support** - Light and dark mode toggle
- ⚡ **Fast & Reliable** - Built with modern React and optimized queries

## 🛠 Tech Stack
### Frontend
- **Framework**: React 19.1.1 with Vite
- **Language**: TypeScript 5.8.3
- **Styling**: Tailwind CSS 4.1.13
- **UI Components**: shadcn/ui with Radix UI
- **State Management**: TanStack Query 5.87.1
- **Charts**: Recharts 3.2.1
- **Icons**: Lucide React
- **Routing**: React Router DOM 7.8.2
- **Deployment**: Vercel

### API & Services  
- **Weather API**: OpenWeatherMap API
- **Geolocation**: Browser Geolocation API
- **HTTP Client**: Fetch API with TanStack Query

### Development Tools
- **Build Tool**: Vite 7.1.4
- **Linter**: ESLint 9.35.0
- **Package Manager**: pnpm

## 📦 Installation
### Prerequisites
- Node.js 18.20 or higher
- pnpm (recommended) or npm
- OpenWeatherMap API key

### Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yats1304/klimate.git
    cd klimate

2. Install dependencies:
    ```bash
    pnpm install


3. Set up environment variables:
    ```bash
    VITE_OPENWEATHER_API_KEY=your_api_key_here

    Get your free API key from [OpenWeatherMap](https://openweathermap.org/api)

4. Run the project:
    ```bash
    pnpm dev

5. Open your browser:
    ```bash
    Navigate to `http://localhost:5173`

## 🎯 Usage
- **Location Access**: Allow location access for automatic weather detection
- **Search Cities**: Use the search bar to find weather for any city worldwide
- **Add Favorites**: Click the star icon to save cities to your favorites list
- **View Forecasts**: Scroll to see interactive hourly temperature charts
- **Theme Toggle**: Switch between light and dark modes using the theme toggle
- **Responsive Design**: Access from any device with optimized mobile experience

## 🌐 API Documentation
This app integrates with OpenWeatherMap API endpoints:
- **Current Weather**: `/data/2.5/weather` - Real-time weather conditions
- **5-Day Forecast**: `/data/2.5/forecast` - Hourly forecasts for 5 days
- **Geocoding**: `/geo/1.0/direct` - City search and coordinates
- **Reverse Geocoding**: `/geo/1.0/reverse` - Location names from coordinates

## 📁 Project Structure
```
klimate/
├── public/
│ ├── vite.svg
│ └── index.html
├── src/
│ ├── api/
│ │ ├── config.ts               # API configuration
│ │ ├── types.ts                # TypeScript interfaces
│ │ └── weather.ts              # Weather API service
│ ├── components/
│ │ ├── ui/ # shadcn/ui components
│ │ │ ├── button.tsx
│ │ │ ├── alert.tsx
│ │ │ ├── command.tsx
│ │ │ ├── scroll-area.tsx
│ │ │ └── sonner.tsx
│ │ ├── city-search.tsx          # City search component
│ │ ├── favourite-cities.tsx     # Favorite cities management
│ │ ├── weather-dashboard.tsx    # Main dashboard
│ │ ├── header.tsx # App header
│ │ └── loading-skeleton.tsx # Loading states
│ ├── hooks/
│ │ ├── use-geolocation.ts      # Geolocation hook
│ │ ├── use-waether.ts          # Weather query hooks
│ │ ├── use-search-history.ts   # Search history hook
│ │ ├── use-favourite.ts        # Favorites management
│ │ └── use-local-storage.ts    # Local storage hook
│ ├── pages/
│ │ ├── weather-dashboard.tsx
│ │ └── city-page.tsx
│ ├── lib/
│ │ └── utils.ts                # Utility functions
│ ├── styles/
│ │ └── globals.css # Global styles
│ ├── App.tsx                   # Main App component
│ ├── main.tsx # Entry point
│ └── vite-env.d.ts             # Vite type definitions
├── .env # Environment variables
├── .gitignore                  # Git ignore rules
├── eslint.config.js            # ESLint configuration
├── index.html                  # HTML template
├── package.json                # Dependencies and scripts
├── pnpm-lock.yaml              # Package lock file
├── postcss.config.js           # PostCSS configuration
├── tailwind.config.js          # Tailwind CSS configuration
├── tsconfig.json               # TypeScript configuration
├── vite.config.ts              # Vite configuration
└── README.md                   # Project documentation
```

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Contact
**Yatish Shashikant Chaubal**
- GitHub: [@yats1304](https://github.com/yats1304)
- LinkedIn: [Yatish Chaubal](https://linkedin.com/in/yatish-chaubal)
- Email: yatishchaubal1304@gmail.com
- Mobile: +91 8551994340

## 🙏 Acknowledgments
- [OpenWeatherMap](https://openweathermap.org/) for comprehensive weather data
- [shadcn/ui](https://ui.shadcn.com/) for beautiful UI components
- [Recharts](https://recharts.org/) for interactive weather charts
- [TanStack Query](https://tanstack.com/query) for efficient data fetching
- [Lucide](https://lucide.dev/) for modern icons

---

<div align="center">
  Made with ❤️ and ☀️ by Yatish Chaubal
</div>
