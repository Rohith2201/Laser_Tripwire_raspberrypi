# Laser_Tripwire_raspberrypi
Laser trip wire is a system for detecting the presence of intruders in a given area

Laser Trip Alarm System
ECS IoT Hackathon Project

This project aims to create a system that detects motion and activates an alarm when the laser beam is interrupted. Prior to using this system, we strongly advise you to carefully read this user manual to ensure correct setup and operation.

## Table of Contents:

System Components:

The Laser Trip Wire System comprises the following elements:
1. Laser emitter (Laser)
2. Laser receiver (LDR)
3. Alarm
4. Power supply
5. PiCamera

Installation:

a. RaspberryPi OS Installation:
   Start by installing RaspberryPi OS using Imager (we recommend the 32-bit version). Then, initialize the VNC viewer via Putty. Log in to the VNC Viewer with your username and password. It's a good practice to enable a hotspot during RaspberryPi OS installation.

b. Mounting the Laser Emitter and Receiver:
   Position the laser emitter and receiver to face each other at the desired distance, allowing the laser beam to pass between them. Utilize the supplied mounting brackets to securely attach the emitter and receiver on opposite sides of the monitored area.

c. Connecting the Alarm and Power Supply:
   Connect the alarm and power supply to the laser receiver following the provided instructions. Ensure the power supply is linked to a stable power source with the correct voltage and polarity.

d. Testing:
   Verify the system's functionality by disrupting the laser beam between the emitter and receiver. The alarm should immediately activate when the beam is interrupted. If the system malfunctions, refer to the troubleshooting section in this manual.

   After successfully testing the circuit, you can directly connect the components to the Raspberry Pi, as illustrated below:
   - Attach one leg of the LDR and the longer leg of the capacitor to a female-to-female jumper lead and secure them with tape.
   - Insert the remaining legs into jumper leads and reconnect everything to the Raspberry Pi.
   - If desired, enclose the Raspberry Pi and components in a housing for concealment. In our example, we used a plastic box with a hole for the straw.
   - Mount the laser pointer on the wall to focus the beam down the straw.
   - Finally, run the code and test your laser tripwire.
   - If you want to automate tasks with Cron and run your code upon Raspberry Pi boot, refer to the instructions below.

e. Enabling Camera:
   - Execute `sudo raspi-config` in the terminal.
   - Select Interface Options and enable the camera. Then, use the `cam.py` code to check the camera's functionality.

f. Setting up Email:
   - We have configured an email ID and generated an app password using smtplib.
   - We are sending emails with attached images captured by the PiCamera. Refer to `sent.py` for details.

g. Setting up LiveStream:
   - Follow the instructions in the live file for this setup.

operation:

The Laser Trip Wire System is designed to identify motion and activate an alarm when the laser beam is disrupted. It serves both security purposes, such as detecting intruders, and industrial automation needs, such as monitoring machinery movements.

We trust that you will find the Laser Trip Wire System valuable and dependable for your security or industrial automation requirements. Should you have any questions or concerns, please don't hesitate to contact us.

Best regards,
Team Destiny
