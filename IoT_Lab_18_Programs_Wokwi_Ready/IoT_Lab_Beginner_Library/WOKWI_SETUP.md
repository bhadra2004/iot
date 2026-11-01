# Wokwi setup — IoT Lab (18 programs)

## Which programs use Wokwi?

Programs **1 (DHT22), 2 (LDR), 3 (PIR), 4 (ESP32 MQTT)** and **18 (Smart Traffic demo)** include ready-to-copy `diagram.json` and Arduino sketches. The other programs are Python/HTML applications and run locally in VS Code; see their individual READMEs. Program 18 is a simplified demonstration, not a full implementation of the project.

## Run an ESP32 program

1. Open https://wokwi.com/projects/new/esp32 and create an ESP32 project.
2. Copy the program's `.ino` file into Wokwi `sketch.ino`.
3. Replace Wokwi `diagram.json` with the program's `diagram.json`.
4. For programs 1 and 4, use the Wokwi Library Manager to add the names in `libraries.txt`.
5. Start Simulation and view the Serial Monitor. Change DHT22 values by clicking the sensor; change LDR light by clicking the photoresistor; trigger PIR motion using the simulator sensor control.
6. For Program 4, Wokwi uses `Wokwi-GUEST` (no password). Run the local `subscriber.py` on your computer after installing `requirements.txt`. The subscriber and publisher must use the same MQTT topic. Public broker connectivity depends on Wokwi networking and broker availability.

## Python programs

From the folder containing `requirements.txt`, run `python -m pip install -r requirements.txt`, then follow each program's README. `pip` installs Python packages only; it does not install Arduino libraries or fetch program files.

## Notes

- Wokwi does not require a physical ESP32 or sensors.
- Programs 5–17 remain local Python/HTML implementations; they have **not** been converted to Wokwi, since Wokwi is used for ESP32 simulation.
- Some programs require internet, API keys, services or datasets.
- If a diagram reports an invalid pin or component, use the Wokwi component picker to verify the part and pin names for the simulator version in use.
