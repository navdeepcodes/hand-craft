# Hand Craft

A hand-tracked visual playground that runs entirely in your browser. Your camera feed never leaves your device: hand and face tracking run locally with [MediaPipe Tasks Vision](https://developers.google.com/mediapipe/solutions/vision/hand_landmarker).

## Modes

**✦ Aura**: cast light with your hands.

| Gesture | Effect |
|---|---|
| ✋ Open palm | A sigil that draws itself and tilts with your palm |
| 🤏 Pinch and move | Paint with light |
| ☝️ Point | Fire stream |
| ✊ Fist, then open | Charge ring, then a blast |
| 🙌 Both palms | Portal with a star tunnel |
| ☝️☝️ Both point | Lightning |

**◈ Mesh**: an elastic net you make with your fingers.

| Gesture | Effect |
|---|---|
| 🤏 Pinch, then spread | A mesh forms between your thumb and index |
| ↔️ Spread or close those fingers | Bigger or smaller (turn your hand to turn it) |
| 🤏 Close your fingers on it | Grab it and carry it, then open your fingers to drop it (fast = throw) |
| ✊ Fist while holding it | It bursts and vanishes |
| 🙂 Drop it on your face | Wear it as a mask fitted to your face (pinch it to take it off) |
| 🙌 Pinch with both hands | Stretch and rotate |

A built-in step-by-step coach teaches each mode the first time you open it. Restart it with the 🎓 button.

**Keys:** `M` mode · `G` mesh shape · `1`–`4` palette · `V` camera · `S` skeleton · `L` labels · `H` guide · `C` clear · `P` snapshot

## Run locally

The camera only works over `https` or `localhost`:

```bash
python3 -m http.server 5173
```

Then open http://localhost:5173.

It's a single static file (`index.html`) with no build step.
