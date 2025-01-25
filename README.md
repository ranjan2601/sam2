
# Hand Movement Masking Using SAM2, Torch, and Torchvision

## Features
- **Mask Generation**: Leverages SAM2 (Segment Anything Model) for generating segmentation masks.
- **Frame-by-Frame Processing**: Extracts frames from a video and processes them individually.
- **Integration with Torch and Torchvision**: Efficient handling of video data and deep learning operations.
- **Google Colab Support**: Ready-to-run on Colab for ease of use and reproducibility.

## Requirements
Ensure the following dependencies are installed:

- Python 3.12
- torch
- torchvision
- supervision
- opencv-python (cv2)
- google.colab (if running on Colab)

Install the dependencies using:
```bash
pip install torch torchvision supervision opencv-python
```

## Getting Started

1. Clone the repository:
   
```bash
   git clone https://github.com/ranjan2601/sam2.git
   cd sam2
```

2. Upload your video file to the project directory.

3. Run the hand_movement.ipynb file on Google Colab or your local Jupyter Notebook environment.

### Steps in the Notebook

1. **Setup Environment**:
   The first cell contains the code to install SAM2 and its dependencies. Ensure to enable GPU acceleration in Google Colab for faster processing (Runtime > Change runtime type > Hardware accelerator > GPU).

2. **Video Loading**:
   The script reads the input video and extracts frames for processing.

3. **Hand Position Localization**:
   After extracting the frames, bounding boxes for hands are detected. The center of each bounding box (calculated as the center of x and y) is used to localize the hand positions for subsequent mask generation.

4. **Mask Generation**:
   SAM2 uses the localized hand positions to generate segmentation masks for hand movements in each frame.

5. **Visualization**:
   Outputs a video or visualizations of the generated masks overlaid on the original frames.

6. **Export Results**:
   The processed video with masks is saved as output_video.mp4 in the project directory.

## Google Colab
Run the project directly in Google Colab by using the following link: [Google Colab Link](https://colab.research.google.com/drive/1fLbNTUbDy3339KozfeQPAEC9JrcY0KTc?usp=sharing)
