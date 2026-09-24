# Invisibility Cloak

A real-time invisibility cloak effect using OpenCV — wear something blue, and it's replaced by the background, making you appear invisible.

## How It Works

Captures a clean background from empty frames, then masks out blue pixels in each frame and replaces them with the corresponding background pixels.

## Requirements

- Python 3, `opencv-python`, `numpy`
- A webcam
- A solid blue cloth/shirt as the "cloak"

## Install & Run

```bash
pip install opencv-python numpy
python main.py
```

Step out of frame when it starts (background capture), then step back in wearing blue. Press `q` to quit.

## Tips

- Adjust `lower_blue` / `upper_blue` in `main.py` if detection is poor for your lighting/fabric.
- Stay still during the initial background capture to avoid artifacts.
