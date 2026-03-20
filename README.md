<div align="center">

<!-- ANIMATED BANNER -->
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=200&section=header&text=🎧%20Music%20Streaming%20App&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Flutter%20%2B%20FastAPI%20%2B%20Cloudinary&descAlignY=58&descSize=18&descColor=bb86fc&animation=fadeIn" />

<br/>

<!-- BADGES ROW 1 -->
![Flutter](https://img.shields.io/badge/Flutter-%2302569B.svg?style=for-the-badge&logo=Flutter&logoColor=white)
![Dart](https://img.shields.io/badge/Dart-%230175C2.svg?style=for-the-badge&logo=dart&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi&logoColor=white)
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white)

<br/>

> *Stream, discover, and feel the music — beautifully crafted for the modern listener.*

</div>

---

## 🌟 Features

<table>
<tr>
<td width="50%">

### 🔐 Authentication
Secure signup & login with token-based auth — keeping your library safe and personal.

### 🎵 Song Upload
Upload tracks with full metadata: title, artist, cover art, and audio — all stored on Cloudinary.

### 📃 Browse Library
Scroll through every available track on a beautifully designed home screen.

</td>
<td width="50%">

### ❤️ Favourites
One tap to save any song. Your personal collection, always ready.

### 🎧 Interactive Player
Full playback controls — play, pause, seek, and more — in a stunning player UI.

### 🎨 Dynamic Themes
Every song gets its own color palette, transforming the UI to match the mood of the music.

</td>
</tr>
</table>

---

## 📱 App Preview

<div align="center">

### 🏠 Home Screen

<img src="client/assets/screenshots/home.png" width="320" alt="Home Screen" />

<br/><br/>

### 🔐 Authentication

<table>
<tr>
<td align="center">

**✍️ Sign Up**

<img src="client/assets/screenshots/signup.png" width="280" alt="Sign Up Screen"/>

</td>
<td align="center">

**🔑 Sign In**

<img src="client/assets/screenshots/login.png" width="280" alt="Login Screen"/>

</td>
</tr>
</table>

<br/>

### 🎵 Upload a Song

<img src="client/assets/screenshots/upload.png" width="320" alt="Upload Screen" />

</div>

---

## ⚙️ Backend & Data

<div align="center">

### 🛠️ FastAPI Swagger Docs

<img src="client/assets/screenshots/backend.png" width="750" alt="FastAPI Backend Docs" />

<br/><br/>

### 📊 Song Metadata Response

<img src="client/assets/screenshots/db.png" width="750" alt="API Response Data" />

</div>

> Each song response includes **title**, **artist**, **audio URL**, **thumbnail URL**, and a **hex color** used to theme the player UI dynamically.

---

## 🧠 Architecture

<div align="center">

```
  ┌─────────────────────────────────────────────┐
  │              📱  Flutter App                │
  │         Beautiful UI · Dart · Mobile        │
  └──────────────────┬──────────────────────────┘
                     │  REST API (HTTP/JSON)
                     ▼
  ┌─────────────────────────────────────────────┐
  │            ⚡  FastAPI Backend              │
  │       Python · Auth · Song Management       │
  └──────────────────┬──────────────────────────┘
                     │  Upload / Stream Media
                     ▼
  ┌─────────────────────────────────────────────┐
  │           ☁️  Cloudinary Storage            │
  │        Audio Files · Cover Images           │
  └─────────────────────────────────────────────┘
```

</div>

---

## 🏗️ Tech Stack

<div align="center">

| Layer | Technology | Purpose |
|:---:|:---:|:---|
| 📱 Frontend | ![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white) ![Dart](https://img.shields.io/badge/Dart-0175C2?style=flat-square&logo=dart&logoColor=white) | Cross-platform mobile UI |
| ⚙️ Backend | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) | REST API & business logic |
| ☁️ Storage | ![Cloudinary](https://img.shields.io/badge/Cloudinary-3448C5?style=flat-square&logo=cloudinary&logoColor=white) | Audio & image hosting |

</div>

---

## 📂 Project Structure

```
🎵 music-app/
│
├── 📱 client/                    ← Flutter Frontend
│   ├── lib/
│   │   ├── core/                 ← Constants, themes, utils
│   │   ├── features/
│   │   │   ├── auth/             ← Login & Signup screens
│   │   │   ├── home/             ← Browse & player UI
│   │   │   └── upload/           ← Song upload screen
│   │   └── main.dart
│   └── assets/
│       └── screenshots/          ← App preview images
│
├── ⚡ server/                    ← FastAPI Backend
│   ├── main.py                   ← App entry point
│   ├── routes/                   ← API route handlers
│   └── models/                   ← Data models
│
├── requirements.txt
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites

- Flutter SDK `≥ 3.0`
- Python `≥ 3.9`
- A [Cloudinary](https://cloudinary.com) account

### 1️⃣ Clone

```bash
git clone https://github.com/akankshacore/music-app.git
cd music-app
```

### 2️⃣ Backend

```bash
cd server
pip install -r requirements.txt
uvicorn main:app --reload
```

```
✅  API running at   → http://localhost:8000
📖  Swagger docs at  → http://localhost:8000/docs
```

### 3️⃣ Frontend

```bash
cd client
flutter pub get
flutter run
```

---

## 🗺️ Roadmap

```
✅  User Authentication
✅  Song Upload (Cloudinary)
✅  Browse Song Library
✅  Favorites
✅  Interactive Music Player
✅  Dynamic Color Theming
⬜  Search & Filter
⬜  Playlist Support
⬜  Audio Streaming Optimization
⬜  Offline Mode
⬜  Social Sharing
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repo
2. Create a feature branch — `git checkout -b feature/amazing-feature`
3. Commit your changes — `git commit -m 'Add amazing feature'`
4. Push to the branch — `git push origin feature/amazing-feature`
5. Open a Pull Request

---

## 👩‍💻 Author

<div align="center">

**Akanksha**

[![GitHub](https://img.shields.io/badge/GitHub-akankshacore-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/akankshacore)

</div>

---

<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:24243e,50:302b63,100:0f0c29&height=120&section=footer" />

</div>
