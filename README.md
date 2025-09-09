# 🩺 Blood Pressure Tracker

A full-stack application to record, analyze, and track blood pressure readings with secure authentication, OCR scanning, Excel export, and interactive visualizations.

---

## 🚀 Features
- 🔑 **Authentication** – Register/Login with hashed passwords & token-based auth  
- 📝 **Readings Management** – Add, edit, delete, and view BP readings  
- 📱 **Swipe Gestures** – Mobile-friendly delete/edit actions  
- 📷 **OCR Scanning** – Extract readings from uploaded images (Tesseract.js)  
- 📊 **Analysis Charts** – Filter by day, month, year, or custom range  
- 🎯 **Target Lines** – Highlight healthy SYS/DIA levels in charts  
- 📤 **Excel Export** – Download history with optional date range  
- 🌐 **Responsive UI** – Tailored for both desktop & mobile  

---

## 🛠️ Tech Stack
**Backend**
- Flask + PostgreSQL  
- psycopg2, openpyxl  
- Token-based authentication  

**Frontend**
- React (Vite) + Tailwind CSS  
- Chart.js + lucide-react icons  
- Tesseract.js for OCR  

---

## 📦 Setup & Run

### Backend
```bash
# clone repo & go to backend folder
cd backend
pip install -r requirements.txt

# set environment variables
export DATABASE_URL="your_postgres_url"
export PORT=5000

# run server
python app.py

Frontend
# clone repo & go to frontend folder
cd frontend
npm install
npm run dev

📂 API Endpoints
Method	Endpoint	Description
POST	/api/register	Register new user
POST	/api/login	Login & get token
POST	/api/bp	Add a reading
PUT	/api/bp/:id	Update a reading
DELETE	/api/bp/:id	Delete a reading
GET	/api/history	Fetch history of readings
GET	/api/export	Export readings to Excel
📊 Demo Screenshots

🔐 Login/Register

📝 Add & OCR Readings

📊 Analysis with Filters

📤 Export to Excel

🌍 Deployment

Backend: Render / Supabase / Heroku

Frontend: Vercel / Netlify
