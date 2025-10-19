# ☕ Cafe Finder

A simple, modern, and elegant web app for finding and saving your favorite cafes, built with Vanilla JS.

![Vanilla JS](https://img.shields.io/badge/Vanilla%20JS-ES6+-yellow?style=flat-square)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

## ✨ Features

-   **Interactive Swipe Interface**: Tinder-style card swiping powered by [Hammer.js](http://hammerjs.github.io/).
-   **Local Storage**: Save your favorite cafes and access them anytime.
-   **Clean & Modern UI**: A minimalist design with smooth animations.
-   **Responsive**: Works seamlessly on both desktop and mobile devices.
-   **Zero Dependencies**: Built with pure JavaScript, HTML, and CSS.
-   **Mock Mode**: Includes sample data for a quick demo without needing API keys.

##  Quick Start

### Prerequisites

-   A modern web browser (Chrome, Firefox, etc.).
-   A local web server to handle ES6 modules.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/cafe-finder.git
    cd cafe-finder
    ```

2.  **Start a local server:**
    ```bash
    # Using Python 3
    python -m http.server 8000

    # Or with Node.js
    npx http-server -p 8000
    ```

3.  **Open in your browser:**
    `http://localhost:8000`

## 📁 Project Structure

```
cafe-finder/
├── index.html              # Main HTML file
├── styles.css              # All styles for the app
├── data/
│   └── mock-places.json    # Mock data for cafes
└── src/
    ├── config.js           # Configuration (API key, mock mode)
    ├── constants.js        # Animation and stack constants
    ├── main.js             # App initialization and event handling
    ├── ui.js               # UI rendering and card creation
    ├── hammer.js           # Swipe gesture handling
    ├── storage.js          # localStorage utility functions
    ├── places.js           # Data fetching (API or mock)
    ├── geolocation.js      # Geolocation utility functions
    └── toast.js            # Toast notification handling
```

## ⚙️ Configuration

The app runs in **mock mode** by default, using local data from `data/mock-places.json`.

To use the **live mode** with the Google Places API:

1.  Get an API key from the [Google Cloud Console](https://console.cloud.google.com/).
2.  Update `src/config.js` with your key:
    ```javascript
    export const apiKey = 'YOUR_GOOGLE_API_KEY';
    export const useMock = false; // Set to false to use the API
    ```

## 🛠️ Technologies Used

-   **Vanilla JavaScript (ES6 Modules)**
-   **Hammer.js** for touch gestures
-   **Google Places API** (optional) for live data
-   **HTML5 & CSS3** for structure and styling

---





