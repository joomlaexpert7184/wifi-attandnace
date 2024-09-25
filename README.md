Wifi Attendance Project
#Overview
The Wifi Attendance Project is a Django-based web application developed to streamline attendance management by leveraging WiFi network connections. This project aims to automate the detection of connected devices and track student attendance based on their registered MAC addresses. The project was developed by students of the Industrial Training Institute Bilimora.

#Features
View and manage student details.
Select available WiFi networks.
Detect connected devices within a selected WiFi network.
Highlight students whose MAC addresses match those in the connected devices list.
Generate attendance reports in Excel format.

#Project Structure
wifi_attendance/
├── wifi_attendance/
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── forms.py
│   ├── views.py
│   ├── urls.py
│   └── templates/
│       ├── base.html
│       ├── dashboard.html
│       ├── student_list.html
│       ├── add_student.html
│       ├── confirm_delete.html
│       ├── wifi_list.html
└── manage.py
#Requirements
Python 3.12+
Django 5.0+
Openpyxl for generating Excel files.
Nmap for network scanning.
#Installation
Clone the repository:
git clone https://github.com/joomlaexpert7184/wifi-attendance.git
Navigate to the project directory:
cd wifi-attendance
Create and activate a virtual environment:
python -m venv venv
source venv/bin/activate  # On Windows, use venv\Scripts\activate
Install the required dependencies:
pip install -r requirements.txt
Apply migrations:
python manage.py migrate
Apply migrations:
python manage.py migrate
Run the development server:
python manage.py runserver
Access the application at http://127.0.0.1:8000/.
Usage
Adding Students
Use the "Add Student" feature in the navigation bar to input student details, including name, mobile number, and MAC address.
Detecting Connected Devices
Select a WiFi network from the list to scan for connected devices. The system automatically matches students based on their MAC addresses and marks them as present.
Generating Attendance Report
Click the Download Attendance button to export the current attendance data to an Excel file.
Contributing
Feel free to fork this repository and submit pull requests if you'd like to contribute to the project. All contributions are welcome!
