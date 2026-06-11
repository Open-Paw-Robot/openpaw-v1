# 🐾 OpenPaw Robot — V1 (Spherical Self-Balancing Prototype)

The first generation of the **OpenPaw / PawMe** robot: a spherical, self-balancing
ball-bot with an ESP32 camera, which we replicated and built ourselves end-to-end.

## 🙏 Credits & Origin

**V1 is a faithful replication of the outstanding open project
[ESP-ROLL: Build a Spherical Self-balancing Robot With ESP32 Camera!](https://www.instructables.com/ESP-ROLL-Build-a-Spherical-Self-balancing-Robot-Wi/)
by [Max Imagination](https://www.instructables.com/member/Max%20Imagination/).**

All design files in this repository (schematic, PCB Gerbers, BOM, assembly files, and the
firmware snapshot) originate from Max Imagination's project and are redistributed here with
attribution under the original license:
[**CC BY-NC-SA 4.0** (Attribution-NonCommercial-ShareAlike)](https://creativecommons.org/licenses/by-nc-sa/4.0/).
Huge thanks to Max Imagination for open-sourcing the project that kicked off this robot. ❤️

The firmware is based on [s60sc/ESP32-CAM_MJPEG2SD](https://github.com/s60sc/ESP32-CAM_MJPEG2SD)
(AGPL-3.0) — the snapshot included here is the version used in the original build video and is
**not** up to date with the upstream repo.

3D-printable STL files are distributed by the original author on Cults3D:

- [ESP-ROLL — ESP32 spherical robot with camera (STL files)](https://cults3d.com/en/3d-model/game/esp-roll-an-esp32-spherical-robot-with-camera-rc-ball-bot-3d-design-stl-fil-e83bfe979989d6ad6f66)
- [ESP-ROLL — FPV ESP32 spherical robot (STL files)](https://cults3d.com/en/3d-model/game/esp-roll-an-fpv-esp32-spherical-robot-rc-ball-bot-3d-design-stl-files)

## 📁 Repository Layout

| Folder | Contents |
|:---|:---|
| `Mechanical/` | 3D-printed parts — see the Cults3D links above for the author's STLs |
| `Electrical/Schematics/` | Full wiring schematic of the ESP-ROLL spherical robot |
| `Electrical/PCB Gerbers/Main Board/` | Main board Gerbers + JLCPCB BOM & pick-and-place files |
| `Electrical/PCB Gerbers/LED Ring Light Board/` | LED ring light board Gerbers |
| `Firmware/ESP32-CAM_MJPEG2SD (as used in video)/` | ESP32 firmware snapshot used in the build |
| `Design/` | Industrial design & renders |
| `Docs/` | Build notes & documentation |

## 🤖 Other Versions

- [openpaw-v2](https://github.com/Open-Paw-Robot/openpaw-v2) — second prototype
- [openpaw-v3](https://github.com/Open-Paw-Robot/openpaw-v3) — **current generation**

## 📜 License

- Hardware design files (schematic, Gerbers, BOM): **CC BY-NC-SA 4.0** © Max Imagination
- Firmware (`ESP32-CAM_MJPEG2SD`): **AGPL-3.0** © s60sc (see bundled `LICENSE`)

---

*Part of the [Open-Paw-Robot](https://github.com/Open-Paw-Robot) organization — open-source AI companion robot for the whole family.*
