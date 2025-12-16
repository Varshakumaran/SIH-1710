# Smart India Hackathon Workshop
# Date: 16-12-2025
## Register Number: 212223220122
## Name: varsha k
## Problem Title
SIH 1710: Enhancing Navigation for Railway Station Facilities and Locations
## Problem Description
Background: Railway stations are complex environments with numerous facilities and locations such as ticket counters, platforms, restrooms, food courts, and waiting areas. Passengers often face difficulties in navigating these spaces, especially in large or unfamiliar stations. Efficient and user-friendly navigation systems are crucial for improving passenger experience, reducing congestion, and ensuring timely travel connections. Description: The problem involves developing a comprehensive navigation solution for railway stations that assists passengers in locating various facilities and destinations within the station premises. This includes creating detailed maps, providing real-time directions, and integrating features such as accessibility options for individuals with disabilities. The solution should be intuitive, easy to use, and accessible via multiple platforms, including mobile devices and digital kiosks. Key challenges include updating navigation information in real-time, ensuring accuracy, and accommodating the diverse needs of all passengers. Expected Solution: The expected solution is a multi-platform navigation system that provides detailed, real-time directions to all facilities and locations within a railway station. This system should include: A mobile application with 3D interactive maps and step-by-step navigation. Digital kiosks located throughout the station with touch-screen interfaces. Voice-guided navigation for visually impaired passengers. Regular updates to reflect changes in station layout and facility locations. Integration with existing railway apps and services for seamless user experience. The solution should enhance the overall passenger experience by reducing confusion, saving time, and improving accessibility within the station.

## Problem Creater's Organization
Ministry of Railway

## Idea
Enhancing Navigation for Railway Station Facilities and Locations

## Proposed Solution / Architecture Diagram
RailWayFinder uses Bluetooth Low Energy (BLE) beacons and an AI-based path engine to enable accurate indoor navigation inside railway stations without GPS.
BLE Beacons are installed at key station locations.

The mobile app detects nearby beacons to identify the passenger’s indoor position.

The AI Path Engine calculates the best route using station layout and crowd data.

Real-time directions are shown on the app or played as voice instructions.

Station admins update layouts and alerts using a web dashboard.

<img width="1536" height="1024" alt="64693dd4-82cc-4566-b643-b608f0d2b3ed" src="https://github.com/user-attachments/assets/48c6d108-31df-4fd6-a436-2ed861f26197" />

## Use Cases
## Passenger Use Cases

Find the shortest route to platforms, exits, or facilities

Get voice-guided navigation inside the station

Receive alerts for platform changes

Access wheelchair-friendly routes

Navigate without internet (cached maps)
## Station Admin Use Cases

Update station layout digitally

Enable or disable routes during maintenance

Monitor crowd density

Send emergency or rerouting alerts
## Accessibility Use Cases

Voice navigation for visually impaired passengers

Vibration-based directions for hearing impaired

Elevator-only routing for wheelchair users

## Technology Stack
Layer	-Technology
Mobile Application-Flutter / Kotlin
Beacon Communication-	Bluetooth Low Energy (BLE 5.0)
Backend - API	FastAPI / Node.js
Database-	Neo4j (Graph DB)
Real-time- Data	Firebase
Admin Dashboard	React.js
Voice Guidance-	Text-to-Speech APIs
AI Path Logic	Dijkstra + ML Optimization

## Dependencies
## Mobile App Dependencies

flutter_blue_plus – BLE scanning

provider – State management

text_to_speech – Voice navigation

path_provider – Offline map storage
## Backend Dependencies

fastapi – API framework

uvicorn – Server runtime

neo4j-driver – Graph database connection

firebase-admin – Real-time updates
## Admin Dashboard Dependencies

react – UI framework

axios – API communication

chart.js – Crowd analytics

leaflet – Indoor map visualization
