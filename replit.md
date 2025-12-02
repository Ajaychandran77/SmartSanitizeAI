# SmartSanitizeAI - Smart City Waste & Toilet Hygiene Monitoring System

## Overview
SmartSanitizeAI is a futuristic, feature-rich frontend application for smart city waste management and toilet hygiene monitoring. Built with a modern glassmorphism UI design, it provides citizens with tools to report waste issues and toilet hygiene problems to local municipalities.

## Current State
- **Version**: 1.0 (MVP)
- **Status**: Fully functional frontend with Flask backend serving static files
- **Last Updated**: December 2024

## Project Architecture

### File Structure
```
SmartSanitizeAI/
├── app.py                 # Flask backend (serves static files)
├── templates/
│   └── index.html         # Main HTML file with all sections
├── static/
│   ├── style.css          # Comprehensive CSS with glassmorphism, neon effects
│   └── script.js          # All JavaScript functionality
├── .gitignore
└── replit.md              # This file
```

### Technology Stack
- **Backend**: Flask (Python) - minimal server to serve static files
- **Frontend**: 
  - HTML5, CSS3, Vanilla JavaScript
  - Leaflet.js for interactive mapping
  - Google Fonts (Poppins, Inter)
- **APIs Used**:
  - Browser Geolocation API
  - Nominatim (OpenStreetMap) for reverse geocoding
  - Various tile providers for map layers

## Core Features

### 0. About Page (Home)
- Hero section with animated gradient background
- Project inspiration and motivation
- What the system does (workflow overview)
- Technology stack showcase
- Challenges faced during development
- Accomplishments and achievements
- Learning outcomes
- Future roadmap and vision

### 1. Location Detection
- Automatic GPS location detection
- Animated "Locating..." indicator
- Reverse geocoding for address display
- Manual marker placement fallback

### 2. Interactive Map (Leaflet.js)
- Dark, Light, and Satellite tile layers
- Pulsing user location marker
- Route drawing to municipalities
- Recenter button

### 3. Street Waste Reporting
- Drag-and-drop image upload
- Real-time image preview with metadata
- Simulated AI severity scoring (0-100)
- Confidence meter
- Waste type tags
- Category selection buttons

### 4. Toilet Hygiene Scoring
- Image upload with drag-and-drop
- Simulated AI cleanliness score
- Hygiene rating badges (Excellent/Good/Needs Cleaning/Critical)
- Detailed breakdown metrics:
  - Floor cleanliness
  - Seat cleanliness
  - Wall condition
  - Odor level
  - Water spill level
- Low score alert with report button

### 5. Municipality Finder
- Local dataset of municipalities
- Haversine distance calculation
- Sorted by nearest
- Contact details (email, phone)
- Route visualization on map

### 6. Smart Dashboard
- Total reports counter
- Cleanup success rate
- Average waste severity
- Average hygiene score
- Weekly reports bar chart (Canvas)
- Severity trends line chart (Canvas)

### 7. Theme Switcher
- Dark mode (default)
- Light mode
- Smooth animated transitions

### 8. Toast Notifications
- Success, Error, Warning types
- Neon glow effects
- Auto-dismiss

### 9. Floating Chatbot (SanitizeBot)
- FAQ responses
- Typing indicator animation
- Smooth open/close transitions

## UI Design Elements
- Glassmorphism cards
- Neon green/blue/purple glows
- Poppins/Inter typography
- Card hover lift effects
- Pulsing animations
- Fully responsive layout

## Running the Application
```bash
python app.py
```
The application runs on port 5000.

## Future Enhancements (Next Phase)
1. Real computer vision API integration for waste/hygiene classification
2. Backend database for persisting reports and images
3. Real municipality API with live contact info
4. User authentication system
5. Report management with status tracking
6. Admin dashboard for municipality officials

## User Preferences
- Modern, futuristic UI aesthetic
- Dark mode as default theme
- Hackathon-ready visual design
- No external charting libraries (uses Canvas)
