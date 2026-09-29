<div align="center">

# 🛡️ Javi.QL

### *Ctrl+Z for your database.*

**Just-in-time Automated Versioned Intelligence for SQL**

![Python](https://img.shields.io/badge/python-3.12-blue) ![FastAPI](https://img.shields.io/badge/FastAPI-009688) ![License](https://img.shields.io/badge/license-MIT-green)

</div>

---

## 😱 The problem

It's 5:58 PM. You type `DELETE FROM orders` and forget the `WHERE`.

## 😌 The Javi.QL fix

Before a single row is touched, Javi.QL **quietly saves it to a CSV** and hands you the rollback SQL. Mistakes stop being disasters and turn into a one-click undo.

---

## ✨ Superpowers

| | Power | What it means |
|---|---|---|
| 💾 | **Backup Vault** | Every `UPDATE` / `DELETE` is backed up first, with rollback SQL on demand |
| 🔍 | **Query Console** | PostgreSQL, MySQL and SQLite in one place. `Ctrl+Enter` to fire |
| 🗺️ | **Live Inspector** | Explore tables, columns and types without leaving the page |
| 🤖 | **AI Generator** | Say *"top 10 customers by order value"*, get SQL back from Gemini |
| 📜 | **Audit Trail** | Who ran what, when, how long, and how many rows it touched |

## 🚀 Take off in 60 seconds

```bash
git clone https://github.com/janhavichauhan/JaviQL.git
cd JaviQL
pip install -r requirements.txt
python main.py
```

Your browser opens at **http://127.0.0.1:8000**. Hit **No Database Connected**, fill in your details, and you're in.

<details>
<summary>🔧 Optional: enable audit logging with a <code>.env</code></summary>

```bash
DB_TYPE=postgresql
DB_HOST=your-host
DB_PORT=5432
DB_NAME=your_db
DB_USER=your_user
DB_PASSWORD=your_password
```

</details>

## 🎬 How a rollback feels

1. Run `DELETE FROM users WHERE status = 'inactive'`
2. 📥 A CSV of the doomed rows lands in your downloads
3. 😬 You realise that was the wrong filter
4. 🪄 Open the **Vault**, press **Rollback**, and get the rows back

## 🧰 Under the hood

`FastAPI` · `SQLAlchemy` · `Vanilla JS` · `Tailwind` · `Google Gemini`

## ☁️ Ship it

A `render.yaml` is included. Point [Render](https://render.com) at this repo and it deploys.

---

<div align="center">

**Made with 💙 for everyone who has ever typed DELETE and held their breath.**

<sub>MIT License</sub>

</div>
