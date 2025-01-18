# Face-Recognition-Attendance-System
## Overview
This project is a face recognition-based attendance system that identifies individuals using a webcam and logs their attendance. The attendance log is then emailed to a specified address. The system uses the face_recognition library and OpenCV for facial recognition and handles attendance tracking in real time.

## Features
Real-time face recognition using a webcam.
Automatic logging of recognized faces with timestamps.
Email notification with the attendance log attached as a CSV file.
Prerequisites
Python 3.6 or later.
Install required libraries:
bash
Copy
Edit
pip install -r requirements.txt
## Setup
Face Database:
Prepare your own face image dataset and store it in a directory (e.g., path/to/your/images). Images should be named according to the individual's name (e.g., John.jpg).

Embeddings File:
The script automatically generates a .pkl file (face_database_class.pkl) to store face encodings for future use.

Email Configuration:

Replace the placeholder values in the script with your own:
sender_address: Your email address.
sender_pass: Your email's app-specific password.
receiver_address: The recipient's email address.
Use an app-specific password if using Gmail or similar services.
Run the System:

bash
Copy
Edit
python script.py
Press q to quit the video feed.
## Limitations
Face Database: The script does not include a default face database due to privacy concerns. You must create and preprocess your own dataset.
Email Configuration: Sensitive information like email credentials is required for sending emails. Ensure these are handled securely and not shared publicly.
Security
Sensitive Data: Ensure that private images and credentials are not included in the repository. Use environment variables or a .env file to store sensitive information securely.
## Future Improvements
Implement environment variable support for email credentials.
Integrate a GUI for easier configuration.
Add support for multiple recipients.
## Disclaimer
This project is for educational purposes only. Do not use private images without the subject's consent.


