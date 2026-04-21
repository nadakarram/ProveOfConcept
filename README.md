

# 🚀 SensSystem: Multi-Sensor AI Vision System for Real-Time Cable Defect Detection

![SensSystem Banner](dashbourd.PNG)

---

## 📌 Project Overview

**SensSystem** is an AI-powered industrial inspection platform designed for **real-time cable defect detection** in high-speed manufacturing environments.

The system leverages **computer vision, deep learning (YOLOv8), and multi-sensor integration (2D, 3D, IR)** to detect surface and subsurface defects with high accuracy.

It replaces manual inspection with a **fully automated Industry 4.0 solution** that enhances quality control, reduces human error, and improves production efficiency.

---

## 🧠 Core Idea

SensSystem is not just a detection tool — it is a **complete intelligent inspection ecosystem** that:

- Detects defects in real-time
- Tracks and logs inspection data
- Provides analytics and reports
- Supports continuous AI model improvement
- Integrates seamlessly with industrial workflows

---

## ⚙️ Key Features

- **Real-Time Detection**  
  Live camera streaming with sub-second AI inference.

- **Multi-Media Support**  
  Analyze images and videos for defect detection.

- **Smart Analytics Dashboard**  
  Visual insights into defect trends using charts.

- **Automated Capture System**  
  Automatically saves frames when defects are detected.

- **Role-Based Access Control**  
  Secure system with multiple user roles:
  - Super Admin
  - Admin
  - Technical User

- **PDF Reporting System**  
  Generate professional inspection reports.

- **Database Storage**  
  Store all detection results including:
  - Bounding boxes
  - Confidence scores
  - Images and metadata

---

## 🏭 System Architecture

### 1. Sensor Layer
- 2D Cameras
- 3D Depth Sensors
- IR Thermal Sensors

### 2. AI Processing Layer
- YOLOv8 Object Detection
- Real-time inference
- Multi-sensor data fusion

### 3. Backend Layer
- Flask API
- Image processing pipeline
- Database management

### 4. Frontend Layer
- Dashboard UI
- Analytics visualization
- Monitoring tools

---

## 🧰 Technology Stack

### Backend
- Flask (Python)
- SQLAlchemy
- OpenCV & Pillow
- FPDF (PDF reports)

### AI / Machine Learning
- YOLOv8 (Ultralytics)
- PyTorch

### Frontend
- HTML5 & Jinja2
- CSS3 (Glassmorphism Design)
- JavaScript (ES6+)
- Chart.js

### Database
- MySQL

---

## 🔁 Project Workflow

1. Cable passes through inspection system  
2. Sensors capture real-time data  
3. AI model processes frames  
4. Defects are detected and classified  
5. Results are displayed on dashboard  
6. Data is stored in database  
7. Reports and analytics are generated  

![SensSystem Banner](workflow.jpg)
---

## 🧪 AI Capabilities

- Defect detection (scratches, deformation, surface damage)
- Severity classification (Low / Medium / High)
- Real-time processing
- Continuous improvement using new data
- ng uploaded media, and analyzing historical detection data.


---

##  Technology Stack

### Backend
- **Framework**: [Flask](https://flask.palletsprojects.com/) (Python)
- **Database ORM**: [SQLAlchemy](https://www.sqlalchemy.org/)
- **Image Processing**: [OpenCV](https://opencv.org/) & [Pillow](https://python-pillow.org/)
- **Report Generation**: [fpdf2](https://github.com/fpdf2/fpdf2)

### AI/ML
- **Model**: [YOLOv8](https://docs.ultralytics.com/) (You Only Look Once) by Ultralytics
- **Inference**: Real-time bounding box prediction and classification.

### Frontend
- **Structure**: HTML5 & Jinja2 Templates
- **Styling**: Vanilla CSS3 (Custom Glassmorphism Design)
- **Logic**: Vanilla JavaScript (ES6+)
- **Visualization**: [Chart.js](https://www.chartjs.org/)

### Database
- **Engine**: MySQL

---



##  Installation & Setup

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd project
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Database Configuration**:
   - Create a MySQL database (e.g., `sens_system_db`).
   - Configure your credentials in a `.env` file:
     ```env
     DB_HOST=localhost
     DB_PORT=3306
     DB_USER=root
     DB_PASSWORD=your_password
     DB_NAME=sens_system_db
     ```

4. **Initialize Database**:
   ```bash
   python init_db.py
   ```

5. **Run the Application**:
   ```bash
   python app.py
   ```
   Access the dashboard at `http://127.0.0.1:5000`.

---

## 📸 Usage
1. **Login**: Use your credentials to access the main dashboard.
2. **Detection Mode**:
   - **Live Camera**: Select a camera source and click "Start Camera".
   - **File Upload**: Drag and drop images or videos into the upload zone.
3. **Analytics**: Visit the Analysis page to view historical data and download summary reports.
4. **Settings**: Adjust the confidence threshold and FPS settings in real-time to optimize detection performance.

---

## 📁 Repository Structure
- `app.py`: Main Flask application server.
- `models.py`: Database schema definitions.
- `database.py`: DB connection and session management.
- `static/`: Frontend assets (CSS, JS, Icons).
- `templates/`: HTML templates for different views.
- `results/`: Storage for processed media with detections.
- `runs/`: YOLO training and prediction logs.

---

