# Hydroponic Control v2
Mobile-first GitHub Pages application for ESP32/Nano hydroponics.

## Upload
Upload all files preserving folders. Open GitHub Pages URL.

## Firebase
Uses Firebase JS SDK 12.18.0 browser modules with Email/Password Authentication and Firestore. Replace Firebase config only if project changes.

## MQTT
HiveMQ Cloud WebSocket: `wss://99580666d99a4632b4a1d5087e22d494.s1.eu.hivemq.cloud:8884/mqtt`
Topics:
- hydroponic/GH001/sensors
- hydroponic/GH001/state
- hydroponic/GH001/config
- hydroponic/GH001/config/state
- hydroponic/GH001/command
- hydroponic/GH001/ack
- hydroponic/GH001/availability

## Notes
The web client must have Firestore rules allowing authenticated users to access only their own `users/{uid}/...` data. MQTT password is entered in Settings; it is not hard-coded.
