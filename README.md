# 🎮 Arduino AFK & Chat Spam Bot (PC + Console)

Automate AFK movement, mouse clicks, and chat spam for PC games — or simulate PS4 controller input using Arduino Leonardo with a USB Host Shield. Perfect for botting, farming, or just staying alive in multiplayer lobbies.

---

##  Requirements

###  PC Version
- [Arduino Leonardo](https://www.amazon.com/KEYESTUDIO-Leonardo-Development-Board-Arduino/dp/B0786LJQ8K/ref=asc_df_B0786LJQ8K?mcid=0fd9a8d21d28396d8aecc7d94f5858cc&hvocijid=13190418784293758253-B0786LJQ8K-&hvexpln=73&tag=hyprod-20&linkCode=df0&hvadid=721245378154&hvpos=&hvnetw=g&hvrand=13190418784293758253&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9007848&hvtargid=pla-2281435178338&psc=1) or [Micro](www.amazon.com/diymore-ATmega32U4-Replace-ATmega328-Leonardo/dp/B01KJR41J4/ref=asc_df_B01KJR41J4?mcid=12a3181b166f3d4896e09cda912526f6&hvocijid=13944012122565128041-B01KJR41J4-&hvexpln=73&tag=hyprod-20&linkCode=df0&hvadid=721245378154&hvpos=&hvnetw=g&hvrand=13944012122565128041&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9007848&hvtargid=pla-2281435175938&psc=1)
- [Micro USB cable](https://www.amazon.com/FEMORO-Transfer-Charging-Smartphone-Bluetooth/dp/B0D2KZQR8T/ref=sr_1_3?crid=1GRBMKRBQKLAI&dib=eyJ2IjoiMSJ9.2ODqAvSnCFLkB1v4odzbS67ytg_uNKRTTrMoEc2auz8yw0yCljJfozlBgSPEJMKASYTxKklSAl-Lm3mAT4OGwMAma_M8wEq8J6zsM4y-7JYNn0wFlQYyuHkp50DPqqv7XC3ttfDCpRlzbtLDMOaz1QNT_SweTDqJ7I_EZpOgrYoB_1EVmY-g3IPlWfNlBFqSwb4Iov-fqznt5Xj0gN3VXTssxBTJVv5-JXvIB5j1DNya09njqR3nPiulnZoSO5wlTKEFp-YbhRZpb9P8vQQ-OQrAI5EOg4Vnc-514Mnk34o.JyiA-Vag-ZFKqfZfRwLh9TFrSeEZVLzpQM3cgUUG47E&dib_tag=se&keywords=micro+usb+cable+data&qid=1746560106&s=electronics&sprefix=micro+usb+cable+data%2Celectronics%2C184&sr=1-3)
- [Arduino IDE](https://www.arduino.cc/en/software/) installed

### 🎮 Console Version (PS4)
- [Arduino Leonardo](https://www.amazon.com/KEYESTUDIO-Leonardo-Development-Board-Arduino/dp/B0786LJQ8K/ref=asc_df_B0786LJQ8K?mcid=0fd9a8d21d28396d8aecc7d94f5858cc&hvocijid=13190418784293758253-B0786LJQ8K-&hvexpln=73&tag=hyprod-20&linkCode=df0&hvadid=721245378154&hvpos=&hvnetw=g&hvrand=13190418784293758253&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9007848&hvtargid=pla-2281435178338&psc=1) or [Micro](www.amazon.com/diymore-ATmega32U4-Replace-ATmega328-Leonardo/dp/B01KJR41J4/ref=asc_df_B01KJR41J4?mcid=12a3181b166f3d4896e09cda912526f6&hvocijid=13944012122565128041-B01KJR41J4-&hvexpln=73&tag=hyprod-20&linkCode=df0&hvadid=721245378154&hvpos=&hvnetw=g&hvrand=13944012122565128041&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9007848&hvtargid=pla-2281435175938&psc=1)
- [USB Host Shield 2.0](https://www.amazon.com/HiLetgo-Shield-Arduino-Support-Android/dp/B01MTU9OLM/ref=asc_df_B01MTU9OLM?mcid=844f8521b6813e00842a57c9b9e1f417&hvocijid=3040638385995976275-B01MTU9OLM-&hvexpln=73&tag=hyprod-20&linkCode=df0&hvadid=721245378154&hvpos=&hvnetw=g&hvrand=3040638385995976275&hvpone=&hvptwo=&hvqmt=&hvdev=c&hvdvcmdl=&hvlocint=&hvlocphy=9007848&hvtargid=pla-2281435177858&psc=1)
- PS4 Controller (USB wired)
- [USB-A to USB-B cable](www.amazon.com/Amazon-Basics-External-Gold-Plated-Connectors/dp/B00NH13DV2/ref=sr_1_3?crid=3RHVARL6FPM9&dib=eyJ2IjoiMSJ9.bCBJMqo5p_qtLjShMZULkMHBEqbL6KjSu_Qh9Abr2OlyfKOw1Si4xoF5FdOEEPZ6IoEuIB0VYK4gvAByiCh95HygO5nBTr8kiTmzEzSiRVq1Vv3YOXWgjVI9mevKUUdUS1GKkK-Wvas12LCmgy_XQJKd37-oiis--hOllu4Ckn5_iFh44wwt-NXkq5onjp_xBrbMAFcWftpgU7gAxJ1Y8mhx0nfn_GYiu4tTAUvuglXaW3JY6WBS8UJ-94dKCa1V4nGcdZ_6tUqjl1g_BY14R6FQdSrjZ3qfKVKt0oc7L6Y.my2C_D09kRMC2rO-7owucWwMPrYrRTuJ0if3l6iXUh0&dib_tag=se&keywords=USB-A+to+USB-B+cable&qid=1746560311&s=electronics&sprefix=usb-a+to+usb-b+cable%2Celectronics%2C95&sr=1-3) (for Leonardo)
- [Arduino IDE](https://www.arduino.cc/en/software/) installed

>**Note:** PS4 Controller must be branded controller, not generic.
---

## 🖥️ PC AFK + Chat Spam Bot

### 🔧 Arduino Code

```cpp
#include "Keyboard.h"
#include "Mouse.h"

// Set timing intervals
unsigned long lastActionTime = 0;
unsigned long actionInterval = 10000; // Every 10 seconds
unsigned long mouseMoveInterval = 5000; // Move mouse every 5 seconds

// AFK random actions
const int randomKeys[] = {'W', 'A', 'S', 'D', 'Q', 'E', 'R', 'F', 'G'};  // Example keys to press
const int keyCount = sizeof(randomKeys) / sizeof(randomKeys[0]);

// Meme chat messages
const char* messages[] = {
  "My goldfish is playing for me rn 🐠",
  "Keyboard on fire 🔥",
  "Beep boop I'm a bot",
  "I’m here but spiritually gone",
  "Haven’t blinked in 2 hours 👁️👁️",
  "Running on 3 FPS and dreams",
  "My cat is farming XP",
  "This is totally not a bot",
  "Using dial-up WiFi 📡",
  "I trained a squirrel to play for me 🐿️",
  "Send snacks pls 🍕",
  "Keyboard held hostage",
  "I'm running this on a toaster 🔌",
  "Currently in stealth mode 😎",
  "AI takeover starts now 🤖",
  "Mentally I'm in Minecraft",
  "Ping: 99999ms 🚨",
  "Respawning IRL",
  "My hamster unplugged the router",
  "Hard carrying my KD into the ground",
  "My aim is based on vibes only",
  "Stuck in third person view",
  "Every move is a jump scare 💀",
  "Error 404: Skill not found",
  "I only play with my eyes closed",
  "Fighting lag more than players",
  "Cursed loadout equipped",
  "Powered by coffee and regrets ☕",
  "This isn’t even my final form",
  "My dog queued for me 🐶",
  "Losing pixels by the second",
  "Mousepad is a pizza box",
  "Brain.exe has stopped working",
  "I'm just background noise rn",
  "I mapped shoot to sneeze",
  "Using Morse code to play",
  "This game runs on hopes and dreams ✨",
  "I blink and I die",
  "LAG IS MY SUPERPOWER",
  "Controller is held together by tape",
  "This is a cry for help but make it funny",
  "I can quit anytime I want 🫠",
  "Botting? No this is divine intervention"
};
const int messageCount = sizeof(messages) / sizeof(messages[0]);

// Send message with different methods (T/ENTER)
void sendMessage(const char* msg, bool useT) {
  if (useT) {
    Keyboard.press('t');
    delay(100);
    Keyboard.release('t');
  } else {
    Keyboard.press(KEY_RETURN);
    delay(100);
    Keyboard.release(KEY_RETURN);
  }

  delay(200);
  Keyboard.print(msg);
  delay(100);
  Keyboard.press(KEY_RETURN);
  delay(100);
  Keyboard.release(KEY_RETURN);
}

// Simulate random key press
void pressRandomKey() {
  int keyIndex = random(0, keyCount);
  Keyboard.press(randomKeys[keyIndex]);
  delay(100); // Hold key for a while
  Keyboard.release(randomKeys[keyIndex]);
}

// Simulate random mouse movement
void moveMouseRandomly() {
  int moveX = random(-10, 10);  // Small random horizontal movement
  int moveY = random(-10, 10);  // Small random vertical movement
  Mouse.move(moveX, moveY);
}

// Simulate right stick movement (optional for console setup)
void moveRightStick() {
  // Example movement emulation for right stick (PC version for now)
  int moveX = random(-5, 5);   // Random horizontal movement
  int moveY = random(-5, 5);   // Random vertical movement

  // You would need to adapt this for actual console emulation using USB Host Shield or similar.
  Mouse.move(moveX, moveY);
}

void setup() {
  Keyboard.begin();
  Mouse.begin();
  delay(3000); // Wait before starting actions
}

void loop() {
  unsigned long now = millis();

  if (now - lastActionTime > actionInterval) {
    // AFK Simulation: Perform random key press (WASD, etc.)
    pressRandomKey();

    // AFK Simulation: Move mouse randomly every few seconds
    if (now - lastActionTime > mouseMoveInterval) {
      moveMouseRandomly();
      moveRightStick();  // Simulate right stick movement for console or testing
    }

    // Optional random chat spam
    if (random(0, 2)) {
      int index = random(0, messageCount);
      sendMessage(messages[index], true);  // Try with 'T'
      delay(500); // Small delay between attempts
      sendMessage(messages[index], false); // Try with 'Enter'
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
#include <HID-Project.h>
#include <HID-Settings.h>
#include <Joystick.h>

Joystick_ Joystick(JOYSTICK_DEFAULT_REPORT_ID,
  JOYSTICK_TYPE_GAMEPAD, 8, 0, // Buttons, Hat switch
  true, true, false, // X, Y, Z
  false, false, false, // Rx, Ry, Rz
  false, false, // Rudder, Throttle
  false, false, false); // Accelerator, Brake, Steering

unsigned long lastActionTime = 0;
unsigned long actionInterval = 10000;
unsigned long stickMoveInterval = 5000;

const int buttonCount = 8;
const int buttons[buttonCount] = {
  1, 2, 3, 4, // A, B, X, Y or Cross/Circle/Square/Triangle
  5, 6, 7, 8  // L1, R1, L2, R2 (can map as needed)
};

const char* messages[] = {
  "My goldfish is playing for me rn 🐠",
  "Keyboard on fire 🔥",
  "Beep boop I'm a bot",
  "I’m here but spiritually gone",
  "Haven’t blinked in 2 hours 👁️👁️",
  "Running on 3 FPS and dreams",
  "My cat is farming XP",
  "This is totally not a bot",
  "Using dial-up WiFi 📡",
  "I trained a squirrel to play for me 🐿️",
  "Send snacks pls 🍕",
  "Keyboard held hostage",
  "I'm running this on a toaster 🔌",
  "Currently in stealth mode 😎",
  "AI takeover starts now 🤖",
  "Mentally I'm in Minecraft",
  "Ping: 99999ms 🚨",
  "Respawning IRL",
  "My hamster unplugged the router",
  "Hard carrying my KD into the ground",
  "My aim is based on vibes only",
  "Stuck in third person view",
  "Every move is a jump scare 💀",
  "Error 404: Skill not found",
  "I only play with my eyes closed",
  "Fighting lag more than players",
  "Cursed loadout equipped",
  "Powered by coffee and regrets ☕",
  "This isn’t even my final form",
  "My dog queued for me 🐶",
  "Losing pixels by the second",
  "Mousepad is a pizza box",
  "Brain.exe has stopped working",
  "I'm just background noise rn",
  "I mapped shoot to sneeze",
  "Using Morse code to play",
  "This game runs on hopes and dreams ✨",
  "I blink and I die",
  "LAG IS MY SUPERPOWER",
  "Controller is held together by tape",
  "This is a cry for help but make it funny",
  "I can quit anytime I want 🫠",
  "Botting? No this is divine intervention"
};

const int messageCount = sizeof(messages) / sizeof(messages[0]);

void setup() {
  Joystick.begin();
  delay(3000);  // Give console time to detect input device
}

void loop() {
  unsigned long now = millis();

  if (now - lastActionTime > actionInterval) {
    moveStickRandomly();       // Simulate AFK movement
    pressRandomButton();       // Tap a random button

    if (random(0, 2)) {
      fakeChatSpam();          // Simulate text spam
    }

    lastActionTime = now;
  }
}

// Simulate thumbstick movement (right stick = camera, left = movement)
void moveStickRandomly() {
  int x = random(120, 135);  // Range around center 128 (±)
  int y = random(120, 135);
  Joystick.setXAxis(x);
  Joystick.setYAxis(y);
  delay(200);
  Joystick.setXAxis(128);
  Joystick.setYAxis(128);
}

// Simulate random button press
void pressRandomButton() {
  int b = buttons[random(0, buttonCount)];
  Joystick.pressButton(b - 1); // Buttons 0-7
  delay(100);
  Joystick.releaseButton(b - 1);
}

// Simulate console chat spam by "typing" one character at a time (some games support virtual keyboard)
void fakeChatSpam() {
  int index = random(0, messageCount);
  const char* msg = messages[index];

  for (int i = 0; msg[i] != '\0'; i++) {
    Joystick.setXAxis(127 + random(-3, 3));  // Slight motion
    Joystick.pressButton(1);  // Fake "type"
    delay(50);
    Joystick.releaseButton(1);
    delay(50);
  }

  // Fake 'Enter' button press
  Joystick.pressButton(2);  // Change to appropriate button if needed
  delay(100);
  Joystick.releaseButton(2);
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
