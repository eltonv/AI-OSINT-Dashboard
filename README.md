# AI-OSINT-Dashboard

### Overview
AI-OSINT-Dashboard is an open-source, real-time geographic dashboard for visualizing OSINT data. The dashboard integrates AI/ML models for object detection, NLP-based analytics, and anomaly detection, while leveraging edge AI devices for efficiency. It provides a map-based interface to correlate geospatial data, camera feeds, and text feeds in real time.

---

### Technologies
- **Backend**: Node.js (Express.js), MongoDB
- **Frontend**: React.js, CesiumJS, Leaflet.js
- **Edge AI Models**: TensorFlow Lite, YOLOv8 (Ultralytics), Hugging Face Transformers
- **Data Sources**: OpenStreetMap, public OSINT APIs (Twitter API, RSS feeds)

---

### Features
1. Real-time dashboard with 3D map layers.
2. Ingests camera feeds and performs object detection using edge devices (ESP32, Raspberry Pi).
3. OSINT APIs analyzed with sentiment tagging (e.g., Twitter, news RSS feeds).
4. Multi-layered data visualization:
   - Object Localization on Camera Feeds
   - Live Event Annotation from APIs (text NLP)
5. Secure and scalable backend APIs with real-time monitoring.

---

### File Structure
- **`/backend`**: REST API and backend services (API integration, database).
- **`/frontend`**: React dashboard and map visualization.
- **`/edge-ai`**: AI/ML pipelines and edge inference scripts.
- **`/resources`**: Datasets and learning resources.

---

### Getting Started
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/eltonv/AI-OSINT-Dashboard.git
   cd AI-OSINT-Dashboard
   ```

2. **Install Dependencies**:
   - Backend: `cd backend && npm install`.
   - Frontend: `cd frontend && npm install`.

3. **Run the Application**:
   - Start Backend: `npm start` (from `/backend`).
   - Start Frontend: `npm start` (from `/frontend`).

4. **Contribute**:
   - Check `roadmap.md` for issues and milestones.

---

### License
[MIT License](LICENSE)