# Video Frame Keypoint Detection and Tracking

This project was *completed as part of AIML331* at Te Herenga Waka — Victoria University of Wellington.

## Objective:
 - Part 1: Sparse keypoint detection and tracking using SIFT.
 - Part 2: Dense tracking using optical flow (Lucas-Kanade).
 - Part 3: Object tracking with initial bounding box using both methods.

## Data
- `data/` - Contains 69 consecutive video frames of a race car.

## Structure
- `01_sparse_keypoints.ipynb` – Extracts the SIFT descriptors and keypoints from each frame, matches keypoints between consecutive frames, and visualises tracked keypoints.
- `02_dense_optical_flow.ipynb` – Computes the dense optical flow between consecutive frames using the Lucas-Kanade method and visualises the motion vectors.
- `03_object_tracking_sift.ipynb` – Tracks a bounding box around the race car using SIFT keypoints.
- `04_object_tracking_optical_flow.ipynb` – Tracks a bounding box around the race car using dense optical flow.

## Results
- Visualisation images are saved for every fifth frame to reduce file clutter, and are available in `results/`.
- Sparse keypoint tracking: lines connecting keypoints across consecutive frames.
- Dense optical flow: arrows showing motion vectors across frames.
- Bounding box tracking: updated bounding boxes over frames showing tracked car.

## How to Run:
```bash
pip install -r requirements.txt
jupyter notebook
# Open the notebooks in numerical order and run all cells
```
