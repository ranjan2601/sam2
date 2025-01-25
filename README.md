
# Hand Movement Masking Using SAM2, Torch, and Torchvision

## Features
- **Mask Generation**: Leverages SAM2 (Segment Anything Model) for generating segmentation masks.
- **Frame-by-Frame Processing**: Extracts frames from a video and processes them individually.
- **Integration with Torch and Torchvision**: Efficient handling of video data and deep learning operations.
- **Google Colab Support**: Ready-to-run on Colab for ease of use and reproducibility.

## Requirements
Ensure the following dependencies are installed:

- Python 3.8+
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

2. Upload your video file  to the project directory.

3. Run the `hand_movement.ipynb` file on Google Colab or your local Jupyter Notebook environment.

### Steps in the Notebook

1. **Setup Environment**:
   The first cell contains the code to install SAM2 and its dependencies. Ensure to enable GPU acceleration in Google Colab for faster processing (`Runtime > Change runtime type > Hardware accelerator > GPU`).

2. **Video Loading**:
   The script reads the input video and extracts frames for processing.

3. **Mask Generation**:
   SAM2 generates segmentation masks for hand movements in each frame.

4. **Visualization**:
   Outputs a video or visualizations of the generated masks overlaid on the original frames.

5. **Export Results**:
   The processed video with masks is saved as `output_video.mp4` in the project directory.


## Google Colab
Run the project directly in Google Colab by using the following link:

[Open in Google Colab]([(https://colab.research.google.com/drive/1fLbNTUbDy3339KozfeQPAEC9JrcY0KTc?usp=sharing)])


