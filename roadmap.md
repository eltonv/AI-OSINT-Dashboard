# Roadmap

### Phase 1: Core Backend Infrastructure
##### Goal: Build RESTful APIs for data ingestion.
1. **Set up Node.js backend**:
   - Create the base project with Express.js.
   - Configure MongoDB for storing and querying:
     - OSINT feeds + API results.
     - Camera feed metadata.
2. **Build APIs**:
   - Real-time OSINT ingestion (Twitter/NLP pipelines).
   - Endpoints to upload and store video feed metadata.
3. **Install Basic Security**:
   - HTTPS requests.
   - Rate-limit APIs against abuse.
4. **Tech Resources**:
   - [Node.js Guide](https://nodejs.dev/en/)
   - [MongoDB Geospatial Indexing](https://docs.mongodb.com/manual/geospatial-queries/)

### Phase 2: AI Pipelines (Edge AI + NLP)
##### Goal: Enable object detection / sentiment analysis.
1. **Object Detection**:
   - Train or fine-tune a YOLOv8 model (or use pretrained).
   - Optimize using TensorFlow Lite or ONNX for embedded deployment.
   - Create edge device scripts for ESP32 or Raspberry Pi.
2. **NLP Sentiment Analysis**:
   - Extract data from Twitter API or RSS feeds.
   - Perform sentiment tagging with Hugging Face models (DistilBERT, etc.).
   - Cluster OSINT data (e.g., DBSCAN in scikit-learn).
3. **Tech Resources**:
   - [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)
   - [Hugging Face NLP Models](https://huggingface.co/transformers)
   - [TensorFlow Lite Guide](https://www.tensorflow.org/lite)

### Phase 3: Dashboard Visualization
##### Goal: Visualize data on 3D/2D maps.
1. **Set Up CesiumJS or Leaflet**:
   - Display real-time camera feed locations.
   - Plot sentiment-tagged OSINT data with heatmaps.
2. **React.js Integration**:
   - Populate map with API data using React components.
   - Create a filtering system (by feed type, object, etc.).
3. **Tech Resources**:
   - [CesiumJS Documentation](https://cesium.com/learn/)
   - [Leaflet.js Documentation](https://leafletjs.com/examples/quick-start/)

### Phase 4: Deployment and QA
1. **Containerize Backend/AI**:
   - Use Docker to manage backend and ML pipelines.
   - Host on a free-tier cloud platform.
2. **Test**: Implement unit tests and CI/CD pipelines with GitHub Actions.
3. **Build a Demo**:
   - Host the dashboard (e.g., on Vercel).
4. **Tech Resources**:
   - [Docker Tutorial](https://docs.docker.com/get-started/)
   - [GitHub Actions CI/CD](https://docs.github.com/en/actions)