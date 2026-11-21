# BLUEWATER — Flight Sandbox

A browser-based, non-combat 3D flight sandbox featuring real-scale models of the F/A-18E Super Hornet and F-35C Lightning II, a Nimitz-class-scale aircraft carrier (angled deck, catapults, arresting wires), procedural ocean, distant islands and clouds.

## Run locally

Open `index.html` in a modern browser with an internet connection. Three.js is loaded from jsDelivr at runtime, so no build step or package installation is needed.

## Controls

| Key | Action |
| --- | --- |
| W / S | Increase / decrease throttle |
| Arrow Up / Down | Pitch |
| A / D | Bank |
| Q / E | Rudder while on deck |
| C | Switch chase / cockpit camera |
| R | Reset to deck |
| F | Fire bow catapult (when stopped at the catapult) |
| Space | Airbrake |
| Esc | Pause / resume |

## Aircraft and scale

- **F/A-18E Super Hornet**: 18.3 m long, 13.6 m span, twin canted fins, LEX, side intakes.
- **F-35C Lightning II**: 15.7 m long, 13.1 m span, single engine, DSI intakes, canted fins.
- **Carrier**: ~333 m long, 76 m flight deck about 20 m above the sea, 9 degree angled deck with four arresting wires, two bow catapults, island and elevators.

The jets are procedural models built to published dimensions. Press F on the catapult to launch (0 to 150 kt in about 2 s). Land on the angled deck to catch a wire. Gear retracts after takeoff. No weapons or combat.

### Using real 3D models
Put your own openly licensed models at `models/f18.glb` and `models/f35.glb`. They are auto-scaled to real length and used instead of the procedural jets. Check each model's license first.

## Deploy to Vercel

This is a static site. Import the repository into Vercel with the project root set to the repository root. No framework, build command or output directory is required.
