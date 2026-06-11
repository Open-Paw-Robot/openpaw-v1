# 🐾 OpenPaw Robot — V1 (ESP-ROLL Replica, Jul–Sep 2025)

The first generation of the **OpenPaw / PawMe** robot: a spherical, self-balancing
ball-bot with an ESP32 camera, which we replicated and built ourselves end-to-end
as the fastest path to a working AI-robot base.

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

## 📖 What Was Done (Development History)

**Timeline: 21 Jul 2025 → ~19 Sep 2025.**

- **21 Jul 2025** — project kickoff; Product Requirements Document written; the ESP-ROLL
  project chosen as the foundation (100 mm transparent sphere, ESP32-CAM/ESP32-Sense,
  DRV8833 motor driver, N20-style motors, 1000 mAh battery).
- **Jul–Aug 2025** — Kickstarter market research (Loona, EILIK, Rux, Pebby and other
  companion robots); first multimodal AI demo working (29 Jul).
- **22 Aug 2025** — firmware and hardware engineering team onboarded; "RollBot" demo running.
- **27 Aug–4 Sep 2025** — AI firmware milestone: the DFRobot OpenAI-QA example was rebuilt
  from scratch — audio transcription, image Q&A, and text-to-speech out of the robot's
  speaker all working. Key finding: OpenAI **Realtime** required ESP-IDF while the QA code
  was Arduino-based, so the two could not be merged in this generation.
- **5 Sep 2025** — web UI with record/stop control and the ability to toggle between the
  ESP-ROLL driving firmware and the OpenAI-QA firmware.
- **18 Sep 2025** — one fully assembled ESP-ROLL unit hand-built ("with a lot of tape, glue
  and adhesives") and shipped to Hong Kong.
- **20 Sep 2025** — **end of V1**: the original project's CAD files turned out to be
  uneditable and under-dimensioned — parts didn't fit ("near impossible to use its 3D files
  and build on top of that"). Decision taken to redesign all mechanical parts from scratch
  → [V2](https://github.com/Open-Paw-Robot/openpaw-v2).

## 📁 Repository Layout

| Folder | Contents |
|:---|:---|
| `Mechanical/` | 3D-printed parts — see the Cults3D links above for the author's STLs |
| `Electrical/Schematics/` | Full wiring schematic of the ESP-ROLL spherical robot |
| `Electrical/PCB Gerbers/Main Board/` | Main board Gerbers + JLCPCB BOM & pick-and-place files |
| `Electrical/PCB Gerbers/LED Ring Light Board/` | LED ring light board Gerbers |
| `Firmware/ESP32-CAM_MJPEG2SD (as used in video)/` | ESP32 firmware snapshot used in the build |
| `Design/` | Industrial design & renders |
| `Docs/` | Firmware requirements, project requirement document & project plan |

## ⚠️ Missing Files (known to exist, not yet in this repo)

- **`RollBot` firmware repo** — the working V1 driving + AI firmware lived at
  `github.com/aeropriest/RollBot` (referenced 22 Aug 2025). Needs to be imported or linked.
- **`OPEN_AI_QA` firmware** — the rebuilt OpenAI question-answering firmware was pushed to a
  separate GitHub repo (5–6 Sep 2025); not yet mirrored here.
- **STL files** — only available via the author's Cults3D listings above (account required);
  our own print-ready copies from the build are not archived here.
- **PRD (Product Requirements Document)** — lives as a Google Doc in the team Drive (21 Jul 2025).
- **Build media** — assembly photos, wiring diagrams and demo videos are archived in the team
  Google Drive (`5. Product/History/WhatsApp Chat - Rolling Robot - Pawme/` and
  `5. Product/ESP-32 Roll + ChatGPT/`), including a video transcription of the
  ESP-32-Ball + ChatGPT replication.

## 🤖 Other Versions

- [openpaw-v2](https://github.com/Open-Paw-Robot/openpaw-v2) — custom rolling robot (own mechanicals + custom PCBA)
- [openpaw-v3](https://github.com/Open-Paw-Robot/openpaw-v3) — **current generation** (two-wheeled expressive companion)

## 📜 License

- Hardware design files (schematic, Gerbers, BOM): **CC BY-NC-SA 4.0** © Max Imagination
- Firmware (`ESP32-CAM_MJPEG2SD`): **AGPL-3.0** © s60sc (see bundled `LICENSE`)

---

*Part of the OpenPaw project — open-source AI companion robot for the whole family.*
