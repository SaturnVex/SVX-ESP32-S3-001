# Wi-Fi AP / STA HTTP Test

**Board:** `SVX-ESP32-S3-001` · **MCU:** ESP32-S3 · **Framework:** ESP-IDF v6.1

Wi-Fi SoftAP (phone connects to `SaturnVex-S3-WiFi`, 192.168.4.1) or Station (board joins a 2.4 GHz router) selected in menuconfig, with an HTTP server on port 80 serving an HTML page at `/` and JSON status at `/status`.

## Files

- [Test setup, configuration, build/flash and acceptance guide (PDF)](SaturnVex_ESP32S3_WiFi_AP_STA_Test_Guide_EN.pdf)
- [ESP-IDF source project (ZIP)](ESP32S3_WiFi_AP_STA_Test_SaturnVex.zip?raw=true)

## Run this test

1. Read the PDF guide and confirm the hardware connections and prerequisites.
2. Download and extract `ESP32S3_WiFi_AP_STA_Test_SaturnVex.zip`, preserving the project files.
3. In VS Code select File → Open Folder, choose the extracted `SVX_ESP32S3_WiFi_Test` folder, open an ESP-IDF v6.1 terminal and run `idf.py set-target esp32s3` and `idf.py menuconfig` (SaturnVex Wi-Fi Test Configuration → SoftAP or Station), then `idf.py build` and `idf.py -p COM_PORT -b 115200 flash monitor`, following the guide.
4. Verify the results using the PDF acceptance criteria.

SaturnVex files are provided under the BSD-3-Clause license (`LICENSE.txt`). Espressif ESP-IDF and other third-party software keep their own licenses (`NOTICE.txt`); preserve them when redistributing.

[← All tests](../README.md) · [← Product home](../../README.md)
