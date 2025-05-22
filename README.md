# Camera-Control-Panels-application
-------

This is a web-based Camera Control Panels application built using **Java (Spring Boot)** for the backend and **HTML, CSS, JavaScript** for the frontend.

The application allows users to:

- Enter IP address and port number to connect to a camera.
- Navigate to the camera control panel once the connection is successful.
- Interact with camera control buttons (e.g., pan, tilt, zoom).
- Trigger specific messages or actions on button clicks (e.g., "Other Controls" button).

---

## 🔧 Technologies Used

- **Backend**: Java, Spring Boot
- **Frontend**: HTML, CSS, JavaScript
- **Build Tool**: Maven / Gradle
- **Browser**: Chrome, Firefox, Edge (any modern browser)

---

## 🚀 How It Works

1. **Startup Page**:
   - User is prompted to enter the **IP address** and **Port number**.
   - On valid connection, user is navigated to the **Camera Controls** page.

2. **Camera Controls Page**:
   - Displays a set of control buttons (15–16 total).
   - Buttons may include: Zoom In, Zoom Out, Pan Left, Pan Right, Tilt Up, Tilt Down, etc.
   - Clicking the **Other Controls** button will print:  
     ```
     Other controls button clicked
     ```

---

## 📁 Project Structure

````

camera-control-app/
│
├── backend/
│   └── src/
│       └── main/
│           └── java/com/yourcompany/cameracontrol/
│               ├── CameraController.java
│               ├── ConnectionService.java
│               
│
├── frontend/
│   ├── index.html       // IP & Port Input Page
│   ├── style.css
│   └── script.js
│
├── README.md
└── pom.xml or build.gradle

````

---

## 🛠️ Setup & Run Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/camera-control-app.git
cd camera-control-app
````

### 2. Run the Backend (Spring Boot)

```bash
cd backend
./mvnw spring-boot:run
```

### 3. Serve the Frontend

Open `frontend/index.html` in your browser directly, or use a simple static server like:

```bash
cd frontend
python3 -m http.server 8081
```

### 4. Usage

* Open `http://localhost:8081` in your browser.
* Enter the camera **IP** and **Port** and click **Connect**.
* On success, you’ll be redirected to the **Controls** page.
* Click on any button, including the **Other Controls** button to see console messages.

---

## 📝 Example Output

```bash
Connecting to IP: 192.168.1.10, Port: 8080
Connection successful!
Navigating to Camera Controls Page...

# On clicking Other Controls
Other controls button clicked
```

---
