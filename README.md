# ayn-ai

**ayn-ai** is an intelligent real-time video analysis system that captures RTSP camera streams, detects and stores human faces, and is designed to support additional vision features like license plate recognition.

---

## 🧠 Project Idea

A modular vision system that connects to one or more IP cameras, analyzes video frames in real-time, detects human faces, and stores them with metadata (timestamp, camera ID). Future extensions include license plate recognition and smart alerts.

---

## 🔍 Features

- Connect to RTSP camera streams
- Detect faces in real-time
- Save face images with timestamp & camera ID
- REST API for image retrieval and search
- Frontend UI for monitoring and searching faces
- Future support: License plate detection, face matching, alerting

---

## 🧰 Tech Stack

| Component       | Technology                              |
| --------------- | --------------------------------------- |
| Frontend        | React (Vite, TypeScript)                |
| Backend         | Node.js (Express)                       |
| Face Detection  | face-api.js / OpenCV                    |
| Database        | PostgreSQL                              |
| Video Input     | RTSP + OpenCV                           |
| Future Features | License plate detection (OpenALPR/YOLO) |

---

## 📁 Project Structure (Planned)

```
ayn-ai/
├── backend/
│   ├── controllers/
│   ├── routes/
│   ├── services/
│   └── index.ts
├── face-detector/
│   ├── cameraReader.ts
│   └── faceRecognizer.ts
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   └── App.tsx
│   ├── public/
│   └── vite.config.ts
├── database/
│   └── schema.sql / connection.ts
├── public/
│   └── faces/
├── README.md
```

---

## 📝 API Endpoints
			
| Endpoint           | Method  | Description                                                  |
| ------------------ | ------- | ------------------------------------------------------------ |
| /api/faces         | GET     | Retrieve all stored faces                                    |
| /api/faces/:id     | GET     |Retrieve a specific face by ID                                |
| /api/faces/search  | GET     |Search for faces based on timestamp, camera, etc.             |
| /api/faces/upload  | POST    |Upload new face image with metadata (timestamp, camera ID)    |
| /api/platesVideo   | GET     |Retrieve stored license plates (future feature)               |
| /api/plates/upload | POST    |Upload new license plate image (future feature)               |

---

## 🚀 Getting Started (Soon)

1. Clone the repo
2. Install backend & frontend dependencies
3. Configure camera URL and database
4. Run the face detector, backend server, and frontend UI

---

## 📌 Notes

- Diagrams and documentation will guide development
- Frontend will visualize face captures and allow searching by date/time/camera

---

## 📸 Sample Use Cases

- Security surveillance
- Smart attendance systems
- Real-time visitor tracking

---

## License

MIT License

---

> Developed with clarity and vision 🧠👁️ by [Yousef Qawasmeh]

