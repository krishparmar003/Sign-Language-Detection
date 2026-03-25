# Sign Language Detection

Real-time ASL detector that recognizes **A-Z letters and 0-9 digits** via webcam.

Built with MediaPipe, OpenCV, and scikit-learn.

---

## How it works

1. **Collect** — Captures hand images via webcam for each sign
2. **Extract** — MediaPipe detects 21 hand landmarks per frame
3. **Train** — Random Forest Classifier trained on the landmark coordinates
4. **Detect** — Real-time prediction overlaid on the webcam feed

<img width="408" height="329" alt="outputt" src="https://github.com/user-attachments/assets/f3d32645-b635-4220-8805-23ab5acddb2c" />

---

## Setup

```bash
git clone https://github.com/krishparmar003/Sign-Language-Detection.git
cd Sign-Language-Detection
pip install -r requirements.txt
```

Run the notebook cells in order:
1. `Collect Imgs` — collect training data via webcam
2. `Dataset` — extract hand landmarks using MediaPipe
3. `Train Classifier` — train the Random Forest model
4. `Inference` — run real-time detection

---
## Tech Stack
- **Hand Detection** — MediaPipe (21 landmarks per hand)
- **Classifier** — Random Forest (scikit-learn)
- **Camera/Video** — OpenCV

---


<img width="480" height="679" alt="a-z 0-9" src="https://github.com/user-attachments/assets/9c882413-6aad-4a53-82bc-a256b78d5a85" />


*Based on work by Computer Vision Developer — MIT License*

