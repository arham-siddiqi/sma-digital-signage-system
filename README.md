# sma-digital-signage-system
# SMA Digital Signage System (Public Overview)

## Overview
A production-grade digital signage system designed and deployed for the Stittsville Muslim Association (SMA). The system runs on a Raspberry Pi and autonomously drives a television display with dynamic content and real-time prayer information.

This repository serves as a **technical overview and project showcase**.  
The full production source code is maintained in a private repository to protect organizational infrastructure and configuration.

---

## Problem Statement
SMA required a reliable, low-maintenance way to display high-definition announcements and prayer schedules that could be updated by non-technical administrators without manual intervention or direct system access.

---

## Solution
I designed and implemented a Raspberry Pi–based signage platform with:
- Automated data ingestion from a cloud-managed source
- A browser-based kiosk frontend
- Boot-time auto-launch and crash recovery
- Remote maintenance capability

The system is designed for **unattended, long-running operation** in a real-world environment.

---

## System Architecture (High-Level)
Admin (Content Management)
↓
Python Backend (Data Fetch & Processing)
↓
Local HTTP Server
↓
Chromium (Kiosk Mode)
↓
TV Display

---

## Key Technical Highlights
- **Automated Synchronization**  
  Periodic polling of structured data sources to keep on-screen content up to date without manual refreshes.

- **Fault Tolerance & Recovery**  
  Multiple system services ensure the application launches on boot and recovers automatically from crashes or browser failures.

- **Non-Technical Content Management**  
  Administrators update content using familiar tools without interacting with the underlying system.

- **Resource-Constrained Design**  
  Optimized for reliable performance on Raspberry Pi hardware.

---

## Tech Stack
- **Hardware:** Raspberry Pi 4 
- **Backend:** Python  
- **Frontend:** HTML, CSS, JavaScript  
- **System:** Linux, systemd, Chromium (kiosk mode)

---

## Deployment Status
- Actively deployed in a live environment
- Used by real users
- Designed for continuous operation

---

## Why the Code Is Private
This project is deployed for a real organization.  
To avoid exposing configuration details, service definitions, and operational infrastructure, the production repository is kept private.

Source code access can be provided upon request.

---

## What This Project Demonstrates
- Systems and reliability engineering
- Linux service management (systemd)
- Real-world deployment and maintenance
- Secure handling of production infrastructure
