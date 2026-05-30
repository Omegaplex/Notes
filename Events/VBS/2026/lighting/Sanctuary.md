VBS LED Installation Summary

This document summarizes the three planned LED installations: booth lights, light wall, and ceiling lights. Each install uses a separate 24 V power supply, controller, enclosure, and DC branch protection.

Overall Assignment

Install| Location / Purpose| Light Type| Controller| Power Supply| Breaker
Booth lights| Around the sound booth| 16 ft WS2814 addressable strip| ESP32 WLED controller| 24 V 8 A PSU| 6 A breaker
Light wall| 8 tall × 12 wide milk-jug wall| 24 V WS2811 pixel lights| ESP32 WLED controller| 24 V 6 A PSU| 4 A breaker
Ceiling lights| Sanctuary ceiling lighting| 24 V analog 5050 RGB strips, two 50 ft runs| LS8P-Dual-WLED| 24 V 6 A PSU| 3 A breaker

---

Booth Lights

Summary

The booth lights are a 16 ft WS2814 addressable LED strip installed around the sound booth. This install uses the largest power supply, the 24 V 8 A brick, and a 6 A DC breaker. Control will be through one ESP32 running WLED.

Booth Lights Parts Table

Item| Status| Purpose / Notes
16 ft WS2814 LED strip| Purchased / known| Main addressable strip around the sound booth
ESP32 WLED controller| Purchased / already have| Controls the WS2814 strip through WLED
24 V 8 A power supply| Purchased| Main power supply for booth lights
DIYhz 6 A thermal circuit breaker| Purchased| DC branch protection for the booth light circuit
Waterproof/project box| Purchased| Enclosure for controller, breaker, and wiring
IP68 cable gland kit| Purchased| Cable entry into the project box
Wagos| Already have| Internal DC splicing and distribution
Cable clips| Purchased| Cable support and routing

Booth Lights Basic Layout

24 V 8 A power supply
    ↓
Cable gland into project box
    ↓
6 A breaker
    ↓
DC distribution / Wagos
    ├── ESP32 WLED controller power
    └── WS2814 strip power

ESP32 data output
    ↓
WS2814 strip data input

---

Light Wall

Summary

The light wall is the 8 tall × 12 wide milk-jug wall using one WS2811 pixel per jug. The planned layout uses 96 pixels total. Two 50-pixel strings provide 100 pixels, leaving 4 spare pixels.

This install uses a 24 V 6 A power supply, a 4 A DC breaker, and an ESP32 WLED controller.

Light Wall Parts Table

Item| Status| Purpose / Notes
ALITOVE 24 V WS2811 LED pixel lights| Purchased| Main pixels for the milk-jug light wall
Two 50-pixel strings| Purchased / planned| 100 pixels total; 96 used and 4 spare
ESP32 WLED controller| Purchased / already have| Controls the WS2811 pixel strings through WLED
24 V 6 A power supply| Purchased / already have| Main power supply for the light wall
DIYhz 4 A thermal circuit breaker| Purchased| DC branch protection for the light wall
Waterproof/project box| Purchased| Enclosure for controller, breaker, and wiring
IP68 cable gland kit| Purchased| Cable entry into the project box
Wagos| Already have| Internal DC splicing and distribution
Cable clips| Purchased| Cable support and routing

Light Wall Basic Layout

24 V 6 A power supply
    ↓
Cable gland into project box
    ↓
4 A breaker
    ↓
DC distribution / Wagos
    ├── ESP32 WLED controller power
    └── WS2811 pixel string power

ESP32 data output
    ↓
WS2811 pixel string data input
    ↓
8 tall × 12 wide milk-jug layout

Light Wall Pixel Layout

Planned physical layout: serpentine pattern.

Row 1:   1  → 12
Row 2:  24 ← 13
Row 3:  25 → 36
Row 4:  48 ← 37
Row 5:  49 → 60
Row 6:  72 ← 61
Row 7:  73 → 84
Row 8:  96 ← 85

---

Ceiling Lights

Summary

The ceiling lights use 24 V analog 5050 RGB LED strips. The known strip total is 100 ft, planned as two parallel 50 ft runs. The total load is known as 36 W, which is approximately 1.5 A at 24 V.

This install uses a 24 V 6 A power supply, a 3 A DC breaker, and the LS8P-Dual-WLED controller.

Ceiling Lights Parts Table

Item| Status| Purpose / Notes
24 V analog 5050 RGB LED strips| Purchased / known| Main ceiling lighting
100 ft total strip length| Purchased / known| Planned as two parallel 50 ft runs
LS8P-Dual-WLED| Purchased| WLED control for the analog RGB ceiling strips
24 V 6 A power supply| Already have| Main power supply for the ceiling lights
DIYhz 3 A thermal circuit breaker| Purchased| DC branch protection for the ceiling light circuit
Waterproof/project box| Purchased| Enclosure for controller, breaker, and wiring
IP68 cable gland kit| Purchased| Cable entry into the project box
Wagos| Already have| Internal DC splicing and distribution
Cable clips| Purchased| Cable support above the drop ceiling

Ceiling Lights Basic Layout

24 V 6 A power supply
    ↓
Cable gland into project box
    ↓
3 A breaker
    ↓
LS8P-Dual-WLED
    ├── 50 ft RGB strip run #1
    └── 50 ft RGB strip run #2

---

Shared Network Equipment

Summary

All three lighting installs will run on a dedicated local WLED Wi-Fi network. Internet is not required. The router will be used only to let the controllers and sound-booth PC communicate with each other.

Shared Equipment Table

Item| Status| Purpose / Notes
TP-Link Archer A54 / AC1200 router| Purchased| Dedicated WLED Wi-Fi network
Sound-booth PC Wi-Fi adapter| Purchased / planned| Connects the PC to the WLED network
ESP32 WLED controller #1| Purchased / already have| Assigned to booth lights
ESP32 WLED controller #2| Purchased| Assigned to light wall
LS8P-Dual-WLED| Purchased| Assigned to ceiling lights

Network Layout

TP-Link Archer A54 WLED Wi-Fi network
    ├── Booth lights: ESP32 WLED controller
    ├── Light wall: ESP32 WLED controller
    └── Ceiling lights: LS8P-Dual-WLED

---

Power Supply Summary

Install| Power Supply| Breaker| Notes
Booth lights| 24 V 8 A| 6 A| Largest supply assigned to the WS2814 strip
Light wall| 24 V 6 A| 4 A| Powers 96 WS2811 pixels with 4 spare pixels available
Ceiling lights| 24 V 6 A| 3 A| Ceiling strip load is about 1.5 A based on 36 W total

---

Current Notes

- All power supplies are external power bricks.
- Low-voltage DC enters each project box through cable glands.
- Each install has its own breaker.
- Wagos can be used for internal DC distribution inside the boxes.
- Cable clips are for supporting cable runs and keeping wiring off the drop ceiling.
- Black stage foil / cinefoil is not currently included due to budget.
