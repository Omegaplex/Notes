# LED Installation Summary for Sanctuary 

This document summarizes the three planned LED installations:

- Booth lights
- Light wall
- Ceiling lights

Each installation uses its own 24 V power supply, controller, enclosure, and DC branch protection.

---

## Overall Assignment

| Install | Location / Purpose | Light Type | Controller | Power Supply | Breaker |
|---|---|---|---|---|---|
| Booth lights | Around the sound booth | 16 ft WS2814 addressable strip | ESP32 WLED controller | 24 V 8 A PSU | 6 A breaker |
| Light wall | 8 tall × 12 wide milk-jug wall | 24 V WS2811 pixel lights | ESP32 WLED controller | 24 V 6 A PSU | 4 A breaker |
| Ceiling lights | Sanctuary ceiling lighting | 24 V analog 5050 RGB strips, two 50 ft runs | LS8P-Dual-WLED | 24 V 6 A PSU | 3 A breaker |

---

## Booth Lights

### Summary

The booth lights are a 16 ft WS2814 addressable LED strip installed around the sound booth. This installation uses the 24 V 8 A power supply, a 6 A DC breaker, and one ESP32 WLED controller.

### Parts Table

| Item | Purpose / Notes |
|---|---|
| 16 ft WS2814 LED strip | Main addressable strip around the sound booth |
| ESP32 WLED controller | Controls the WS2814 strip through WLED |
| 24 V 8 A power supply | Main power supply for booth lights |
| DIYhz 6 A thermal circuit breaker | DC branch protection for the booth light circuit |
| Waterproof/project box | Enclosure for controller, breaker, and wiring |
| IP68 cable gland kit | Cable entry into the project box |
| Wagos | Internal DC splicing and distribution |
| Cable clips | Cable support and routing |

### Basic Layout

```text
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
```

---

## Light Wall

### Summary

The light wall is the 8 tall × 12 wide milk-jug wall using one WS2811 pixel per jug. The planned layout uses 96 pixels total. Two 50-pixel strings provide 100 pixels, leaving 4 spare pixels.

The face of the light wall will be the base of each milk jug, not the full side height of the jug. Based on an estimated 5.5 in to 6 in square jug base, the lighted area is expected to be about 5.5 ft to 6 ft wide by about 3.7 ft to 4 ft tall, before adding any frame, border, rail, or spacing allowance.

### Estimated Physical Dimensions

| Dimension | Estimate | Notes |
|---|---:|---|
| Layout | 12 wide × 8 tall | 96 total jug faces |
| Visible face | Jug base | The bottom/base of each milk jug faces forward |
| Estimated jug base width | 5.5 in to 6 in | Varies by jug style |
| Estimated jug base height | 5.5 in to 6 in | Treating the base as roughly square |
| Estimated lighted width | 66 in to 72 in | 12 jugs × 5.5-6 in |
| Estimated lighted height | 44 in to 48 in | 8 jugs × 5.5-6 in |
| Estimated lighted size | About 5.5 ft to 6 ft wide × 3.7 ft to 4 ft tall | Actual size depends on jug base and spacing |
| Practical finished size | About 6 ft wide × 4 ft tall, plus frame/border | Good planning estimate before final measuring |

### Parts Table

| Item | Purpose / Notes |
|---|---|
| ALITOVE 24 V WS2811 LED pixel lights | Main pixels for the milk-jug light wall |
| Two 50-pixel strings | 100 pixels total; 96 used and 4 spare |
| ESP32 WLED controller | Controls the WS2811 pixel strings through WLED |
| 24 V 6 A power supply | Main power supply for the light wall |
| DIYhz 4 A thermal circuit breaker | DC branch protection for the light wall |
| Waterproof/project box | Enclosure for controller, breaker, and wiring |
| IP68 cable gland kit | Cable entry into the project box |
| Wagos | Internal DC splicing and distribution |
| Cable clips | Cable support and routing |

### Basic Layout

```text
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
```

### Pixel Layout

Planned physical layout: serpentine pattern.

```text
Row 1:   1  → 12
Row 2:  24 ← 13
Row 3:  25 → 36
Row 4:  48 ← 37
Row 5:  49 → 60
Row 6:  72 ← 61
Row 7:  73 → 84
Row 8:  96 ← 85
```

---

## Ceiling Lights

### Summary

The ceiling lights use 24 V analog 5050 RGB LED strips. The known strip total is 100 ft, planned as two parallel 50 ft runs. The total load is known as 36 W, which is approximately 1.5 A at 24 V.

This installation uses a 24 V 6 A power supply, a 3 A DC breaker, and the LS8P-Dual-WLED controller.

### Parts Table

| Item | Purpose / Notes |
|---|---|
| 24 V analog 5050 RGB LED strips | Main ceiling lighting |
| 100 ft total strip length | Planned as two parallel 50 ft runs |
| LS8P-Dual-WLED | WLED control for the analog RGB ceiling strips |
| 24 V 6 A power supply | Main power supply for the ceiling lights |
| DIYhz 3 A thermal circuit breaker | DC branch protection for the ceiling light circuit |
| Waterproof/project box | Enclosure for controller, breaker, and wiring |
| IP68 cable gland kit | Cable entry into the project box |
| Wagos | Internal DC splicing and distribution |
| Cable clips | Cable support above the drop ceiling |

### Basic Layout

```text
24 V 6 A power supply
    ↓
Cable gland into project box
    ↓
3 A breaker
    ↓
LS8P-Dual-WLED
    ├── 50 ft RGB strip run #1
    └── 50 ft RGB strip run #2
```

---

## Shared Network Layout

All three lighting installations will run on a dedicated local WLED Wi-Fi network. Internet is not required. The router will be used so the controllers and sound-booth PC can communicate with each other.

```text
TP-Link Archer A54 WLED Wi-Fi network
    ├── Booth lights: ESP32 WLED controller
    ├── Light wall: ESP32 WLED controller
    └── Ceiling lights: LS8P-Dual-WLED
```

---

## Current Notes

- All power supplies are external power bricks.
- Low-voltage DC enters each project box through cable glands.
- Each installation has its own breaker.
- Wagos can be used for internal DC distribution inside the boxes.
- Cable clips are for supporting cable runs and keeping wiring off the drop ceiling.
