# BMI270 IMU to UART Test

**Board:** `SVX-ESP32-S3-001` · **MCU:** ESP32-S3 · **Framework:** ESP-IDF v6.1

Bosch BMI270 accelerometer / gyroscope over I²C with the official Bosch SensorAPI; 100 ms polling and CSV output on UART1 TX (GPIO43, 115200 8-N-1).

## Files

- [Test setup, connections, build/flash and acceptance guide (PDF)](SaturnVex_ESP32S3_BMI270_UART_Test_Guide_EN.pdf)
- [ESP-IDF source project (ZIP)](ESP32S3_BMI270_UART_Test_SaturnVex.zip?raw=true)

## Run this test

1. Read the PDF guide and confirm the hardware connections and prerequisites.
2. Download and extract `ESP32S3_BMI270_UART_Test_SaturnVex.zip`, preserving the project files.
3. In VS Code select File → Open Folder, choose the extracted `SVX_ESP32S3_BMI270_UART_Test` folder, open an ESP-IDF v6.1 terminal and run `idf.py set-target esp32s3`, `idf.py build` and `idf.py -p COM_PORT -b 115200 flash monitor`, following the guide.
4. Verify the results using the PDF acceptance criteria.

SaturnVex files are provided under the BSD-3-Clause license (`LICENSE.txt`). Espressif ESP-IDF and other third-party software keep their own licenses (`NOTICE.txt`); preserve them when redistributing. The bundled Bosch BMI270 SensorAPI (unmodified, BSD-3-Clause) keeps its own license (`components/bosch_bmi270/LICENSE`).

[← All tests](../README.md) · [← Product home](../../README.md)
