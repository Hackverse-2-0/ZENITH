## Project Details

### Team Name: ZENITH

### Project Name: VOLTVISION

### Project Description:
VoltVision is an AI-powered aerial inspection and analysis system designed to automate the monitoring of critical infrastructure such as power lines and industrial assets. The system uses a manually controlled drone equipped with a Raspberry Pi Zero 2 W and Camera Module v3 to capture live aerial imagery. These images are processed using multiple custom-trained machine learning models to detect issues such as insulator damage, fire and smoke presence, vegetation encroachment, and corrosion.
Beyond drone-based capture, VoltVision also provides a scalable cloud-enabled web platform where users can directly upload images for instant analysis. The system integrates OpenCV for image handling, deep learning models for defect detection, and a web dashboard that generates real-time results along with downloadable inspection reports. VoltVision aims to reduce manual inspection time, improve early hazard detection, and provide an accessible AI inspection solution for utilities, smart cities, and industrial monitoring.


# Setup & Installation Instructions

## Prerequisites
- Python 3.8 or higher
- pip package manager
- Raspberry Pi OS (for edge device)
- Quadcopter F450 Frame
- Motors – 2200kv
- FC – Apm
- Transmitter and Receiver (Fsi6)
- 2200mah 3s Lipo Battery
- ESCs
- Raspberry pi Zero 2W
- Camera Module V3
- 5v Power Source
- Basic Electronic Instruments: Screw Driver, Soldering Station etc.
- Stable internet connection

## Installation

### Clone the Repository
```bash
git clone https://github.com/your-repo/voltvision.git
cd voltvision
```

### Create virtual environment (recommended)
```bash
python -m venv venv
```

### Activate Environment

**Windows:**
```bash
venv\Scripts\activate
```

**Linux/Mac:**
```bash
source venv/bin/activate
```

### Install dependencies
```bash
pip install -r requirements.txt
```

## Configuration

### Configure model paths
- Place trained model weights inside the `/analysis/models` directory
- Update paths in `/analysis/detection` if required

## Running the Application

### Run the backend server
```bash
python manage.py runserver
```

### Launch the dashboard
Open your browser and go to: [http://localhost:5000](http://localhost:5000)

## Usage

You can test VoltVision in two ways:

### 1. Drone Mode
- Capture images from Raspberry Pi Camera
- Images automatically sent for analysis

### 2. Upload Mode
- Click Analyze
- Upload any inspection image
- View instant AI results
- Download the generated report

---
*System ready for evaluation.*

