# GSoc-AirMashup

✈️ AirMashup: Immersive Flight Tracking for Liquid Galaxy

AirMashup is an innovative, real-time aeronautical visualization platform specifically engineered for the Liquid Galaxy multi-display rig. By bridging the gap between live global flight data and large-scale interactive displays, it provides a 180-degree panoramic tracking experience that traditional 2D maps cannot match.


🌟 Key Features
Live Global Tracking: Fetches real-time state vectors (latitude, longitude, altitude) via the OpenSky Network API.
AI Voice Assistant: Integrated NLP for hands-free navigation (e.g., "Fly to flight UAE501" or "Track aircraft over London").

Panoramic Visualization: Custom KML generation engine optimized for 5-screen/3-screen Liquid Galaxy setups.
SSH Connectivity: Secure, low-latency communication between the Flutter mobile controller and the Master Node.
Telemetry Dashboard: Real-time data cards showing aircraft velocity, heading, and origin/destination status.


🛠️ Tech Stack

Framework: Flutter (Dart)

API: OpenSky Network (REST)

Communication: SSH2 / SFTP for KML transmission

Visualization: Google Earth / KML Engine

State Management: Provider / Riverpod


📂 Project Architecture

air_mashup/

├── assets/               # KML templates, Icons, and Images

├── lib/                  # Main Application Logic

│   ├── api/              # OpenSky Network API integration

│   ├── models/           # Flight & Telemetry Data Models

│   ├── services/         # SSH Client & KML Generation logic

│   ├── ui/               # Neon-Aviation Theme Screens & Widgets

│   └── main.dart         # App Entry Point

├── pubspec.yaml          # Project Dependencies

└── README.md             # Project Documentation

🚀 Getting Started
  1. clone the repo :
      https://github.com/Yashvendrasahu/GSoc-AirMashup/tree/main
  2. install dependencies
     flutter pub get
  3.Configure SSH:
     Go to Settings -> SSH Configuration and enter your Liquid Galaxy Master Node credentials.
  4. run the app
     flutter run
     
🤝 Acknowledgments

Special thanks to the Liquid Galaxy Organization and mentors for the inspiration and support in building immersive geospatial tools.
