# Smart Expense Tracker (Flask + SQLite)

A clean, beginner-friendly expense tracker designed for interview readiness. It demonstrates full CRUD, summary analytics, and clear usage of data structures and algorithms in a practical backend project.

## ✨ Features
- Add, edit, and delete expenses
- View all expenses with simple UI
- Category-wise summary (hash map aggregation)
- Monthly summary (hash map aggregation)
- Sort expenses by amount (descending)

## 🧰 Tech Stack (and why)
- **Python + Flask**: Lightweight, fast to learn, and perfect for explaining routing, templates, and REST-style flows in interviews.
- **SQLite**: Zero-config, file-based database that keeps the project simple and portable while still representing real DB usage.
- **HTML/CSS/JS**: Minimal UI for clarity and focus on backend logic.

## 📁 Project Structure
```
expense_tracker/
├── app.py              # Flask app & routes
├── db.py               # Database connection & table creation
├── models.py           # CRUD operations
├── utils.py            # DSA logic: summaries, sorting
└── templates/
    └── index.html      # Simple UI
```

## 🚀 How to Run Locally
1. **Install dependencies**
   ```bash
   pip install flask
   ```
2. **Start the app**
   ```bash
   python app.py
   ```
3. **Open in browser**
   ```
   http://127.0.0.1:5000
   ```

> The SQLite database file (`expenses.db`) is created automatically on first run.

## 🧠 DSA Usage (Interview-friendly)
- **Hash maps for aggregation**: Category and monthly summaries are built using dictionaries to achieve **O(n)** time.
- **Sorting**: Expenses are sorted by amount using Python’s built-in sort, which runs in **O(n log n)** time.
- These are explicitly implemented in `utils.py` with time-complexity comments.

## ✅ Edge Cases Handled
- Empty list (no expenses yet)
- Invalid input (missing fields, negative amount, invalid date)

## 🧩 How This Scales in the Future
- Replace SQLite with PostgreSQL/MySQL for multi-user support.
- Add authentication (optional) and role-based views.
- Move summaries to SQL aggregation for large datasets.
- Add API endpoints and a modern frontend (React/Vue).

## 🗣️ How to Explain in Interviews
- **Why Flask?** It’s lightweight and shows understanding of HTTP routing, templates, and backend flow without overhead.
- **Why SQLite?** Perfect for quick demos; illustrates DB design without setup complexity.
- **Where is DSA used?** In summary aggregations (hash maps) and sorting (O(n log n)).
- **Why this project?** It is realistic, shows CRUD + analytics, and maps directly to backend fundamentals.

---

If you’re prepping for SDE internships, this project gives you a strong, practical story to tell during interviews.
