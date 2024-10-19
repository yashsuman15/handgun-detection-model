# Weapon Detection Program

This project implements a real-time weapon detection system using YOLOv11 and OpenCV. It processes video input to detect weapons (specifically guns) and draws bounding boxes around them with confidence scores.

## Features

- Real-time weapon detection using YOLOv11
- Processes video files or live camera feed
- Draws bounding boxes around detected weapons
- Displays class name (GUN) and confidence score for each detection
- Adjustable confidence threshold for detections

## Requirements

- Python 3.11
- OpenCV (`cv2`)
- Ultralytics YOLO (`ultralytics`)
- cvzone

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yashsuman15/weapon-detection.git
   cd weapon-detection
   ```

2. Install the required packages:
   ```
   pip install opencv-python ultralytics cvzone
   ```

3. Download the YOLOv8 weights file trained for weapon detection and place it in the `runs/detect/train3/weights/` directory.

## Usage

1. Update the paths in the script:
   - Set the correct path for the YOLOv11 weights file
   - Set the correct path for the input video file, or use `0` for live camera feed

2. Run the script:
   ```
   python weapon_detection.py
   ```

3. The program will open a window showing the processed video with bounding boxes around detected weapons. Press 'q' to quit the application.

## Customization

- Adjust the `confidence` threshold in the script to fine-tune detection sensitivity (currently set to 0.2)
- Modify the `class_name` variable if you want to detect other objects besides guns
- Change the color scheme for bounding boxes and text as needed

## Important Notes

- This program is designed for educational and research purposes only.
- Ensure you comply with all local laws and regulations regarding weapon detection systems.
- The accuracy of the detection depends on the quality of the trained model and input video.

## Contributing

Contributions to improve the project are welcome. Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## License

[Specify your license here, e.g., MIT License, GPL, etc.]

## Acknowledgments

- [Ultralytics](https://github.com/ultralytics/ultralytics) for the YOLOv8 implementation
- [cvzone](https://github.com/cvzone/cvzone) for enhanced OpenCV utilities

## Disclaimer

This software is provided for educational and research purposes only. The authors and contributors are not responsible for any misuse or illegal use of this software. Users are solely responsible for ensuring their use of this software complies with all applicable laws and regulations.
