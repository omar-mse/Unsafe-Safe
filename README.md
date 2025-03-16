# safeuno

A project for Scrapyard-SHJ hackathon.

safeuno is an Arduino-powered electronic safe with a twist—it forgets its password every time it locks! Designed with a keypad, LCD display, and servo motor, safeuno challenges users to remember (or guess) the new password each time they want to open it. Perfect for adding an element of unpredictability to security!

🚀 Set a password, lock the safe, and watch it vanish into oblivion! Can you crack your own safe? 😆


## Features

- **Keypad Input** - Set and enter a password
- **LCD Display** - Shows prompts and status messages.
- **Servo Lock Mechanism** - Locks/unlocks based on input.
- **Random Password Reset** - The safe "forgets" the old password when locked.


## Hardware

- Arduino Uno R3
- 4x4 Keypad
- 16x2 LCD Display
- SG90 Servo Motor
- Resistors and Wires


## Wiring

| Component     | Arduino Pin(s)  |
|--------------|---------------|
| Keypad       | 8, 9, 10, 11, 12, 13, A0, A1 |
| LCD RS       | 7             |
| LCD E        | 6             |
| LCD D4-D7    | 5, 4, 3, 2     |
| Servo PWM    | 9             |
| LCD VCC      | 5V            |
| LCD GND      | GND           |


## Code Overview

- **Set Password:** User enters a password on the keypad.
- **Lock Safe:** Servo locks; password resets.
- **Unlock Safe:** User enters the correct password (or tries to guess the new one 😝)


## How It Works

1. **Power on** – The safe prompts for a password.
2. **User sets password** – Enter and confirm.
3. **Safe locks** – Password is erased.
4. **To open** – Enter the forgotten password. (Good luck!)
5. **Wrong password?** – Try again.


## Future Improvements

- Add EEPROM to store passwords.
- Implement a hacking deterrent (e.g, alarm or timeout).
- Add an emergency unlock system.
