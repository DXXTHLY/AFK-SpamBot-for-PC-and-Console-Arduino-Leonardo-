# 🎮 Arduino AFK & Chat Spam Bot (PC + Console)

Automate AFK movement, mouse clicks, and chat spam for PC games — or simulate PS4 controller input using Arduino Leonardo with a USB Host Shield. Perfect for botting, farming, or just staying alive in multiplayer lobbies.

---

##  Requirements

###  PC Version
- Arduino Leonardo or Micro
- Micro USB cable
- Arduino IDE installed

### 🎮 Console Version (PS4)
- Arduino Leonardo or Micro
- USB Host Shield 2.0
- PS4 Controller (USB wired)
- USB-A to USB-B cable (for Leonardo)
- Arduino IDE installed

---

## 🖥️ PC AFK + Chat Spam Bot

### 🔧 Arduino Code

```cpp
#include "Keyboard.h"
#include "Mouse.h"

unsigned long lastActionTime = 0;
unsigned long actionInterval = 10000; // Every 10 seconds

// Array of random messages
const char* messages[] = {
  "hello world",
  "gg ez",
  "anyone got mic?",
  "yo chill 😭",
  "bro thinks he's him",
  "nice hacks bro",
  "i lagged 😒",
  "touch grass 💀",
  "LMAO",
  "👽👽👽"
};
const int messageCount = sizeof(messages) / sizeof(messages[0]);

void setup() {
  Keyboard.begin();
  Mouse.begin();
  delay(3000); // Wait before starting actions
}

void loop() {
  unsigned long now = millis();

  if (now - lastActionTime > actionInterval) {
    // Move mouse slightly
    int moveX = random(-10, 10);
    int moveY = random(-10, 10);
    Mouse.move(moveX, moveY);

    // Optional random mouse click
    if (random(0, 2)) {
      Mouse.click(MOUSE_LEFT);
    }

    // Random chat spam
    if (random(0, 2)) {
      Keyboard.press('t'); // Open chat (change key if needed)
      delay(100);
      Keyboard.release('t');
      delay(100);

      // Pick a random message and send it
      int index = random(0, messageCount);
      Keyboard.print(messages[index]);

      Keyboard.press(KEY_RETURN); // Send
      delay(100);
      Keyboard.release(KEY_RETURN);
    }

    lastActionTime = now;
  }
}
````

###  How It Works

| Action                | Description                         |
| --------------------- | ----------------------------------- |
| `Mouse.move()`        | Simulates idle movement             |
| `Mouse.click()`       | Random firing or input              |
| `Keyboard.print()`    | Chat message typing                 |
| `Keyboard.press('t')` | Opens chat window (varies per game) |

### ⚠️ Notes

* This starts automatically when powered.
* You can add a physical toggle switch or keystroke to stop/start later.

---

##  Console (PS4) AFK Bot

###  Arduino + USB Host Shield Code

```cpp
#include <PS4USB.h>
USB Usb;
PS4USB PS4(&Usb);

unsigned long lastActionTime = 0;

void setup() {
  Usb.begin();
  delay(2000); // Wait for USB devices to connect
}

void loop() {
  Usb.Task();

  if (PS4.connected()) {
    unsigned long now = millis();

    if (now - lastActionTime > random(10000, 15000)) {
      // Simulate analog stick movement
      int lx = random(-127, 127);
      int ly = random(-127, 127);
      PS4.setAnalogHat(LeftHatX, lx);
      PS4.setAnalogHat(LeftHatY, ly);

      // Random button press
      if (random(0, 2)) PS4.setButtonClick(CROSS);
      if (random(0, 2)) PS4.setButtonClick(R2);

      lastActionTime = now;
    }
  }
}
```

###  How It Works

| Action                 | Description                   |
| ---------------------- | ----------------------------- |
| `PS4.connected()`      | Ensures controller is working |
| `PS4.setAnalogHat()`   | Simulates stick movement      |
| `PS4.setButtonClick()` | Triggers in-game actions      |

### 🔌 Setup Instructions

1. Stack USB Host Shield on Arduino Leonardo
2. Plug in PS4 controller to USB Host Shield
3. Upload the sketch
4. Connect Leonardo to PS4 (USB-A to Micro)
5. Wait for actions to begin

---

## 🕹️ Xbox Compatibility

🚫 Xbox does **not** support generic USB HID devices.

### ✅ To use with Xbox:

* Buy a **Titan Two**, **XIM Apex**, or similar hardware
* OR use a **Raspberry Pi Pico / RP2040-Zero** flashed with **GP2040-CE**

  * Emulates Xbox 360/Series controller
  * Supports macros, input remapping, anti-recoil, turbo, etc.

---

## 🔒 Future Additions

* Hardware **kill switch / toggle button**
* Customizable **action profiles**
* **Hotkey triggers** to pause or change modes
* Support for **DualSense** or **Bluetooth**

---

##  Need Help?

Open an [Issue](https://github.com/your-username/your-repo/issues) or ask for:

* Console-specific tweaks
* Xbox macro device setup
* Advanced spam or recoil logic

---

## ⚠️ Disclaimer

This project is for educational and accessibility purposes. Do not use to violate game TOS or cheat in online matches.

---

##  License

MIT License

```

---

MIT License

Copyright (c) 2025 DXXTHLY

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights  
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell    
copies of the Software, and to permit persons to whom the Software is       
furnished to do so, subject to the following conditions:                     

The above copyright notice and this permission notice shall be included in  
all copies or substantial portions of the Software.                          

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,    
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER      
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING    
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER        
DEALINGS IN THE SOFTWARE.
```
