# 🚀 AirMashup: Immersive Flight Tracking for Liquid Galaxy

**Real-time aeronautical visualization platform engineered for next-generation multi-display systems**

---

## 📋 Overview

AirMashup is an innovative, real-time flight tracking and visualization platform specifically engineered for the **Liquid Galaxy multi-display rig**. By seamlessly bridging live global flight data with large-scale interactive panoramic displays, it delivers an immersive 180-degree tracking experience that transcends traditional 2D mapping solutions.

Whether you're an aviation enthusiast, a geospatial analyst, or exploring immersive technologies, AirMashup provides an unparalleled way to explore global aviation in real-time.

---

## ✨ Key Features

- **🌍 Live Global Flight Tracking**  
  Real-time state vectors (latitude, longitude, altitude, velocity) fetched via the OpenSky Network API

- **🎙️ AI Voice Assistant**  
  Integrated NLP engine for hands-free navigation  
  *Examples: "Fly to flight UAE501" • "Track aircraft over London"*

- **🖼️ Panoramic Visualization**  
  Custom KML generation engine optimized for 5-screen and 3-screen Liquid Galaxy configurations

- **🔒 Secure SSH Connectivity**  
  Low-latency, encrypted communication between the Flutter mobile controller and Master Node

- **📊 Telemetry Dashboard**  
  Real-time data visualization showing aircraft velocity, heading, origin, and destination status

---

## 🛠️ Technology Stack

| Component | Technology |
|-----------|-----------|
| **Framework** | Flutter (Dart) |
| **Flight Data API** | OpenSky Network (REST) |
| **Communication** | SSH2 / SFTP |
| **Visualization Engine** | Google Earth / KML |
| **State Management** | Provider / Riverpod |
| **Language** | 100% Dart |

---

## 📂 Project Architecture

```
air_mashup/
├── assets/                    # KML templates, Icons, and Images
├── lib/                       # Core Application Logic
│   ├── api/                   # OpenSky Network API integration
│   ├── models/                # Flight & Telemetry Data Models
│   ├── services/              # SSH Client & KML Generation
│   ├── ui/                    # UI Screens & Widgets (Neon-Aviation Theme)
│   ├── providers/             # State Management (Provider/Riverpod)
│   └── main.dart              # Application Entry Point
├── pubspec.yaml               # Project Dependencies
├── .gitignore
└── README.md                  # Documentation
```

---

## 🚀 Getting Started

### Prerequisites
- Flutter SDK (v3.0+)
- Dart SDK (v3.0+)
- Liquid Galaxy Master Node (SSH-enabled)
- OpenSky Network API credentials (free tier available)

### Installation

**1. Clone the Repository**
```bash
git clone https://github.com/Yashvendrasahu/GSoc-AirMashup.git
cd air_mashup
```

**2. Install Dependencies**
```bash
flutter pub get
```

**3. Configure SSH Credentials**
- Launch the app
- Navigate to **Settings → SSH Configuration**
- Enter your Liquid Galaxy Master Node credentials:
  - Host IP address
  - SSH username & password
  - KML output directory path

**4. Run the Application**
```bash
flutter run
```

---

## 📖 Usage Guide

### Tracking a Flight
1. Enter a flight ICAO code or airline flight number
2. Press "Search" or use voice command
3. Watch real-time flight data render on your Liquid Galaxy display

### Voice Commands
- *"Fly to flight UAE501"*
- *"Track aircraft over London"*
- *"Show me all flights at 35,000 feet"*
- *"Pause tracking"*

---

## 🔧 Configuration

### Environment Variables
Create a `.env` file in the project root:
```
OPENSKY_API_USERNAME=your_username
OPENSKY_API_PASSWORD=your_password
```

### Liquid Galaxy Setup
Ensure your Master Node:
- Has SSH enabled and publicly accessible
- Has sufficient disk space for KML files (recommended: 1GB+)
- Supports SFTP protocol

---

## 📱 Project Structure Details

| Module | Purpose |
|--------|---------|
| `api/` | Handles OpenSky Network REST calls and flight data parsing |
| `models/` | Dart models for Aircraft, Flight, and Telemetry data |
| `services/` | SSH/SFTP client and KML generation engine |
| `ui/` | Flutter widgets and screens with Neon-Aviation design theme |
| `providers/` | State management and reactive data streams |

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

---

## 📝 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Liquid Galaxy Organization** – For the inspiring multi-display platform
- **OpenSky Network** – For providing real-time flight data
- **GSoC Mentors** – For guidance and support
- **Flutter Community** – For comprehensive documentation and packages

---

## 📞 Contact & Support

- **GitHub Issues**: [Report bugs or request features](https://github.com/Yashvendrasahu/GSoc-AirMashup/issues)
- **Author**: [Yashvendrasahu](https://github.com/Yashvendrasahu)

---

**Made with ✈️ and ❤️ for aviation enthusiasts and geospatial innovators**