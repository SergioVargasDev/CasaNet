# CasaNet: Smart Home Energy Management System

CasaNet is a web-based energy management platform designed to optimize household energy consumption through IoT integration and real-time monitoring. Built with sustainability at its core, the system delivers actionable insights to help users reduce energy waste while maintaining comfort and convenience. CasaNet achieves a projected 23% reduction in energy usage through AI-powered recommendations and supports SDG 11 for Sustainable Cities and Communities.

## Features

- **Real-Time Energy Monitoring**: Live tracking of household energy consumption in kWh with instant cost calculations and usage analytics.
- **IoT Sensor Integration**: Arduino and NodeMCU (ESP8266) hardware for precise flash-count tracking through photoresistor sensors.
- **Smart Analytics Dashboard**: Interactive web interface displaying energy trends, historical data, and consumption patterns.
- **AI-Powered Recommendations**: OpenAI and machine learning integration providing personalized energy-saving suggestions.
- **Sustainability Education**: Environmental impact insights and user education on energy consumption behaviors.
- **Cost Optimization**: Real-time cost calculations and budget tracking for informed energy management decisions.

## Tech Stack

### Frontend
- **HTML5 & CSS3** – Responsive web interface with modern design principles for optimal user experience.
- **JavaScript** – Interactive dashboard functionality and real-time data visualization.

### Backend & Database
- **Firebase** – Secure, scalable cloud storage with real-time database synchronization and user authentication.

### Hardware Integration
- **Arduino & NodeMCU (ESP8266)** – Microcontroller platform for IoT connectivity and sensor data processing.
- **Photoresistor Sensor** – Light detection system for accurate energy meter flash counting and consumption tracking.

### AI Integration
- **OpenAI API** – Advanced language model integration for intelligent energy recommendations and user insights.
- **Machine Learning Models** – Predictive analytics for consumption patterns and optimization strategies.

## Installation

### Prerequisites

- **Node.js 16.0+** - Required for development tools and package management
- **Arduino IDE** - For hardware programming and sensor calibration
- **Firebase Account** - For cloud database and authentication services

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-org/casanet.git
   cd casanet
   ```

2. **Web Application Setup**
   ```bash
   # Install dependencies
   npm install
   
   # Configure environment variables
   cp .env.example .env
   # Add your Firebase credentials and OpenAI API key
   
   # Start development server
   npm run dev
   ```

3. **Hardware Configuration**
   ```bash
   # Upload Arduino code to NodeMCU
   # Connect photoresistor sensor to designated pins
   # Configure WiFi credentials in hardware setup
   ```

4. **Firebase Configuration**
   ```javascript
   // Initialize Firebase in your project
   import { initializeApp } from 'firebase/app';
   import { getDatabase } from 'firebase/database';
   
   const firebaseConfig = {
     // Your Firebase configuration
   };
   ```

5. **Access the platform**
   - Open your web browser and navigate to: `http://localhost:3000`
   - The dashboard will load with real-time energy monitoring and analytics

### System Configuration

The platform can be customized through the admin interface:

- **Sensor Calibration**: Adjust photoresistor sensitivity and flash detection parameters
- **Cost Settings**: Configure local energy rates and billing preferences  
- **AI Parameters**: Fine-tune machine learning models for personalized recommendations
- **Alert Thresholds**: Set consumption limits and notification preferences

### File Structure

```
casanet/
├── frontend/
│   ├── src/
│   │   ├── components/     # Web interface components
│   │   ├── pages/          # Dashboard and analytics pages
│   │   └── utils/          # API calls and helper functions
├── hardware/
│   ├── arduino/            # NodeMCU and sensor code
│   ├── calibration/        # Sensor setup and testing
│   └── schematics/         # Hardware connection diagrams
├── backend/
│   ├── firebase/           # Cloud functions and database rules
│   ├── ai/                 # OpenAI integration and ML models
│   └── api/                # Data processing and analytics
└── README.md               # This file
```

### Running Different Components

#### 1. Development Mode
```bash
# Start web application
npm run dev

# Monitor hardware logs
npm run hardware:monitor

# Test sensor connectivity
npm run sensor:test
```

#### 2. Production Deployment
```bash
# Build web application
npm run build

# Deploy to Firebase Hosting
firebase deploy

# Update hardware firmware
npm run hardware:update
```

#### 3. System Monitoring
```bash
# Check sensor status
npm run status:sensors

# View real-time data
npm run monitor:realtime

# Generate analytics report
npm run analytics:report
```

### Platform Controls

Once the system is running:

1. **Hardware Setup**: Connect NodeMCU to household energy meter and configure WiFi
2. **Dashboard Access**: Real-time energy monitoring and consumption analytics
3. **AI Insights**: Personalized recommendations based on usage patterns
4. **Cost Tracking**: Live cost calculations and budget management
5. **Sustainability Metrics**: Environmental impact tracking and education
6. **Alert System**: Automated notifications for unusual consumption patterns

### Hardware Integration

For optimal sensor performance:

1. **Photoresistor Placement**: Position sensor to detect energy meter light flashes accurately
2. **Calibration Process**: Fine-tune sensitivity for precise flash counting
3. **Network Configuration**: Ensure stable WiFi connectivity for real-time data transmission
4. **Power Management**: Optimize NodeMCU power consumption for continuous operation

### Troubleshooting

**Common Issues:**

- **Sensor not detecting flashes**: Check photoresistor positioning and lighting conditions
- **WiFi connectivity problems**: Verify network credentials and signal strength
- **Data sync issues**: Confirm Firebase configuration and internet connectivity
- **Inaccurate cost calculations**: Update local energy rates in system settings

**Performance Optimization:**

- Implement data caching for improved dashboard responsiveness
- Optimize sensor reading intervals for battery efficiency
- Use Firebase real-time listeners for instant data updates
- Monitor API usage limits for OpenAI integration

### Impact & Results

CasaNet demonstrates significant potential for household energy optimization:

- **23% projected reduction** in energy usage through AI-powered recommendations
- **Real-time accuracy** in energy consumption tracking and cost calculations
- **Seamless IoT integration** with household energy infrastructure
- **User education impact** promoting sustainable energy behaviors
- **SDG 11 alignment** supporting sustainable cities and communities

The system successfully integrates advanced technologies including IoT sensors, cloud computing, and artificial intelligence to create a comprehensive energy management solution that balances efficiency, comfort, and environmental responsibility.
