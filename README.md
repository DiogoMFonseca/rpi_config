# Raspberry Pi Setup Guide

## Introduction

This guide provides instructions for setting up your Raspberry Pi with the necessary configuration files to enable remote access and connect to a Wi-Fi network.

## File Descriptions

1. **wpa_supplicant.conf:**
   - Copy this file to the root folder of your Raspberry Pi's SD card.
   - Modify the content of the file as follows:
     - `country`: Set your country code (e.g., `pt` for Portugal, `en` for England, `us` for the United States).
     - `ssid`: Set your Wi-Fi network's SSID.
     - `psk`: Set your Wi-Fi network's password.

2. **ssh:**
   - Copy this file to the root folder of your Raspberry Pi's SD card.
   - This file enables SSH on your Raspberry Pi. No content modification is needed.

3. **userconf:**
   - Copy this file to the root folder of your Raspberry Pi's SD card.
   - This file sets the default SSH login credentials for the new Raspberry Pi image (Bullseye):
     - Username: `pi`
     - Password: `raspberry`

## Instructions

1. **Copy Files:**
   - Copy the following files to the root folder of your Raspberry Pi's SD card:
     - `wpa_supplicant.conf`
     - `ssh`
     - `userconf`

2. **Modify wpa_supplicant.conf:**
   - Open `wpa_supplicant.conf` with a text editor.
   - Change the values of `country`, `ssid`, and `psk` according to your network configuration.

3. **Insert SD Card:**
   - Insert the SD card into your Raspberry Pi.

4. **Power On:**
   - Power on your Raspberry Pi.

5. **Access Raspberry Pi:**
   - Connect to your Raspberry Pi remotely using SSH with the provided login credentials in `userconf`.

```plaintext
Username: pi
Password: raspberry
