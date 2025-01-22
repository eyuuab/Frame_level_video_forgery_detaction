# Video Tampering Detection

This project analyzes video frame differences to detect potential tampering, such as duplicate or frozen frames. Using OpenCV and NumPy, the script compares a tampered video with a real video and visualizes the results.

---

## Method

The script uses **frame difference analysis**:
1. Convert each video frame to grayscale to simplify processing.
2. Calculate the absolute difference between consecutive frames.
3. Count the number of non-zero pixels in the difference to measure changes.
4. Flag frames with minimal changes (below a threshold) as potential duplicates or frozen frames.

This approach highlights anomalies that may indicate video tampering.

---

## Requirements

- Python 3.x
- Required Libraries:
  - OpenCV (`cv2`)
  - NumPy (`numpy`)
  - Matplotlib (`matplotlib`)

Install dependencies using:
```bash
pip install opencv-python-headless numpy matplotlib
