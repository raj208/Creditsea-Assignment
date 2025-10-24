# Creditsea — XML Credit Report Uploader (MERN)

A minimal MERN app that:
- uploads an **Experian XML** credit file,
- **parses** key fields (basic details, report summary, credit accounts),
- **saves** the parsed data to **MongoDB Atlas**,
- and provides a small **React UI** to preview/save and view reports.

---

## Tech Stack
- **Backend:** Node 20, Express, Multer, fast-xml-parser, Mongoose, CORS, dotenv  
- **DB:** MongoDB Atlas (Free tier)  
- **Frontend:** Vite + React (plain CSS)

---

## Features
- `POST /api/upload` — validate + **parse preview** (no DB write)
- `POST /api/upload/save` — parse **and** persist to MongoDB
- `GET /api/reports` — list recent or fetch **latest by PAN**
- `GET /api/reports/:id` — fetch one report by id
- React UI: choose XML → **Preview** → **Save to DB** → **View report**

---

## Project Structure
