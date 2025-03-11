---
title: EMC Mouse Touchscreen
date: 2025-02-02 20:58:00 +0100
categories: [Projects, Finished]
tags: [Apache, Rest-API, Flask, Python, IPC, Unix-socket, JSON]     # TAG names should always be lowercase
description: User-friendly GUI for a DIY mouse test chamber
toc: true
comments: true
image:
  path: /assets/img/posts/mouse_touchscreen/erasmus-mc-logo.png
  alt: Erasmus MC (Our product owner's) logo
---
*Started on 03-09-2024*

## Overview
My team and I developed a **GUI and control system** for a **mouse testchamber** at the **Erasmus Neuroscience Department**. The goal was to create a **flexible and user-friendly** platform for researchers conducting mouse behavioral experiments.

![Flask Logo](/assets/img/posts/mouse_touchscreen/flask-horizontal.jpg){: w="280" .right}
During this project, I primarily focused on **setting up an Apache webserver on a Raspberry Pi** and developing a **Rest-API** to handle experiment settings, retrieve results, and control experiment execution. Additionally, I helped establish the communication between the **GUI and experiment code**, by implementing **CORS** and setting up a **Unix-Socket** for inter-process communication (between the API and Experiment code).


This project was the first project of my **2nd year**. It was a **relay project**, so we built upon the code and material of **IPO (Industrial product design)** and **ELE (Electrical engineering)**. Besides the fact that it's a relay project, it was also **multi-disciplinary** since we worked together with **BML (Biomedical laboratory research)**. They were allowed to handle the mice, offered advice for information to be included on the page and used the chamber themselves for their own projects.

## Features
- **GUI for Experiment Control** – Provided an intuitive interface for researchers to configure and manage experiments easily.
- **Apache Web Server** – Hosted the GUI and managed requests from the client.
- **Flask API via Apache (WSGI)** – Enabled the API to run under Apache and handle requests using the same port as the server.
- **REST API with Flask** – Allowed seamless communication between the GUI and hardware components (touchscreen and reward system).
- **Inter-Process Communication (Unix-Socket)** – Established a Unix-Socket for real-time communication between the API and experiment code.
- **Data Logging** – Implemented real-time data logging, storing experiment results in **CSV files** for analysis.
- **Deployment on Raspberry Pi** – The system was successfully deployed and tested on a **Raspberry Pi 4**, utilizing existing code from a previous research team.

## Impact
The completed system provided the **Erasmus Neuroscience Department** with a more **versatile and user-friendly** platform for conducting mouse behavioral tests than before, significantly enhancing research capabilities in **behavioral neuroscience**.

We adviced Erasmus MC to continue development of the system since it could still be improved upon.

## Infographic
![Infographic](/assets/img/posts/mouse_touchscreen/infographic.png)
