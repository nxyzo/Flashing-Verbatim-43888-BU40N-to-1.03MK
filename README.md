# Flashing LG BU40N Drive to Firmware 1.03 - User Guide

## Overview
This guide explains how to flash an LG BU40N optical drive to firmware version 1.03 using MakeMKV software. This process allows you to update or modify your drive's firmware for compatibility or functionality improvements.

## Supported Drives
This guide can also be used for the following drives. Simply use the corresponding firmware file named after your drive model and pay attention to the correct version:

- WH16NS60 (Version 1.03)
- WH16NS40 (Version 1.05)
- WH14NS40 (Version 1.05)
- BH16NS55 (Version 1.05)
- BU40N (Version 1.04)

The procedure remains identical. Just select the appropriate firmware file for your drive model from the "All you need firmware pack".

## Prerequisites
- MakeMKV software installed on your computer
- Administrative privileges on your computer
- LG BU40N drive with MT1959 platform
- The firmware file: `HL-DT-ST-BD-RE_BU40N-1.03-NM00000-211810241934.bin` (included in "The all you need firmware pack")

## Drive Compatibility Check
1. Open MakeMKV
2. Verify that your drive:
    - Is identified as LG BU40N
    - Uses the MT1959 platform
    - Current firmware revision is noted (for reference)

## Flashing Procedure
1. **Download Required Files**
    - Obtain "The all you need firmware pack.zip"
    - Extract and locate the appropriate firmware file in the `LG slim BU40N` folder

## Important Notes
- The BU40N 1.04 firmware is encrypted and requires the `enc` parameter in the command
- Do NOT disconnect power or interrupt the flashing process
- The complete process may take several minutes
- The drive will automatically reboot after successful flashing

2. **Flash the Firmware**
    - Open Command Prompt as Administrator
    - Navigate to the MakeMKV installation directory:
      ```
      cd "C:\Program Files (x86)\MakeMKV"
      ```
    - Execute the firmware flashing command:
      ```
      makemkvcon64.exe f --all-yes -d X: rawflash enc -i "PATH_TO_FIRMWARE_FILE"
      ```
      (Replace `X:` with your optical drive letter and `PATH_TO_FIRMWARE_FILE` with the full path to the .bin file)

## Troubleshooting
- If flashing fails, verify you're using the correct firmware file for your specific drive model
- Ensure you have administrative privileges when running the Command Prompt
- Try using a different USB port or connection if using an external drive

## Firmware Information
Supported firmware version: 1.03 for BU40N drives