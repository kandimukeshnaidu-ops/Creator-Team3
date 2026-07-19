# Creator Analytics Dashboard (Creator-Team3)

A monorepo for the Creator Analytics Dashboard application containing both the React frontend and FastAPI backend.

---

## Project Structure
* **`/src`**: React/Vite Frontend source code (dashboard layout, analytics views, revenue tracker, link history analyzer, settings, themes, charts).
* **`/backend`**: FastAPI Python Backend source code (SQLite database connection, user registration/login tokens, notifications logs, social link parser endpoints, revenue CRUD endpoints).
* **`/database`**: Database setup SQL schema dump from teammate Sonali.
* **Root**: Frontend configuration files (`package.json`, `vite.config.js`, etc.).

---

## Getting Started

### 1. Frontend Setup
Make sure you have [Node.js](https://nodejs.org/) installed.
1. Open terminal at the root directory of the project.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
   *The frontend will run at **http://localhost:5173/***

---

### 2. Backend Setup
Make sure you have [Python 3.10+](https://www.python.org/) installed.
1. Open a terminal at the `/backend` directory.
2. Create and activate a Python virtual environment:
   ```bash
   python -m venv .venv
   ```
   * **Windows**:
     ```powershell
     .venv\Scripts\activate
     ```
   * **macOS/Linux**:
     ```bash
     source .venv/bin/activate
     ```
3. Install the backend dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Start the API development server:
   ```bash
   python -m uvicorn main:app --reload
   ```
   *The API backend will run at **http://127.0.0.1:8000/***