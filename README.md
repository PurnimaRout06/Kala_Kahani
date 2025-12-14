<p align="center">
  <img src="logo.jpeg" alt="KALA Banner" width="1000"/>
</p>

<h1 align="center">KALA – Artisan Marketplace Platform</h1>

<p align="left">
A platform that connects artisans, buyers, and volunteers to promote handmade art using AI-powered pricing and multilingual voice assistance.
</p>

---

##  Problem Statement
Many artisans struggle with fair pricing, digital visibility, and access to buyers. Middlemen reduce profits, and language barriers limit reach. KALA addresses these challenges by combining technology, AI, and community support.

---

##  Our Solution
KALA is a digital marketplace where artisans can showcase and sell their products, buyers can discover authentic handmade art, and volunteers can organize skill-building workshops. An integrated AI assistant helps artisans with pricing, language support, and product improvement suggestions.

## 🎥 Demo Video

<p align="center">
  <a href="https://youtu.be/A_xojfM45Vc" target="_blank">
    <img src="https://img.youtube.com/vi/A_xojfM45Vc/0.jpg" alt="KALA Demo Video" width="80%">
  </a>
</p>

---

##  User Roles
- **Artisan:** Upload products, view AI suggestions, track earnings  
- **Buyer:** Browse and purchase handmade products  
- **Volunteer:** Organize workshops and support artisans

---
##  Getting Started

### 1. Clone the Repository
bash

git clone https://github.com/your-username/kala.git


---

### 2. Frontend Setup
bash

cd frontend

npm install

npm run dev


Frontend runs on http://localhost:8080

---
### 3. Backend Setup
bash

cd backend

npm install


Create .env

MONGO_URL=your_mongodb_connection
JWT_SECRET=your_secret


Run backend:

bash

node index.js


Backend runs on http://localhost:5000

## 📁 Project Structure

```text
kala/
├── artisan-bridge/               # React application (UI)
│   ├── src/
│   │   ├── api/            # API calls to backend
│   │   │   ├── api.js
│   │   │   ├── auth.js
│   │   │   ├── product.js
│   │   │   └── workshop.js
│   │   │
│   │   ├── pages/          # Application pages
│   │   │   ├── Register.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Dashboard.jsx
│   │   │
│   │   ├── components/     # Reusable UI components
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   └── public/
│
├── backend/                # Node + Express server
│   ├── index.js            # Server entry point
│   ├── routes/             # API routes
│   │   ├── auth.js
│   │   ├── product.js
│   │   └── workshop.js
│   │
│   ├── models/             # MongoDB schemas
│   └── uploads/            # Uploaded images
│
├── logo.jpeg       # README banner photo
└── README.md
