📦 EnRoute Delivery System (Walmart)
A smart, optimized delivery routing system designed for last-mile logistics at Walmart. This project combines efficient route planning, real-time tracking, and seamless integration with delivery operations—all tailored to enhance efficiency and customer satisfaction.

🧠 Table of Contents
🚀 Project Overview

🎯 Objectives

🏗️ Architecture & Components

🧩 Features

🔧 Tech Stack

🛠️ Setup & Installation

🚗 Usage / Workflow

📈 Performance & Enhancements

🌱 Contributing

⚖️ License

🚀 Project Overview
The EnRoute Delivery System is a complete logistics platform that:

Assigns and optimizes delivery routes for Walmart’s last-mile operations

Tracks delivery vehicles and packages in real time

Offers a dashboard interface for monitoring status, ETA, and delivery performance

Its modular design allows easy integration with existing fleet systems and scales for large volumes across service regions.

🎯 Objectives
Plan the shortest travel routes between dispatch center and delivery addresses

Balance vehicle load to ensure efficient capacity and cost management

Track ongoing deliveries and provide status updates

Visualize routes on an interactive map dashboard

Support scalability in service zones and delivery volume

🏗️ Architecture & Components
css
Copy
Edit
[Order Input API] → [Route Engine] → [Load Balancer] → [Vehicle Dispatch]
        ↓                      ↓                        ↓
  [Route Dashboard] ← [Realtime Tracker] ← [Mobile Tracking API]
Route Engine: Calculates optimized trips via Dijkstra / A*

Load Balancer: Uses Knapsack-based logic to fill vehicles

Tracker: Monitors vehicle GPS and displays status in the UI

Dashboard: Web dashboard to visualize route, progress, ETAs

🧩 Features
📊 Shortest Route Planning — real-time mapping across zones

📦 Dynamic Load Assignment — efficient use of fleet capacity

🚚 Live Tracking — pinpoint location & ETA for each vehicle

🗺️ Dashboard Visualization — traffic-aware route graphs

⚙️ Modular Design — easy to add new features or integrate APIs

🔧 Tech Stack
Backend: Java / Spring Boot (or your choice of stack)

Algorithms:

Shortest Paths: Dijkstra’s or A*

Load Allocation: Knapsack

Route Clustering: K-Means (optional)

Frontend: React + Leaflet or Mapbox for route visualization

Database: PostgreSQL + PostGIS for geospatial queries

APIs: HTTPS endpoints for orders and delivery updates

🛠️ Setup & Installation
Clone the repo

bash
Copy
Edit
git clone https://github.com/VimarshDwivedi/EnRoute_Delivery_system_walmart_.git
cd EnRoute_Delivery_system_walmart_
Backend

Import into your IDE or build CLI (e.g., ./gradlew build)

Configure application.properties with DB host, credentials, API keys

Database Setup

Initialize your Postgres DB with PostGIS

Run the provided SQL scripts: init_schema.sql, seed_delivery_zones.sql

Frontend

Navigate to the dashboard/ folder

Run npm install && npm start to launch the dashboard

Run Services

Start backend (java -jar app.jar)

Launch frontend on http://localhost:3000

🚗 Usage / Workflow
Create or import delivery orders via API or UI

Dispatcher uses dashboard → Generate Routes

System calculates routes + assigns to vehicles

Drivers use mobile app for navigation & status updates

Dashboard shows live vehicle movement & delivery progress

Completed deliveries are logged; dashboards show detailed metrics

📈 Performance & Enhancements
Current route planning supports up to 500 deliveries per zone

Scalability: horizontal scaling via microservices

Future plans:

Integrate traffic estimation (using public data)

Add driver ETA prediction via machine learning

Support multi-modal routing (e.g., drone + truck)

🌱 Contributing
Contributions are welcome! To add features or improvements:

Fork the repo

Create a new branch: feature/your-idea

Implement and add tests

Submit a PR with detailed description and screenshots if needed

⚖️ License
Distributed under the MIT License. See LICENSE.md for details.

📞 Contact
Brought to you by Vimarsh Dwivedi
For feature requests or partnership talks, reach out via GitHub Issues.

