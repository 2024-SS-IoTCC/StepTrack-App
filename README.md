# StepTrack-App

## Project Overview

### Title

_**StepTrack: A Comprehensive IoT and Cloud-based Activity Monitoring System**_

### Objective

Develop an integrated system that leverages smartphone sensors, edge computing, and cloud technology to monitor and
analyze user activity levels, providing real-time and historical data insights.

### Components

1. **Smartphone Application ([StepTrack-Mobile](https://github.com/2024-SS-IoTCC/StepTrack-Mobile))**
    - **Functionality**: Tracks user steps using the smartphone's StepCounter sensor. Data is stored locally and
      transmitted to the edge device periodically.
    - **Features**:
        - Continuous step counting with local storage.
        - Periodical data transmission to the edge device via MQTT.
        - User is identified by a username.
    - **Technologies**: Android, Kotlin

2. **Edge Application ([StepTrack-Edge](https://github.com/2024-SS-IoTCC/StepTrack-Edge))**
    - **Functionality**: Receives raw step data from the smartphone app, aggregates the data and forwards it to the cloud server.
    - **Features**:
        - Real-time data processing.
        - Communication with both the smartphone app and cloud server.
    - **Technologies**: Spring Boot

3. **Cloud Application ([StepTrack-Cloud](https://github.com/2024-SS-IoTCC/StepTrack-Cloud))**
    - **Functionality**: Hosts a web application that presents a live leaderboard and offers historical analysis of user
      activities.
    - **Features**:
        - Tracking of user activities and step counts.
        - Historical data analysis and progression tracking.
        - Web dashboard displaying individual and aggregate statistics.
    - **Technologies**: Vue (frontend), Go (backend)

## Architecture

Take a look at the architecture described in [ARCHITECTURE.md](ARCHITECTURE.md).
