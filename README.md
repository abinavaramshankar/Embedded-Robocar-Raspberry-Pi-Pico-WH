# Embedded Robocar

A four-wheel-drive car that I built and drive from a web page over Wi-Fi. It runs on a Raspberry Pi Pico WH and is written in Python. I made it for the Electronic Systems course in the IIT Madras School Connect Program.

## What this project is

I wanted to see how a tiny microcontroller can turn a few lines of code into something that actually moves. The Pico connects to Wi-Fi and hosts a simple control page. I open that page on my phone or laptop, tap a direction, and the car drives forward, backward, left or right.

Building it taught me a lot about embedded programming, wiring things up properly, and debugging when the code and the hardware disagree.

## What's inside

- **Brain:** Raspberry Pi Pico WH
- **Motors:** 4 × 12V DC motors (about 300 RPM each)
- **Motor drivers:** 2 driver modules, each handling a pair of motors
- **Power:** 3 × 18650 lithium-ion cells in series (about 11.1V total)
- **Body:** a standard four-wheel robot car chassis

## How it works

1. The Pico boots up and joins the Wi-Fi network I've set in the code.
2. I type its IP address into a browser, which opens the control page.
3. When I press a button, the Python program on the Pico reads the command.
4. The Pico sends signals to the two motor drivers.
5. The drivers spin the four motors in the right directions, and the car moves.

## What I learned

- Writing Python for a microcontroller instead of a regular computer
- Connecting a Pico to motor drivers and getting four motors to work together
- Setting up wireless control through a web interface
- Tracking down problems that could be in the wiring, the power, or the code
- Fitting electronics and mechanical parts into one working machine

## Where I'd take it next

- Obstacle detection with sensors, starting with an ultrasonic distance sensor
- Speed control using PWM, so the car isn't always at full throttle
- Live battery and motor readings on the control page
- Eventually, some autonomous driving, like following a path on its own

## Project Demonstration

- Watch the demonstration of the project on youtube
- https://youtu.be/oiq4mEuV4kM?si=RYISXil5QpALXP4S

## Background

This was part of a technical course run through the IIT Madras School Connect Program, which introduces practical ideas in electronic systems and embedded technology.

A demo video showing the car and its movement is available separately.

---

**Platform:** Raspberry Pi Pico WH · **Language:** Python · **Domain:** Embedded Systems & Robotics
