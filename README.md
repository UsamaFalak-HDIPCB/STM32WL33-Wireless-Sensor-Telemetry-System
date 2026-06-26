# Wireless-Sensor-Telemetry-System
Self-Employed / Freelance

<img width="2122" height="457" alt="Image" src="https://github.com/user-attachments/assets/2daa3f7e-836b-41e2-a86e-cd92eff92fbb" />
Two-board 433/434 MHz wireless sensor telemetry system with STM32WL33 sensor node, RF matching network, pressure/temperature sensor, IMU, SPI ADC, and USB-C receiver bridge.


# 433 MHz Wireless Sensor Telemetry System

This project is a two-board 433/434 MHz wireless sensor telemetry system designed for low-power remote sensing, wireless data transmission, and PC-based logging. The system consists of a compact sensor/transceiver board and a separate USB-C receiver/data bridge board.

The sensor board is based on the STM32WL33 wireless MCU and is designed to collect data from multiple sensors, including a pressure/temperature sensor, IMU, and external ADC inputs. It includes a 433/434 MHz RF path with antenna matching, tuning components, RF test options, programming pads, and test points for prototype bring-up.
The receiver board acts as the PC interface and development bridge. It receives wireless packets from the sensor board, sends commands or acknowledgements back to the sensor node, and outputs received data over USB-C as serial data for logging and debugging. The receiver board is intentionally designed to be larger, easier to assemble, easier to probe, and more convenient for firmware development.



## Key Features

- Two-board wireless telemetry architecture
- Board A: compact 433/434 MHz sensor/transceiver node
- Board B: USB-C receiver and PC data bridge
- STM32WL33-based sub-GHz wireless sensor board
- 433/434 MHz RF path with 50Ω routing and matching network
- SMA/u.FL/lab antenna option and custom antenna feed support
- ADS1220 SPI ADC with up to 4 analog input channels
- MS5840 pressure/temperature sensor over I2C
- LSM6DSO IMU over I2C for accelerometer and gyroscope data
- SWD programming and test pads for prototype debugging
- USB-C serial output for packet logging and command interface
- JLCPCB 4-layer impedance-controlled PCB design approach


## Functionality

The sensor board collects environmental and motion data, processes it through the STM32WL33 MCU, and transmits packets wirelessly over the 433/434 MHz sub-GHz link. The receiver board receives the packets and forwards the data to a PC through USB-C, where it can be logged, displayed, or used for testing.

The receiver board can also send commands, acknowledgements, or configuration data back to the sensor board, making the system suitable for bidirectional telemetry and prototype development.

Expected received data may include packet number, RSSI, pressure, temperature, accelerometer data, gyroscope data, ADC readings, and battery voltage if implemented.

<img width="992" height="457" alt="Image" src="https://github.com/user-attachments/assets/48cdb982-3b47-4721-a0af-7d88935df835" />
<img width="1017" height="412" alt="Image" src="https://github.com/user-attachments/assets/4ad8de25-8131-47f3-bd94-77ec1bb22601" />
<img width="957" height="387" alt="Image" src="https://github.com/user-attachments/assets/6ada391d-f479-4303-8a6b-3625046e52de" />
<img width="912" height="402" alt="Image" src="https://github.com/user-attachments/assets/d468b770-ee88-4805-9711-220054662347" />

## My Role

- Converted the technical design brief into schematic and PCB layout for both boards.
- Designed Board A as a compact RF sensor node with STM32WL33, sensors, ADC, antenna feed, RF tuning network, and programming/test access.
- Designed Board B as a robust USB-C receiver bridge for PC logging, wireless packet reception, debugging, and bidirectional communication.
- Planned 4-layer impedance-controlled PCB layouts with 50Ω RF routing, ground stitching, antenna keep-out awareness, and JLCPCB manufacturing requirements.
- Prepared the hardware design for prototype fabrication, testing, and RF tuning.

