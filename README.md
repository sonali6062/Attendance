```markdown
# 📌 Attendance System with Real-Time QR Code Generation & Scanning

This project is a **real-time attendance management system** that generates dynamic QR codes for each session and uses the **system camera to scan and mark attendance** automatically. It is designed for classrooms, meetings, and events to simplify and digitize attendance tracking.

---

## 📖 Project Overview
- **Dynamic QR Code Generation**: Creates a unique QR code for every attendance session.  
- **Real-Time Camera Scanning**: Uses the system webcam to scan QR codes and mark attendance instantly.  
- **Accurate & Automated**: Reduces human error and streamlines attendance management.  
- **Attendance Logs**: Records data in a CSV/Excel file for easy reporting and analysis.  

---

## 🚀 Features
- Generate a session-specific QR code in real time.  
- Scan the QR using **system camera (OpenCV)**.  
- Automatically log attendance with timestamps.  
- Export attendance records for future use.  

---

## 📂 Project Structure
```

Attendance/
├── qr\_generation.py       # Script to generate QR codes
├── qr\_scanner.py          # Script to scan QR codes using camera
├── attendance\_log.csv     # Attendance records (output file)
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation

````

---

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.7+  
- Webcam or system camera  
- pip (Python package manager)  

### Steps
1. **Clone the repository**
   ```bash
   git clone https://github.com/sonali6062/Attendance.git
   cd Attendance
````

2. **Create virtual environment (recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

---

## 🖥️ Usage

### 1. Generate a QR code

```bash
python qr_generation.py --session-id "Session101" --output qr_session.png
```

* Creates a QR code image (`qr_session.png`) for the given session.

### 2. Scan the QR code & log attendance

```bash
python qr_scanner.py --qr-session "Session101"
```

* Activates the system camera.
* Scans the QR code in real time.
* Logs attendance into `attendance_log.csv` with timestamps.

---

## 🛠️ Technologies Used

* **QR Code Generation**: `qrcode` (Python)
* **Camera & Scanning**: `OpenCV (cv2)`, `pyzbar`
* **Data Logging**: `pandas`, `csv`
* **Environment**: Python, Jupyter/Terminal

---

## 📊 Benefits

* ✅ Fast & convenient for large groups.
* ✅ Error-free compared to manual attendance.
* ✅ Scalable for multiple classes or events.

---



