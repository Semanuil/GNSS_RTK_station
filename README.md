📡 BASE STATION (/app/rtk_base_station/)

Features:

✅ UART communication with LC29HBS GNSS module (115200 baud rate)

✅ RTCM reading and parsing from GNSS data

✅ ESP-NOW communication for sending RTCM data to the rover

✅ Wi-Fi Access Point (“RTK_Base_Station”, password: “rtk12345”)

✅ Web server for status monitoring at http://192.168.4.1

✅ FreeRTOS tasks for non-blocking communication

Key Files:
	•	main.c – Main application with FreeRTOS queue system
	•	esp_now_base.c/h – ESP-NOW communication
	•	uart_gnss.c/h – UART communication with LC29HBS
	•	wifi_server.c/h – Wi-Fi AP and web monitoring
