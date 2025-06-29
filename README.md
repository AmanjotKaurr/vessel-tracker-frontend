
# 🌍 Vessel Movement Tracker – Frontend (HTML + JavaScript)

This is the **frontend interface** for the Vessel Movement Tracker project. It interacts with the backend API to display and manage vessel journeys in real-time.

## 🌐 Live Frontend

- **Vercel Deployment**: [https://vessel-tracker-frontend.vercel.app](https://vessel-tracker-frontend.vercel.app)
- **GitHub Pages**: [https://amanjotkaurr.github.io/vessel-tracker-frontend/](https://amanjotkaurr.github.io/vessel-tracker-frontend/)

## 📦 Technologies Used

- HTML5, CSS3
- Vanilla JavaScript (Fetch API)
- GitHub Pages / Vercel for deployment

## 🔗 Connected API

The frontend connects to the backend hosted on Railway:

```
API_BASE = https://vessel-movement-tracker-production.up.railway.app/api/vessels
```

## ⚙️ Features

- Add a new vessel with name, origin, destination, speed, and distance.
- See real-time progress with animated progress bars.
- View estimated time remaining and traveled kilometers.
- Reset all vessels to restart their journeys.
- Delete individual vessels.
- Auto-refreshes every 10 seconds to simulate movement.

## 📁 Folder Structure

```
frontend/
├── index.html       # Main UI file
└── README.md        # Project description
```

## 🚀 Deployment Guide

### On Vercel:

1. Create a new project.
2. Import this repo.
3. Set:
   - **Root Directory**: `frontend/`
   - **Build Command**: (leave empty)
   - **Output Directory**: `.`

### On GitHub Pages:

1. Go to GitHub repo settings → Pages.
2. Set:
   - **Source**: `main`
   - **Folder**: `/frontend`
3. Ensure `index.html` exists in `/frontend/`.

## 🧪 API Communication

All API requests use `fetch()` to:

- `GET` vessel data
- `POST` new vessels
- `DELETE` vessels
- `POST /reset` to restart journeys

Make sure CORS is enabled in backend.

## 📄 License

MIT License
