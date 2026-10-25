# 🎬 Movie Recommendation System

A web-based **Movie Recommendation System** that helps users discover movies, explore movie details, and manage their personal watchlist. Built with a React frontend and a Python FastAPI backend.

## ✨ Features

- 🔐 **User Authentication** — Sign up and sign in to your account.
- 🎥 **Movie Discovery** — Browse a collection of movies.
- 🤖 **Personalized Recommendations** — Get movie recommendations based on the application's recommendation logic.
- 🔎 **Movie Details** — Explore information about individual movies.
- 📚 **Watchlist / Library** — Keep track of movies you want to watch.
- 🕒 **Watch History** — Track movie interactions where supported.
- 🖼️ **Movie Posters** — Display movie posters using TMDB image URLs.
- 📱 **Responsive UI** — A modern interface built with React and Tailwind CSS.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| React | Frontend UI |
| Vite | Frontend development server and build tool |
| Tailwind CSS | Styling |
| Axios | API requests |
| Python | Backend development |
| FastAPI | REST API |
| Uvicorn | Backend server |
| SQLite | Local database |
| Pandas / CSV | Movie data processing |

## 📁 Project Structure

```text
MOVIE-RECOMMENDATION/
├── backend/
│   ├── data/
│   ├── main.py
│   ├── movies.csv
│   ├── ratings.csv
│   ├── requirements.txt
│   └── package.json
├── frontend/
│   ├── src/
│   │   └── components/
│   ├── index.html
│   ├── package.json
│   ├── vite.config.js
│   └── tailwind.config.js
├── .gitignore
└── README.md
```

## ⚙️ Prerequisites

Install the following before running the project:

- Python 3
- Node.js and npm
- Git

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/sudhagirishgeet/MOVIE-RECOMMENDATION.git
cd MOVIE-RECOMMENDATION
```

### 2. Set Up the Backend

Open a terminal in the project root and run:

```bash
cd backend
python -m venv venv
```

Activate the virtual environment.

**Windows:**

```cmd
venv\Scripts\activate
```

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

Start the backend server:

```bash
python main.py
```

The backend runs at:

`http://127.0.0.1:8000`

If FastAPI's interactive API documentation is enabled, visit:

`http://127.0.0.1:8000/docs`

### 3. Set Up the Frontend

Open a **second terminal** in the project root:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL shown in the terminal, typically:

`http://localhost:5173`

Keep both the backend and frontend terminals running while using the application.

## 🔗 API Integration

The React frontend communicates with the FastAPI backend through HTTP requests.

For local development, the frontend API base URL is configured as:

```javascript
const PY_URL = "http://127.0.0.1:8000";
```

The backend must be running for authentication, movie data, watchlist, and recommendation requests to work.

## 🔑 Environment & Security

- Do not commit passwords, API keys, access tokens, or private environment files.
- Keep local database files and user data out of public repositories.
- Configure the backend URL appropriately before deploying the frontend.
- If using a TMDB API key, store it securely in an environment variable rather than hardcoding it.

## 🧪 Troubleshooting

**Backend does not start**
- Verify Python is installed.
- Install dependencies from `backend/requirements.txt`.
- Check the terminal for missing packages or database errors.

**Frontend does not start**
- Verify Node.js and npm are installed.
- Run `npm install` inside the `frontend` directory.
- Check the terminal for build errors.

**API or CORS errors**
- Ensure the backend is running.
- Verify the frontend API URL.
- Confirm that the backend allows requests from the frontend's local origin.

## 🔮 Future Enhancements

- Improve personalized recommendation algorithms.
- Add advanced movie search and filtering.
- Add movie ratings and reviews.
- Deploy the frontend and backend to production.
- Enhance recommendation quality using user preferences and viewing history.

## 👨‍💻 Author

**SudhaGirishGeet**

GitHub: [@sudhagirishgeet](https://github.com/sudhagirishgeet)

---

⭐ If you find this project interesting, consider giving the repository a star!

*Built as a movie discovery and recommendation web application.*
