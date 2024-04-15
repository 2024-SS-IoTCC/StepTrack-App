# StepTrack-App  

## Project Overview

### Title
_**StepTrack: A Comprehensive IoT and Cloud-based Activity Monitoring System**_

### Objective
Develop an integrated system that leverages smartphone sensors, edge computing, and cloud technology to monitor and analyze user activity levels, providing real-time and historical data insights.

### Components

1. **Smartphone Application (StepTrack App)**
    - **Functionality**: Tracks user steps using the smartphone's StepCounter sensor. Data is stored locally and transmitted to the edge device upon user command.
    - **Features**:
        - Continuous step counting with local storage.
        - Manual data sync to the edge device via MQTT or WiFi Direct.
        - User authentication using a unique username/ID.
    - **Technologies**: TBD

2. **Edge Application**
    - **Functionality**: Receives raw step data from the smartphone app, processes the data to categorize activity levels (e.g., walking, running, sprinting), and forwards the summarized data to the cloud server.
    - **Features**:
        - Real-time data processing and categorization.
        - Communication with both the smartphone app and cloud server.
    - **Technologies**: TBD

3. **Cloud Application**
    - **Functionality**: Hosts a web application that presents a live leaderboard and offers historical analysis of user activities.
    - **Features**:
        - Live tracking of user activities and step counts.
        - Historical data analysis and progression tracking.
        - User-friendly web interface displaying individual and aggregate statistics.
    - **Technologies**: TBD

## Architecture

Take a look at the architecture described in [ARCHITECTURE.md](ARCHITECTURE.md).