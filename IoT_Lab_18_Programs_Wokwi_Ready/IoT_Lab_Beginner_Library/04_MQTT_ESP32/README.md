# Program 4: ESP32 MQTT publisher and Python subscriber

Simplified learning version based on the supplied IoT lab manual.

## Run
1. Install PubSubClient and DHT Arduino libraries; wire DHT22 as in Program 1.
2. Edit Wi-Fi credentials and optionally change the MQTT topic in BOTH files.
3. Run `python subscriber.py` in terminal (install requirements first).
4. Upload ESP32_Publisher/ESP32_Publisher.ino and observe messages.

Public MQTT broker: use a unique topic and do not publish private information.

### Wokwi simulator
Open the Arduino sketch folder in this program, and copy its `.ino`, `diagram.json` and `libraries.txt` contents into a Wokwi ESP32 project. See the root `WOKWI_SETUP.md`.
