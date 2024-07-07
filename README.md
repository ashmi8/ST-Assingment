# ST-Assingment

# Ball Tracking and Event Logging with Computer Vision

This project demonstrates a Python-based solution for tracking colored balls across different quadrants in a video using Computer Vision techniques. It detects ball movements, logs entry and exit events for each quadrant, and outputs both a processed video and event logs.

## Features

- **Ball Detection**: Uses HSV color space to detect balls of predefined colors (red, blue, green) in each frame.
- **Quadrant Tracking**: Divides the video frame into four quadrants and tracks ball movements across these regions.
- **Event Logging**: Records the timestamp, quadrant number, ball color, and event type (entry or exit) for each detected ball movement.
- **Visual Feedback**: Draws bounding boxes around detected balls and displays event types on the processed video.
- **Output**: Generates a processed video (`output.avi`) with visual annotations and saves event logs to `event_log.txt`.

## Usage

### Requirements

- Python 3.x
- OpenCV (`pip install opencv-python`)
- NumPy (`pip install numpy`)

### Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your_username/ball-tracking.git
   cd ball-tracking
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Program:**
   ```bash
   python ball_tracking.py --video video.mp4
   ```

   Replace `video.mp4` with the path to your input video file.

4. **Output:**
   - Processed Video: `output.avi`
   - Event Logs: `event_log.txt`

### Customization

- Modify `colors` dictionary in `ball_tracking.py` to detect additional or different colored balls.
- Adjust quadrant boundaries in `ball_tracking.py` (`quadrants` list) based on your video's dimensions.

## Notes

- Ensure your video file is accessible and correctly specified in the command line argument.
- This program assumes the video has clear and distinct ball colors against a relatively uniform background.

