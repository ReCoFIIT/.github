# 👋 Welcome to **ReCo**

**ReCo** is an open-source evaluation platform for cooperative driving using RC cars.  
It provides a controlled environment for testing and evaluating algorithms and strategies in cooperative driving—perfect for both research and development.

Originally developed at **FIIT, Slovak Technical University** in Bratislava.

---

## 🛍️ Project Overview

ReCo is made up of several interconnected components categorized into:

- **Hardware**: Schematics and physical builds for the RC cars  
- **Car Software**: Embedded systems and DevOps for onboard control  
- **Infrastructure**: A microservice-based backend managing vehicle integration, decisions, and data flow

---

## 🛠️ Hardware

- **[KiCad PCB](https://github.com/ReCoFIIT/KiCad)** – Custom PCB designs for onboard electronics  
- **[3D Printable Files](https://github.com/ReCoFIIT/hardware)** – STL models for mechanical parts *(Link coming soon)*

---

## 🚗 On-Car Software

- **[car-ops](https://github.com/ReCoFIIT/car-ops)** – DevOps and provisioning tools for the vehicles  
- **[ROS2 Workspace](https://github.com/ReCoFIIT/ros2_ws)** – ROS2-based software for onboard vehicle logic

---

## 🏗️ Infrastructure

The infrastructure is designed as a set of microservices using a custom UDP protocol.  
Modules are organized in a [**polyrepository**](https://github.com/ReCoFIIT/reco) with Git submodules.

### Main Components

- **[Frontend](https://github.com/ReCoFIIT/frontend)** – Web-based UI for system monitoring and control  
- **[API](https://github.com/ReCoFIIT/backend)** – RESTful backend serving system data  

### Core Services

- **[car-integration](https://github.com/ReCoFIIT/car-integration)**  
  Integrates vehicles with the infrastructure. Handles data collection and command dispatch.

- **[decision-module](https://github.com/ReCoFIIT/decision-module)**  
  Performs high-level decision making based on real-time data and environmental inputs.

- **[integration-api](https://github.com/ReCoFIIT/integration-api)**  
  Shared Go module providing interfaces and models used by the API, car-integration, and decision-module.

---

## 📚 Documentation

Each component contains its own documentation in the respective repositories.  
Start with the [**ReCo Polyrepository**](https://github.com/ReCoFIIT/reco). For full system architecture and setup instructions see the [**Documentation repository**](https://github.com/ReCoFIIT/documentation)
