
```markdown
#  Attendance System with Real-Time QR Code Generation & Scanning

This **Attendance System** project implements a real-time solution for attendance tracking using dynamically generated QR codes and live camera scanning. It enables streamlined, error-resistant attendance marking in classrooms, meetings, or events.

---

##  Project Overview

- **Dynamic QR Code Generation**: Generates unique QR codes for each attendance session securely.
- **Real-Time Camera Scanning**: Captures QR codes via the system camera to instantly register attendance.
- **Automation & Accuracy**: Streamlines attendance management with minimal human intervention while improving accuracy and efficiency.

---

##  Features

- Generate and display a **session-specific QR code** for attendees to scan.
- **Live scanning using camera** (via OpenCV or equivalent) to read QR codes in real time.
- Real-time attendance logging and confirmation through a visual interface or console.
- Exportable attendance data (CSV, Excel) for record-keeping and analysis.

---

##  Project Structure

```

Attendance/
├── qr\_generation.py       # Script to generate QR codes for sessions
├── qr\_scanner.py          # Script to scan QR codes using camera
├── attendance\_log.csv     # Sample or output attendance records
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation

````

---

##  Installation & Setup

### Prerequisites
- Python 3.7 or later  
- pip (Python package manager)  
- Webcam or system camera  

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/sonali6062/Attendance.git
   cd Attendance
````

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the QR code generator**

   ```bash
   python qr_generation.py --session-id "Session123" --output qr_session.png
   ```

   This creates a unique QR code (`qr_session.png`) for the given session.

4. **Start the QR scanner**

   ```bash
   python qr_scanner.py --qr-session "Session123"
   ```

   Activates the camera, scans for the corresponding session QR, and logs attendance in real time.

---

## Usage Example

1. Generate a QR code for the session:

   ```bash
   python qr_generation.py --session-id "Math_101" --output qr_math101.png
   ```

2. Display the QR code on screen or print it.

3. Attendees scan the QR by running the scanner:

   ```bash
   python qr_scanner.py --qr-session "Math_101"
   ```

4. Attendance records are logged in `attendance_log.csv` with timestamps.

---

## Technologies Used

* **QR Code Generation**: `qrcode` library (Python)
* **Real-Time Scanning**: OpenCV (`cv2`), `pyzbar`, or similar for image capture and QR decoding
* **Data Handling**: `pandas`, `csv` for attendance logging and export
* **Environment**: Python 3.x, terminal / GUI display

---

## Benefits & Impact

* **Speed & Convenience**: Attendance can be recorded with a single scan—ideal for large groups.
* **Reduced Errors**: Eliminates manual entry mistakes and misidentification.
* **Scalable & Adaptable**: Session-based QR generation supports multiple classes or events seamlessly.

---


---

