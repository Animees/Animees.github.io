---
title: Started Spotify Matrix Project
date: 2025-03-01 12:00:00 +0100
categories: [Passion Projects, Ongoing]
tags: [ESP32, C++, Webserver, Rest-API]     # TAG names should always be lowercase
description: A 64x64 LED matrix that will display the currently playing song from my Spotify account
toc: true
comments: true
image:
  path: /assets/img/posts/spotify_matrix/spotify_logo.jpg
  alt: Spotify logo
---
![LED Matrix Example](/assets/img/posts/spotify_matrix/led_matrix_example.jpg){: w="240" .right}
## Overview
I'm working on a **64x64 LED matrix** that will display the currently playing song from my Spotify account. The project will be powered by an **ESP32**, which will handle API requests to extract song details and display the song's album cover on the matrix.

## Features
- **WiFi Connectivity** – The ESP32 will connect to the internet via WiFi.
- **WiFi Manager** – A custom WiFi manager will allow easy network setup.
- **Web Server for OAuth** – Since Spotify requires authentication, a small web server will run on the ESP32 for OAuth authentication.
- **HTTP Requests & JSON Parsing** – The ESP32 will fetch song data and extract relevant details to display on the matrix.
- **LED Matrix** - Matrix that displays the song's cover with 64x64 resolution.

## Planned Expansion(s)
- **Mobile/Web App** – An interface to configure:
   - LED matrix settings (brightness, colors, etc.)
   - Spotify account linking
   - WiFi configuration
- **Encasing** - An encasing for production and aesthetics

## Tech Stack
- **ESP32** for processing
- **64x64 LED Matrix** for displaying the song's cover art
- **Spotify API** for fetching song data
- **Webserver (ESPAsyncWebServer)** for OAuth handling
- **VSCODE / PlatformIO** for development

## Next Steps
🔧 Set up WiFi manager <br>
🔧 Start implementing Matrix functionality

Let me know if you have suggestions or ideas! 🚀
