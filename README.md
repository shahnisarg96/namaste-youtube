# Namaste YouTube Clone

A YouTube-inspired video streaming web application built with **React**, **Redux Toolkit**, and **Tailwind CSS**.  
This project demonstrates modern React concepts, efficient state management, API integration, and performance optimizations such as **debouncing** and **caching**.

---

## 🚀 Features

- **Home Feed**: Browse trending YouTube videos (fetched via YouTube Data API).
- **Video Player**: Embedded player with a dedicated watch page.
- **Live Chat**: Simulated live chat with random user messages and input support.
- **Comments Section**: Nested comments with recursive rendering.
- **Sidebar Navigation**: Toggleable sidebar with intuitive links.
- **Search with Suggestions**: Debounced and cached search suggestions for instant results.

### ⚡ Performance Optimizations

- **Debouncing** search input to minimize API calls.
- **Caching** of suggestions in Redux for O(1) lookup.
- `useMemo` and `useRef` for efficient re-renders and state control.

---

## 🛠️ Tech Stack

- React
- Redux Toolkit
- React Router
- Tailwind CSS
- YouTube Data API
- Jest & React Testing Library

---

## 📁 Project Structure

```
namaste-youtube/
├── public/
├── src/
│   ├── components/
│   ├── utils/
│   ├── App.js
│   ├── App.css
│   ├── index.js
│   └── ...
├── .env
├── package.json
├── tailwind.config.js
└── README.md
```

---

## ⚙️ Setup & Installation

1. **Clone the repository:**

```bash
git clone <repo-url>
cd namaste-youtube
```

2. **Install dependencies:**

```bash
npm install
```

3. **Set up environment variables:**

Create a `.env` file in the root directory and add your YouTube API key:

```
REACT_APP_GOOGLE_API_KEY=YOUR_YOUTUBE_API_KEY
```

4. **Start the development server:**

```bash
npm start
```

Visit: [http://localhost:3000](http://localhost:3000)

---

## 🔍 Key Concepts & Code Highlights

### 🔁 Debouncing
Search suggestions are fetched with a **debounce delay** to reduce API calls.

### 🧠 Caching
Search results are cached in Redux for **instant lookup**.

### 🧵 Redux Store
Centralized store manages:
- UI state
- Search suggestions
- Live chat messages

### 💬 Live Chat Simulation
Random messages generated at intervals using mock users and texts.

### 🧷 Recursive Comments
Nested comments rendered recursively for threading.

### 🚀 Performance
- `useMemo`: Prevents expensive recalculations.
- `useRef`: Stores mutable values without triggering re-renders.

---

## 📌 Notes

- This is an **educational project** inspired by Akshay Saini’s Namaste React series.
- You must provide your own YouTube Data API key in the `.env` file.
- The live chat and comments are **simulated** for demo purposes.

---

## 📚 References

- [Namaste React](https://namastedev.com/learn/namaste-react)
- [Redux Toolkit Documentation](https://redux-toolkit.js.org/)
- [Tailwind CSS Documentation](https://tailwindcss.com/)

---

## 👨‍💻 Author

Inspired by: **Akshay Saini**  
Project by: **Nisarg Shah**
