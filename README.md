# 🤖 SCAN-AI — Real-Time AI Object Detection

> Detect and visualize objects in a live camera feed directly in your browser using machine learning and JavaScript.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![ml5.js](https://img.shields.io/badge/ML5.js-Machine%20Learning-blue)
![License](https://img.shields.io/badge/License-Not%20Specified-lightgrey)

## 📖 Overview

**SCAN-AI** is a browser-based object detection project built with HTML, CSS, and JavaScript. It uses **ml5.js** and the COCO-SSD object detection model to identify objects in a live video stream.

The application provides a camera-based interface with an AI toggle and a frames-per-second (FPS) control, allowing users to explore real-time object detection through a simple web interface.

No dedicated backend server is required by the current project structure.

🔗 **GitHub Repository:** [pratikabhang/SCAN-AI](https://github.com/pratikabhang/SCAN-AI)

## ✨ Features

- **Real-Time Object Detection:** Uses the COCO-SSD model through ml5.js to detect supported objects in a video stream.
- **Browser-Based Camera Input:** Uses the browser's video capabilities for live input.
- **Detection Visualization:** Provides a canvas for displaying detection results.
- **AI Toggle:** Includes a control for enabling or disabling AI detection.
- **FPS Control:** Offers a slider to adjust the target detection frame rate.
- **Lightweight Frontend:** Uses standard HTML, CSS, and JavaScript without a dedicated backend.
- **Simple Interface:** Uses Materialize CSS for interface styling.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Defines the application structure and video element |
| CSS3 | Styles the interface and video display |
| JavaScript | Controls the video feed and detection workflow |
| [ml5.js](https://ml5js.org/) | Provides a browser-friendly machine learning interface |
| COCO-SSD | Performs object detection on video frames |
| [Materialize CSS](https://materializecss.com/) | Provides interface styling and UI components |
| HTML Canvas | Displays the video detection output |

## 🏗️ How It Works

```text
          Browser
             |
             v
       Camera / Video
             |
             v
       Video Processing
             |
             v
      ml5.js ObjectDetector
             |
             v
        COCO-SSD Model
             |
             v
      Detection Results
             |
             v
      Canvas Visualization
```

1. The browser loads the HTML page and required JavaScript libraries.
2. The application initializes the ml5.js object detector.
3. The COCO-SSD model loads.
4. The video processing script accesses the video stream.
5. The detector processes video frames and returns object predictions.
6. The application visualizes detection results on the canvas.

Camera access requires user permission and may require HTTPS or a supported local development environment.

## 📂 Project Structure

```text
SCAN-AI/
├── index.html    # Main application interface and model initialization
├── style.css     # Page layout and styling
├── video.js      # Video handling and object detection logic
├── .gitignore    # Git ignore rules
└── .gitattributes
```

## 💻 Prerequisites

- A modern web browser, such as Chrome, Firefox, or Edge.
- An available camera if using live video input.
- An internet connection to load the externally hosted ml5.js and Materialize libraries.
- A local HTTP server for reliable browser camera access.

No Python, Node.js, database, or backend framework is required for the basic static application.

## 🚀 Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/pratikabhang/SCAN-AI.git
cd SCAN-AI
```

### 2. Run a Local HTTP Server

If Python is installed, run:

```bash
python -m http.server 8000
```

Alternatively, use:

```bash
python3 -m http.server 8000
```

### 3. Open the Application

Navigate to:

[http://localhost:8000](http://localhost:8000)

The browser should load `index.html`.

### 4. Allow Camera Access

If prompted, grant camera permission. Wait for the object detection model to finish loading before interacting with the detection controls.

If the camera does not start, check browser permissions and the developer console for errors.

## ▶️ Usage

1. Open the application in your browser.
2. Allow camera access when requested.
3. Wait for the COCO-SSD model to load.
4. Use the AI control to enable or disable detection.
5. Adjust the FPS slider to change the target processing rate.
6. Observe the video and canvas output as the detector identifies supported objects.

Actual detection performance depends on the device, browser, camera input, and model initialization time.

## ⚙️ Dependencies

The current HTML file references external libraries:

- **ml5.js 0.12.2:** Loaded from the unpkg CDN.
- **Materialize CSS 1.0.0:** Loaded from cdnjs.

Because these dependencies are loaded externally, an internet connection is needed unless the libraries are downloaded and configured locally.

For better long-term reliability, consider pinning and reviewing dependency versions before deployment.

## 🔐 Privacy and Security

- Camera access is subject to browser permissions.
- Avoid using camera feeds containing sensitive information.
- Review external library dependencies before using the application in a sensitive environment.
- Serve the application over HTTPS when deploying it publicly.
- Do not assume that all browser-side processing guarantees privacy; verify the behavior of any additional libraries or services you introduce.

## 🔮 Future Enhancements

Potential improvements include:

- Add explicit object labels and confidence scores to detection overlays.
- Improve camera selection and error handling.
- Add a responsive interface for mobile devices.
- Provide clearer model-loading and camera-status messages.
- Optimize detection scheduling and FPS handling.
- Add support for image uploads in addition to live video.
- Add automated tests for the video and detection workflow.
- Bundle dependencies locally for offline use.

These are proposed enhancements, not claims about existing functionality.

## 🤝 Contributing

Contributions and improvements are welcome.

1. Fork the repository.
2. Clone your fork:

   ```bash
   git clone https://github.com/<your-username>/SCAN-AI.git
   cd SCAN-AI
   ```

3. Create a feature branch:

   ```bash
   git checkout -b feature/your-feature-name
   ```

4. Make your changes in `index.html`, `style.css`, or `video.js`.
5. Test the application in a browser with camera access enabled.
6. Commit your changes:

   ```bash
   git add .
   git commit -m "Improve object detection interface"
   ```

7. Push the branch:

   ```bash
   git push origin feature/your-feature-name
   ```

8. Open a pull request describing your changes and testing performed.

## 📄 License

No repository-wide license has been confirmed. Until a `LICENSE` file is added, do not assume that the project's source code may be freely redistributed or reused.

## 👨‍💻 Author

**Pratik Abhang**

- GitHub: [@pratikabhang](https://github.com/pratikabhang)
- Repository: [SCAN-AI](https://github.com/pratikabhang/SCAN-AI)

---

⭐ If you find this project useful, consider starring the repository.

*Explore computer vision. Experiment with machine learning. Build with AI.*
