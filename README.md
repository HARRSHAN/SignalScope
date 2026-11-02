# SignalScope

**SignalScope** is a Python desktop application for acquiring, monitoring, and recording real-time signals through a serial connection. It provides a live plotting interface for observing incoming data and supports saving recorded samples for further analysis.

## Features

- Real-time signal visualization.
- Serial-port connection for receiving data from external hardware.
- Demo/simulated signal mode for testing the interface without connected hardware.
- Start and stop recording.
- Export recorded samples to CSV for analysis.
- Capture the signal plot as an image.

## Technology Stack

- **Python**
- **PySide6** – desktop graphical user interface
- **PyQtGraph** – real-time plotting
- **PySerial** – serial communication
- **NumPy** – numerical operations

## Requirements

- Python 3.9 or later
- A computer running Windows, Linux, or macOS
- For hardware acquisition: a device that sends signal data over a serial connection

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/SignalScope.git
   cd SignalScope
   ```

2. (Recommended) Create and activate a virtual environment:

   **Windows**
   ```bash
   python -m venv .venv
   .venv\\Scripts\\activate
   ```

   **Linux / macOS**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Run the Application

Save the main Python file as `signalscope.py`, then run:

```bash
python signalscope.py
```

If you keep a different filename, replace `signalscope.py` with that filename.

## Usage

1. Launch SignalScope.
2. Select the appropriate serial port and configure the connection settings for your hardware.
3. Connect to the device to receive live serial data.
4. Use the demo/simulation option to test the plotting interface without hardware, if available in your version.
5. Start recording to collect samples and stop recording when finished.
6. Export the recorded data to CSV for further processing.
7. Use the plot capture option to save an image of the displayed signal.

> **Note:** The serial data format and connection settings must match the firmware running on the connected microcontroller. Check your device firmware and the application code if incoming data is not displayed correctly.

## Project Structure

```text
SignalScope/
├── signalscope.py
├── README.md
├── requirements.txt
└── .gitignore
```

## Applications

SignalScope can be used as a lightweight tool for:
- Monitoring sensor output during embedded-system development.
- Visualizing biomedical or other time-series signals.
- Recording serial data for offline analysis.
- Testing signal acquisition workflows using simulated data.

## Future Improvements

- Support for multiple signal channels.
- Configurable sampling and filtering options.
- Additional signal-processing and analysis tools.
- More export formats and session management.

## Author

**Harrshan S**

Biomedical Engineering | Embedded Systems | Signal Processing



---

*SignalScope is an engineering and signal-visualization project. It is intended for development, experimentation, and educational use, not for clinical diagnosis.*
