# LoRa Collision Avoidance Simulation

This repository contains a Python-based simulation for analyzing packet collisions in LoRa networks, with a focus on optimizing transmission strategies for an autonomous water sensor system.

## Overview

Collisions in LoRa networks occur when multiple packets arrive simultaneously at the receiver using the same channel and spreading factor (SF). This project simulates various scenarios to evaluate collision avoidance techniques and optimize data transmission strategies.

## Features

- **Simulation of LoRa network collisions** with:
  - 10 water sensors acting as network nodes.
  - Random positioning between 100 m and 200 m from the gateway.
  - Transmission with SF7, 250 kHz bandwidth, and 5 dBm transmission power.
  - Three available frequencies: 868.1 MHz, 868.3 MHz, and 868.5 MHz.

- **Implemented collision avoidance methods:**
  - Random delays (50 ms to 500 ms) before transmission.
  - Backoff mechanism upon collision detection.
  - Deterministic scheduling for improved transmission efficiency.

- **Performance analysis through statistical visualization:**
  - Number of successfully received packets.
  - Number of collisions and lost packets.
  - Efficiency of transmission scheduling.

## Installation

To run the simulation, ensure you have the following installed:

### Prerequisites

- **Python** (≥3.7)
- **Required Python libraries:**

  Install the necessary dependencies using the following command:

  ```bash
  pip install numpy matplotlib random datetime
