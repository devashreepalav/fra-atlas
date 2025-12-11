# 🌳 FRA Digital Atlas — AI + GIS Powered Forest Rights Act Mapping Platform

The **FRA Digital Atlas** is an open-source, GIS-enabled platform built to support the **Forest Rights Act (FRA), India** by digitizing, mapping, and analyzing forest land rights.  
It provides an interactive way to visualize claims, approvals, village boundaries, and geospatial layers through a user-friendly dashboard.

---

## 🚀 Features

### 🗺️ **Interactive GIS Mapping**
- Built using **Leaflet.js** and **GeoDjango**
- Supports zoom, pan, and live geographic overlays
- Displays village boundaries, forest areas, and claim polygons

### 📊 **Data Visualization**
- Charts & analytics for FRA claim status  
- Detailed attribute tables  
- Layer toggling and filtering options  

### 🤖 **AI-assisted Insights**
- Automated analysis workflows  
- Smart data validation  
- Error handling for GeoServer connections

### 🏛️ **Admin & Role-Based Access**
- Django admin panel  
- Upload/modify shapefiles and geospatial layers  
- Secure user authentication  

---

## 🧰 Tech Stack

| Component | Technology |
|----------|------------|
| Backend | **Python, Django, GeoDjango** |
| Frontend | **HTML, CSS, JavaScript, Leaflet.js** |
| Database | **PostgreSQL + PostGIS** |
| GIS Services | **GeoServer** |
| Deployment | **Docker, Docker Compose** |

---

## 📂 Project Structure

```
fra-atlas/
│
├── geoApp/                  # Main Django application
│   ├── templates/           # HTML templates (dashboard, maps, details pages)
│   ├── static/              # CSS, JS, images
│   ├── tiff/                # TIFF processing utilities
│   ├── migrations/          # Database migrations
│   ├── views.py             # Map + analytics logic
│   ├── models.py            # Database models
│   └── urls.py              # URL routing
│
├── Dockerfile               # Docker build config
├── requirements.txt         # Dependencies
├── run_local.py             # Script to start local server
├── railway.toml             # Deployment config
└── README.md                # Project documentation
```

---

## 🛠️ Installation & Setup

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/devashreepalav/fra-atlas.git
cd fra-atlas
```

### **2️⃣ Create Virtual Environment**
```bash
python -m venv env
source env/bin/activate  # Windows: env\Scripts\activate
```

### **3️⃣ Install Requirements**
```bash
pip install -r requirements.txt
```

### **4️⃣ Set Up PostgreSQL + PostGIS**
Create a database:
```sql
CREATE DATABASE fra_atlas;
CREATE EXTENSION postgis;
```

Configure credentials in `settings.py`.

### **5️⃣ Run Migrations**
```bash
python manage.py migrate
```

### **6️⃣ Start Development Server**
```bash
python manage.py runserver
```

Access the site at:  
👉 **http://localhost:8000**

---

## 📸 Screenshots (Optional)
_Add your dashboard/map screenshots here later._

---

## 🤝 Contributing
Contributions are welcome!  
Fork the repo → Create a branch → Make changes → Submit a pull request.

---

## 📜 License
This project is open-source under the **MIT License**.

---

## ✨ Acknowledgements
- Ministry of Tribal Affairs, GoI  
- Open-source GIS community  
- Contributors of Django, GeoDjango, Leaflet, PostgreSQL  
