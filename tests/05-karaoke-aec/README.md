# Real-Time Karaoke Audio with AEC Test

**Board:** `SVX-ESP32-S3-001` · **MCU:** ESP32-S3 · **Framework:** ESP-IDF v6.1

Live ES7210 microphone to ES8311 speaker audio with Espressif ESP-SR acoustic echo cancellation, 70 Hz high-pass, feedback notch, limiter and overload mute.

## Files

- [Test setup, connections, build/flash and acceptance guide (PDF)](SaturnVex_ESP32S3_Karaoke_AEC_Test_Guide_EN.pdf)
- [ESP-IDF source project (ZIP)](ESP32S3_Karaoke_AEC_Test_SaturnVex.zip?raw=true)

## Run this test

1. Read the PDF guide and confirm the hardware connections and prerequisites.
2. Download and extract `ESP32S3_Karaoke_AEC_Test_SaturnVex.zip`, preserving the project files.
3. In VS Code select File → Open Folder, choose the extracted `SVX_ESP32S3_Karaoke_C8_AEC_FD` folder, open an ESP-IDF v6.1 terminal and run `idf.py set-target esp32s3`, `idf.py build` and `idf.py -p COM_PORT -b 115200 flash monitor`, following the guide. The first build needs Internet access for the ESP-IDF Component Manager.
4. Verify the results using the PDF acceptance criteria.

SaturnVex files are provided under the BSD-3-Clause license (`LICENSE.txt`). Espressif ESP-IDF and other third-party software keep their own licenses (`NOTICE.txt`); preserve them when redistributing. Espressif managed components (`esp_codec_dev`, `esp-sr` and dependencies) are downloaded at build time and keep their own licenses.

[← All tests](../README.md) · [← Product home](../../README.md)
