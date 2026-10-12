<a id="readme-top"></a>

<!-- PROJECT SHIELDS -->
[![MIT License][license-shield]][license-url]

<!-- PROJECT TITLE -->
<div align="center">
  <h3 align="center">SproutCare</h3>

  <p align="center">
    An IoT plant-monitoring system that tracks plant conditions and helps inform plant care.
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About the Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li><a href="#how-it-works">How It Works</a></li>
    <li><a href="#repository-structure">Repository Structure</a></li>
    <li><a href="#getting-started">Getting Started</a></li>
    <li><a href="#usage">Usage</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About the Project

SproutCare is an IoT plant-monitoring system designed to help make plant care more consistent. Sensors connected to an Arduino UNO R4 WiFi will collect plant-condition data and send measurements over Wi-Fi to a backend for storage. A custom Progressive Web App (PWA) will display current readings and historical trends, with the longer-term goal of providing useful plant-care notifications based on collected data.

The project also explores the engineering behind a reliable monitoring system, including sensor calibration, data collection, filtering, fault detection, and analysis of changes over time.

### Built With

**Hardware:**
* Arduino UNO R4 WiFi
* Waterproof capacitive soil-moisture sensor (planned)
* Waterproof DS18B20 temperature probe (optional; subject to testing)
* Breadboard and starter-kit components for prototyping
* 3D-printed enclosure (planned)

**Software:**
* [![Arduino][Arduino-badge]][Arduino-url]
* [![Arduino IDE][ArduinoIDE-badge]][ArduinoIDE-url]
* [![C++][Cpp-badge]][Cpp-url]
* Backend and database (to be selected)
* Progressive Web App (PWA)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- HOW IT WORKS -->
## How It Works

The planned system will collect sensor readings with the Arduino UNO R4 WiFi, send measurements over Wi-Fi to a backend, and store the data for the PWA to display. Once enough reliable data has been collected, the project will explore alert rules based on sustained conditions and drying trends.

```text
Sensors
   ↓
Arduino UNO R4 WiFi
   ↓ Wi-Fi
Backend / Database
   ↓
SproutCare PWA
   ↓
Historical charts and plant-care alerts
```

Sensor selection, calibration, filtering, and alert thresholds will be tested rather than assumed. Predictive features are a future goal and are not part of the initial prototype.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Repository Structure

Update this outline to match the folders in the repository as the project develops.

```text
.
├── docs/          # Design notes, experiments, diagrams, and test results
├── firmware/      # Microcontroller code
├── backend/       # Backend and data storage
├── frontend/      # PWA application
├── hardware/      # Wiring notes and CAD/enclosure files
├── .gitignore
├── LICENSE
└── README.md
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

The complete system is still under development. To prepare for firmware work:

### Prerequisites

* [Arduino IDE](https://www.arduino.cc/en/software)
* Arduino UNO R4 WiFi board support installed through Boards Manager
* Arduino UNO R4 WiFi
* Suitable USB cable for programming

### Installation

1. Install and open the Arduino IDE.
2. In Boards Manager, search for **UNO R4 WiFi** and install the board support package.
3. Connect the board to your computer.
4. Open the firmware sketch once it has been added to the repository.
5. Select **Arduino UNO R4 WiFi** and the connected port, then upload the sketch.

Hardware wiring and software setup instructions will be added as those parts are implemented.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE -->
## Usage

The initial development stage will focus on reading sensors and recording repeatable measurements. Wi-Fi transmission, backend storage, the PWA, and plant-care alerts will be added and documented as they become functional.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[license-shield]: https://img.shields.io/badge/License-MIT-red?style=for-the-badge
[license-url]: LICENSE

[Arduino-badge]: https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white
[Arduino-url]: https://www.arduino.cc/

[ArduinoIDE-badge]: https://img.shields.io/badge/Arduino_IDE-00979D?style=for-the-badge&logo=arduino&logoColor=white
[ArduinoIDE-url]: https://www.arduino.cc/en/software

[Cpp-badge]: https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus
[Cpp-url]: https://isocpp.org/
