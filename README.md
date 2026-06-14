# Lily58 - Wireless

An ergonomic, split mechanical keyboard with a 58-key columnar-staggered layout, derived from the original [Lily58](https://github.com/kata0510/Lily58). This specific variant is optimized for wireless dual-mode connectivity and ultra-low-power Nice!View displays, perfect for developers and creators seeking a clean, cable-free workspace.

## Features

- **Ergonomic Columnar Layout**: 4x12 matrix with 5 thumb keys per side (58 keys total) reduces finger travel and hand strain.
- **Wireless-Ready**: Integrated battery support for seamless Bluetooth operation when paired with BLE controllers (e.g., nice!nano).
- **Nice!View Optimization**: Native compatibility with the low-power Sharp Memory Display (Nice!View), offering a high refresh rate with a fraction of the power consumption of traditional OLEDs.
- **Reversible PCB Design**: Uses a mirrored, flippable design for the left and right sides to simplify manufacturing and sourcing.
---

## Bill of Materials (BOM)

Below is the complete list of components required to build one full TsunyYu - Lily58 keyboard (including both left and right halves):

| Item | Quantity | Model/Specification / Notes |
| --- | --- | --- |
| **Lily58 PCB** | 2 | Left and right halves (reversible design) |
| **PCB Plate** | 2 | Left and right halves (compatible with 58-key layout) |
| **Microcontroller** | 2 | Pro Micro or compatible BLE wireless controllers (e.g., nice!nano) |
| **Tulip Socket** | 2 | SINGLE STRIP ROW 40 CONTACTS, PITCH = 2.54mm |
| **Machined Pin Header** | 2 | Single row 30 contacts, 2.54mm Round Pin Header |
| **Display** | 2 | Nice!View (Ultra-low-power display; backward compatible with 0.91" OLED) |
| **Square Pin Socket** | 2 | 1x5 Female Header |
| **M2 Screw** | 10 | M2x6mm |
| **M2 Spacer** | 10 | |
| **Key Socket** | 58 | Kailh Hotswap Sockets |
| **Switches** | 58 | MX switches |
| **Keycaps** | 58 | 1U keycaps recommended, 1.5U (2) optional for thumb keys |
| **Diodes** | 58 | 1N4148W (SOD-123) |
| **Batteries** | 2 | 3.7V Li-Po batteries (Required for wireless; 110mAh to 300mAh recommended) |
| **Battery Holders** | 2 | Molex 53621-0271 1.25mm 2p |
| **Reset Buttons** | 2 | C&K PTS636 SMT G leads 2.5mm height |

---

## Hardware & Soldering Guide

Please review these critical steps before heating up your soldering iron:

1. **Orientation Check**: Because the PCB is reversible, make sure you clearly identify the "Left" and "Right" sides before soldering any components. Do not accidentally mirror the components on the same side.
2. **Diode Polarity**: Diodes are directional. Ensure the line on the diode (cathode) aligns with the thick line/bar indicated on the PCB silkscreen markings.
3. **Wireless Safety Precautions**:
   - It is highly recommended to apply **insulating tape** (like Kapton tape) over the PCB traces beneath the microcontroller to prevent shorts between the controller pins and the PCB components/battery.
   - Pay close attention to the pinout when installing the Nice!View. It requires 5 pins (including a CS pin), differing slightly from standard 4-pin OLED setups.

---

## Firmware Support

This build is fully compatible with open-source keyboard firmwares:

- **ZMK Firmware**: The ideal choice when paired with nice!nano controllers. It natively handles Bluetooth multi-device pairing and unlocks the full low-power efficiency of the Nice!View screen.

---

## References & Credits

This project is built upon and inspired by the incredible open-source work of the mechanical keyboard community:

- [kata0510/Lily58](https://github.com/kata0510/Lily58) - The original Lily58 design.
- [ZMK Firmware](https://zmk.dev/) & [nice!nano](https://nicekeyboards.com/) - Providing the robust ecosystem for wireless split keyboards.

---

## License

This hardware project is open-source and distributed under the same licensing terms as the original repository:
- **Distributed under the [MIT License](LICENSE)** *(Or specify CERN OHL if applicable to your custom PCB modifications).*
