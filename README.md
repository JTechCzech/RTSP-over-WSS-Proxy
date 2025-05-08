# RTSP over WSS Proxy - Introduction
## Info
This program serves as a proxy between WSS and RTSP. Maybe you ever wanted to get RTSP stream from your security IP camera but it didn't support this protocol and only supported their application. Most of these cameras use websocket communication and transfer data over it in different protocols like RTSP or HLS.

## How does it work?
This program creates an RTSP server on port 8554 and connects to the websocket server. It then forwards RTSP packets from the local server to the websocket messages and vice versa. For packets where modifications such as DESCRIBE, PLAY, etc. are needed, it makes the changes.

## Supported devices:
**This program is primarily created for D-Link security cameras.**
<br>
Tested models:
| Model              | Working |
|--------------------|---------|
| D-Link DCS-P6000LH | YES     |

(if you own a D-Link camera we would be happy to test and create a pull request with results)
# Instalation
