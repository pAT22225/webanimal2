#Wildlife Guardian AI 🇵🇭🐾

A Web-Based Intelligent System for Real-Time Detection and Health Awareness of Endangered Birds and Mammals in the Philippines Using Machine Learning

## Features

Real-Time Wildlife Detection
Detect endangered birds and mammals using image, video, or live camera input powered by YOLOv8.

Health Risk Awareness Module
Identifies visible signs of:

Injury (e.g., wounds, swelling, bleeding)

Malnutrition (e.g., thin body frame, poor feather/fur quality)

Healthy condition

- Species Information Display
- Automatically retrieves and displays:
- Common and scientific name
- Conservation status
- Estimated population
- Habitat
- Estimated lifespan
- Detected health condition
- Endangered Species Alerts
- Notifies users when an endangered species is detected.
- Educational Awareness Module
- Provides species profiles and conservation facts to encourage wildlife advocacy.

User-Friendly Web Interface
Accessible on desktops, tablets, and mobile devices through modern web browsers.
## Technical Stack

- **Frontend**: Next.js, React, Tailwind CSS
- **Backend / API**: Python (Flask) with RESTful API architecture
- **Machine Learning**: YOLOv8 (CNN-based object detection)
- **Database**: MySQL (via SQLAlchemy ORM)
- **Data Visualization**: Chart.js for analytics dashboards
- **Live Camera Input**: Browser-based camera capture
- **Authentication**: JWT-based authentication
- **Cloud Storage**: Server-side storage for uploaded images and videos

## How to Run the System

### Prerequisites

- Node.js (v16.x or later)
- npm (v7.x or later)
- A modern web browser (Chrome, Firefox, Edge, or Safari)

### Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/wildlife-guardian-ai.git
   cd wildlife-guardian-ai
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Create necessary directories**
   ```bash
   mkdir -p public/images/endangered
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Access the application**
   Open your browser and navigate to [http://localhost:3000](http://localhost:3000)

### Using the Wildlife Detection Feature

1. Navigate to "Wildlife Detection" in the main menu
2. Upload an image or use one of the test images
3. Click "Detect Animals" to process the image
4. View detected animals and their confidence scores
5. If endangered species are detected, you'll receive a special alert

### Using Video Analysis

1. Go to the "Video Analysis" section
2. Upload a wildlife video file (MP4, AVI, MOV formats supported)
3. The system will process the video frame-by-frame
4. View a timeline of detected animals with timestamps
5. Export detection data as CSV or JSON for further analysis

### Setting up Live Camera Monitoring

1. Navigate to "Live Monitoring" in the dashboard
2. Select "Add Camera Source" and choose from:
   - Webcam: Direct browser access
   - IP Camera: Enter RTSP stream URL
   - CCTV System: Configure API integration
3. Set detection sensitivity and notification preferences
4. Start monitoring to receive real-time alerts

### Exploring Global Wildlife Data

1. Access the "Global Tracking" section
2. View the interactive map showing recent wildlife sightings
3. Filter by species, conservation status, or region
4. See real-time statistics on detection trends
5. Contribute your own sightings to the global database

### Real-time Analytics Dashboard

1. Go to the "Analytics" section
2. View interactive charts showing:
   - Species distribution
   - Endangered animal sightings over time
   - Conservation hotspots
   - Detection accuracy metrics
3. Set up custom alerts for specific regions or species

### Running in Production Mode

For production deployment:

1. **Build the application**
   ```bash
   npm run build
   ```

2. **Start the production server**
   ```bash
   npm start
   ```

## Troubleshooting

- **Model Loading Issues**: If the AI model fails to load, check your internet connection as it requires downloading the model files.
- **Image Detection Problems**: Ensure your images are clear and well-lit for best results.
- **Browser Compatibility**: The application works best on modern browsers with WebGL support.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
