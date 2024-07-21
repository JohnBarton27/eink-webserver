# E-Ink Webserver
This is a very simple Python application that is meant to run on a Raspberry Pi with a connected e-ink display, using Waveshare drivers. It runs a FastAPI web server (port 8000 by default), with two API endpoint:

* `GET /health`
** Returns `{ "status": "ok" }` if the server is running
* `POST /upload`
** Given a bitmap `file`, uploads the file to the server & displays it on the e-ink display
