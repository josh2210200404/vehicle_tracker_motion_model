# vehicle_tracker_motion_model

## About the Project
This project implements a single vehicle tracking system using YOLOv8 object detection and a Constant Velocity Motion Model.

The system tracks one selected target vehicle across video frames and predicts its next position using motion estimation.

---

## Features
- Single vehicle tracking
- YOLOv8 based car detection
- Constant velocity motion prediction
- Bounding box visualization
- Tracker confidence display
- Motion model confidence display
- Trusted source indication
- Stable tracking of one selected vehicle only

---

## Technologies Used
- Python
- OpenCV
- YOLOv8 (Ultralytics)

---

## Input
- Video file (`car3.mp4`)
- Initial target car selected from first frame

---

## Output
For every frame, the system displays:
- Bounding box (x, y, width, height)
- Tracker confidence
- Motion model confidence
- Trusted output source
- Predicted next position

---

## Project Architecture

1. YOLOv8 detects vehicles in video frames.
2. One target car is selected.
3. Distance and size matching are used to keep tracking the same vehicle.
4. Constant velocity motion model predicts next vehicle position.
5. Tracker and motion model outputs are combined for stable tracking.

---

## How to run

1. Install dependencies
2. Upload video file
3. Run notebook/code
4. Output video with tracked vehicle is generated as `output.mp4`

---

## Build Instructions

1. Open Google Colab or Jupyter Notebook.
2. Install required dependencies.
3. Upload the input video file.
4. Run all notebook cells sequentially.
5. The tracked output video will be generated automatically.

---

## Dependency List

Required Python libraries:

- ultralytics
- opencv-python
- math

Install dependencies using:

```bash
  pip install ultralytics opencv-python
```

---

## Repository Contents

- `BonV_assessment.ipynb` → Main notebook
- `BonV assessment 2-Josh.pdf` → PDF report/output

---

## Video Links

- Input Video:
  https://drive.google.com/file/d/1O9x-tMK2bZ6KdtGHbHneSJebQoeAAfwr/view?usp=drive_link
- Output Video:
  https://drive.google.com/file/d/1raehxIDRwysgNjXcDoYQWi1i7ry5ssRx/view?usp=drive_link

---

## Final Tracking Output
The system successfully tracks a single target vehicle continuously while avoiding switching to nearby vehicles.
