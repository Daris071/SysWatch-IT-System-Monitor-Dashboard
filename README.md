# SysWatch-IT-System-Monitor-Dashboard
A real-time IT infrastructure monitoring dashboard built with vanilla JavaScript. Displays live CPU, RAM, disk, network, and process metrics — simulating the kind of dashboards used in real IT operations.



## What I Built
A dark-themed, terminal-inspired dashboard that auto-refreshes every 3 seconds and shows:

CPU usage with a live mini bar chart
RAM usage (GB used out of 16 GB) with history graph
Disk utilization and read speed
Active processes with status badges (RUNNING / IDLE / WARN)
Network interfaces with RX/TX throughput
Live scrolling system log — similar to journalctl output on Linux


## What I Learned
JavaScript (Vanilla)

setInterval() — polling pattern for auto-refreshing live data every 3 seconds
DOM Manipulation — dynamically building and updating HTML tables, bars, and charts without any framework
Math.random() & simulation — generating realistic fluctuating metric values to simulate real sensor data
Date API — formatting and displaying live timestamps for the system log and clock
Array methods — using .push() and .shift() to maintain a rolling 20-point history buffer for sparkline charts

CSS

CSS Variables for theming — full dark theme with one variable change capability
CSS Grid — complex multi-panel dashboard layout with grid-template-columns and grid-column: span 2
@keyframes animations — pulsing status dot to indicate live data
Monospace design — using Courier New for an authentic terminal aesthetic

IT Knowledge Applied

Understanding what metrics matter in IT monitoring (CPU, RAM, disk I/O, network throughput, process states)
Log formatting conventions — timestamps, severity levels (OK / WARN / ERROR / INFO)
Common Linux system services: nginx, mariadb, sshd, cron, fail2ban, php-fpm
Network interface naming conventions: eth0, lo (loopback), docker0


## Tech Stack
TechnologyPurposeHTML5StructureCSS3Dark theme, Grid layout, AnimationsJavaScript (ES6)Live data simulation, DOM updatesGitHub PagesHosting
No npm packages. No build step. Zero dependencies.

## Structure
syswatch-dashboard/
├── index.html        # Everything in one file — HTML + CSS + JS
├── README.md         # This file
└── preview.png       # Screenshot for README

## How to Run
bashgit clone https://github.com/darisvatic/syswatch-dashboard.git
cd syswatch-dashboard
open index.html
The dashboard starts immediately and refreshes every 3 seconds automatically.

## Planned Features

 Dark/light theme toggle
 Connect to a real Node.js backend via WebSocket for actual system metrics
 Alert threshold configuration (e.g. warn when CPU > 80%)
 Export log as .txt file
 Historical data charts using Chart.js


🔗 Related
This project demonstrates skills relevant to my internship experience as an IT Systems Technician, where I administered servers, performed First Level Support, and maintained software across the school network.
