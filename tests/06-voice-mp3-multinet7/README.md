# Voice-Controlled MP3 Player (MultiNet7) Test

**Board:** `SVX-ESP32-S3-001` · **MCU:** ESP32-S3 · **Framework:** ESP-IDF v6.1

SD-card MP3 player controlled by offline English voice commands (NEXT, BACK, ENTER, EXIT, STOP) using ESP-SR AFE / VAD and MultiNet7, with playback-reference AEC.

## Files

- [Test setup, connections, build/flash and acceptance guide (PDF)](SaturnVex_ESP32S3_Voice_MP3_MultiNet7_Test_Guide_EN.pdf)
- [ESP-IDF source project (ZIP)](ESP32S3_Voice_MP3_MultiNet7_Test_SaturnVex.zip?raw=true)

## Run this test

1. Read the PDF guide and confirm the hardware connections and prerequisites.
2. Download and extract `ESP32S3_Voice_MP3_MultiNet7_Test_SaturnVex.zip`, preserving the project files.
3. In VS Code select File → Open Folder, choose the extracted `SVX_ESP32S3_SD_MP3_MultiNet7` folder, open an ESP-IDF v6.1 terminal and run `idf.py set-target esp32s3`, `idf.py build` and `idf.py -p COM_PORT -b 115200 flash monitor`, following the guide. The first build needs Internet access for the ESP-IDF Component Manager.
   In `idf.py menuconfig` confirm *ESP Speech Recognition → English Speech Commands Model → mn7_en*.
4. Verify the results using the PDF acceptance criteria.

SaturnVex files are provided under the BSD-3-Clause license (`LICENSE.txt`). Espressif ESP-IDF and other third-party software keep their own licenses (`NOTICE.txt`); preserve them when redistributing. Espressif managed components (`esp-sr` with the MultiNet7 model, `esp_codec_dev`, `esp_audio_codec`) are downloaded at build time and keep their own licenses.

[← All tests](../README.md) · [← Product home](../../README.md)
