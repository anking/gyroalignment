Gyroscope Data Viewer
This project is a web-based gyroscope data viewer that utilizes the device's sensors to measure and display yaw (alpha), pitch (beta), and roll (gamma) angles. The app features sensor fusion techniques, smoothing algorithms, and confidence indicators for improved accuracy.

Features
Real-time Gyroscope Data: Displays alpha, beta, and gamma values.
Sensor Fusion: Integrates magnetometer (webkitCompassHeading) for improved yaw accuracy.
Smoothing Algorithm: Uses weighted averaging to reduce fluctuations.
Confidence Indicator: Displays "High" when webkitCompassHeading is available, otherwise "Low".
Fix History: Logs stabilized values when the device is near an aligned position.
Low Accuracy Warning: Displays a warning when magnetometer data is unavailable.
User Permission Handling: Asks for permission to access motion sensors on iOS.
Installation & Usage
Clone the repository:
git clone https://github.com/yourusername/gyroscope-data-viewer.git
Navigate to the project folder:
cd gyroscope-data-viewer
Open index.html in a browser on a mobile device.
Permissions
On iOS, users must grant permission manually by tapping the "Enable Gyroscope" button when prompted.

Known Issues
Yaw Drift: While webkitCompassHeading improves accuracy, some devices may still experience drift.
Sensor Limitations: Older devices may lack necessary motion sensors.
Browser Support: Works best on Chrome and Safari with motion sensor support enabled.
Contributing
Fork the repository.
Create a new branch:
git checkout -b feature-branch
Commit your changes:
git commit -m "Add new feature"
Push to your branch:
git push origin feature-branch
Create a Pull Request.
License
This project is licensed under the MIT License.
