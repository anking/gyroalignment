# Gyroscope Data Viewer

This project is a web-based gyroscope data viewer that utilizes the device's sensors to measure and display yaw (alpha), pitch (beta), and roll (gamma) angles. The app features sensor fusion techniques, smoothing algorithms, and confidence indicators for improved accuracy.

## Features

- **Real-time Gyroscope Data**: Displays alpha, beta, and gamma values.
- **Sensor Fusion**: Integrates magnetometer (`webkitCompassHeading`) for improved yaw accuracy.
- **Smoothing Algorithm**: Uses weighted averaging to reduce fluctuations.
- **Confidence Indicator**: Displays "High" when `webkitCompassHeading` is available, otherwise "Low".
- **Fix History**: Logs stabilized values when the device is near an aligned position.
- **Low Accuracy Warning**: Displays a warning when magnetometer data is unavailable.
- **User Permission Handling**: Asks for permission to access motion sensors on iOS.

## Installation & Usage

1. Clone the repository:
   ```sh
   git clone https://github.com/anking/gyroalignment.git
   ```
2. Navigate to the project folder:
   ```sh
   cd gyroscope-data-viewer
   ```
3. Open `index.html` in a browser on a mobile device.

### Permissions

On iOS, users must grant permission manually by tapping the "Enable Gyroscope" button when prompted.

## Known Issues

- **Yaw Drift**: While `webkitCompassHeading` improves accuracy, some devices may still experience drift.
- **Sensor Limitations**: Older devices may lack necessary motion sensors.
- **Browser Support**: Works best on Chrome and Safari with motion sensor support enabled.

## Contributing

1. Fork the repository.
2. Create a new branch:
   ```sh
   git checkout -b feature-branch
   ```
3. Commit your changes:
   ```sh
   git commit -m "Add new feature"
   ```
4. Push to your branch:
   ```sh
   git push origin feature-branch
   ```
5. Create a Pull Request.

## License

This project is licensed under the MIT License.
