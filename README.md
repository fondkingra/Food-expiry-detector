# ESP8266 Gas and Environment Monitoring with Email Alert

This project utilizes an ESP8266 microcontroller to monitor gas levels using the MQ135 sensor and environmental conditions (temperature and humidity) using the DHT22 sensor. When the gas level exceeds a certain threshold, an email alert is sent to notify the user.

## Prerequisites

Before you begin, ensure you have the following hardware and software:

- ESP8266 board (e.g., NodeMCU)
- MQ135 gas sensor
- DHT22 temperature and humidity sensor
- Arduino IDE or PlatformIO
- Necessary libraries:
  - Adafruit_MQ135
  - DHT sensor library
  - ESP_Mail_Client

## Installation

1. Clone or download this repository.
2. Open the project in your Arduino IDE or PlatformIO.
3. Install the necessary libraries using the library manager.
4. Update the `WIFI_SSID`, `WIFI_PASSWORD`, `AUTHOR_EMAIL`, `AUTHOR_PASSWORD`, and `RECIPIENT_EMAIL` constants in the code with your Wi-Fi and email credentials.

## Usage

1. Connect the MQ135 sensor to analog pin A0 and the DHT22 sensor to digital pin D5 of the ESP8266 board.
2. Upload the code to your ESP8266 board.
3. Open the serial monitor to view the gas level, temperature, and humidity readings.
4. If the gas level exceeds the specified threshold, an email alert will be sent to the specified recipient email address.

## Configuration

- Modify the threshold value for gas level detection (`gasValue > 1000`) in the code to suit your requirements.
- Adjust the delay between sensor readings (`delay(5000)`) and email alerts (`de
