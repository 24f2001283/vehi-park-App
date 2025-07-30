
# 📝 Project Report: Vehicle Parking App - V1  

**Name:** Hiruthik Sudhakar  
**Roll No:** 24F2001283  
**Email:** 24f2001283@ds.study.iitm.ac.in  

---

## 🚀 Project Title  
**Vehicle Parking App – V1: Smart Parking Management System**

---

## 📚 Frameworks and Libraries Used  

- **Python**: 3.x 🐍  
- **Flask**: Micro web framework 🌐  
- **SQLite**: Lightweight relational DB 💾  
- **Flask-SQLAlchemy**: ORM for DB modeling 🛠️  
- **Matplotlib**: Visual analytics for charts 📊  
- **Bootstrap**: UI design framework 🎨  
- **Jinja2**: HTML templating engine 🔗  
- **HTML, CSS, JavaScript**: Frontend technologies 🖼️  

---

## 🛠️ Getting Started  

### 🔧 Prerequisites  
Ensure Python 3.x is installed.

### 📦 Installation Steps  

1. **Clone the repository:**  
   ```bash
   git clone https://github.com/24f2001283/vehi-park-App.git
   cd vehi-park-app/vehi_park_app_24f2001283
   ```

2. **Set up a virtual environment:**  
   ```bash
   python -m venv venv
   ```

3. **Activate the environment:**  
   - On Windows:  
     ```bash
     venv\Scripts\activate
     ```  
   - On macOS/Linux:  
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies:**  
   ```bash
   pip install -r requirements.txt
   ```

5. **Run the application:**  
   ```bash
   flask run
   ```

6. **Access it in your browser:**  
   [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 📝 Abstract  

The Vehicle Parking App is a multi-user Flask-based web application that allows users to manage 4-wheeler parking in multiple lots. It provides role-based dashboards for **Admin** and **User**, enables parking spot allocation, history tracking, and real-time visual summaries through integrated chart visualizations.

---

## 🌟 Core Functionalities  

### 👨‍💼 Admin:  
- Add/edit/delete parking lots and auto-create parking spots.  
- Monitor and manage all bookings, users, and lot statuses.  
- Cascade delete functionality for related spots.  
- Visualize booking and occupancy stats using charts.  
- Search interface for user/bookings/lot information.  

### 🧍 User:  
- Register, login, and access personal dashboard.  
- View available lots and book or release parking spots.  
- Track booking history with cost and timestamps.  
- Access summary charts for personal usage insights.  

---

## 🧱 Database Schema  

> SQLite-based schema created using SQLAlchemy.  
> Models include: `User`, `ParkingLot`, `ParkingSpot`, `Booking`  
> Supports relations with cascading delete and timestamp tracking.

---

## 🌐 API Endpoints (Controller)

| Route | Method(s) | Description |
|-------|-----------|-------------|
| `/` | GET, POST | Login for admin and users |
| `/register` | GET, POST | User registration |
| `/user` | GET, POST | User dashboard |
| `/booking/<spot_id>` | GET, POST | Book a parking spot |
| `/release_booking/<booking_id>` | GET, POST | Release spot and calculate cost |
| `/history` | GET, POST | View user booking history |
| `/summary` | GET | Show user dashboard summary charts |
| `/admin` | GET | Admin dashboard |
| `/add_parking` | GET, POST | Add new parking lot |
| `/edit_parking/<id>` | GET, POST | Edit parking lot |
| `/delete_parking/<id>` | GET, POST | Delete parking lot |
| `/delete_spot/<id>` | POST | Delete parking spot |
| `/admin_user` | GET, POST | Manage all users (non-admin) |
| `/edit_user/<id>` | GET, POST | Edit user profile |
| `/delete_user/<id>` | GET | Delete user |
| `/admin/search` | GET | Admin search |
| `/admin/summary` | GET, POST | Charts for admin dashboard |
| `/admin/booking/<id>` | GET, POST | Admin books spot for user |

---

## ⚙️ Execution Strategy  

### 📌 Step 1: Requirement Analysis  
- Defined admin and user roles  
- Set CRUD functionality for lots and booking logs  
- Designed responsive UI with Bootstrap  

### 📌 Step 2: Modular Development  
- Authentication for both roles  
- Admin: Create/Edit lots, auto-create spots, view usage  
- Users: Book and release spots with live tracking  
- Visual summaries using Matplotlib  

---

## 📽️ Video Demo  

🎥 [Click to Watch Demo](https://drive.google.com/file/d/1sflHPS0V6E5TXlUPXPjgMx8Y4oelKaWs/view)

---
