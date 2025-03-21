# Fabric Defect Detection using YOLOv5

## Project Overview

The **Fabric Defect Detection using YOLOv5** project focuses on detecting defects in textile fabric, specifically identifying **cuts**, **holes**, **thread errors**, and **stains**. This project is a part of the **Final Year Project** and uses the **YOLOv5** model to classify and detect these fabric defects in images.

The model was trained on a custom dataset of fabric images, and it provides real-time feedback on whether the fabric is defective or not. **Defective areas** are marked in **red**, while areas without defects are highlighted in **green**.

## Goal

- **Train a model** using **YOLOv5** to detect **fabric defects** (cuts, holes, thread errors, stains).
- Visualize the detected defects in **real-time**, with color-coded outputs.
- Provide a **real-time feedback system** that flags defective areas (red) and non-defective areas (green).

## Dataset

The dataset used for training consists of images of textile fabrics, with labeled defects such as:

- **Cut**: Visible cuts or rips in the fabric.
- **Hole**: Unintentional holes or tears.
- **Thread Error**: Irregularities or faults in the fabric threads.
- **Stain**: Visible marks or stains on the fabric.

The dataset was manually annotated to train the YOLOv5 model to recognize these defects.

## Files in the Repository

- **data/**: Folder containing the **training** and **test** datasets for fabric defect detection.
- **LICENSE**: License file for the project.
- **README.md**: Documentation for the Fabric Defect Detection using YOLOv5 project.
- **Untitled.ipynb**: Jupyter notebook for model training and evaluation.
- **data.yaml**: Configuration file for dataset paths and class labels.
- **requirements.txt**: List of Python dependencies required to run the project.

## Steps

### 1. Dataset Preparation
- Collected images of textile fabrics and labeled them for defects such as **cut**, **hole**, **thread error**, and **stain**.
- The images were organized into separate directories for training and testing, along with the annotation files.

### 2. Training YOLOv5
- Used the **YOLOv5** model for training the fabric defect detection task.
- Fine-tuned the YOLOv5 model on the custom dataset for **2-3 epochs** to detect the fabric defects.
- Configured the model to identify four types of defects: **cut**, **hole**, **thread error**, and **stain**.

### 3. Testing and Evaluation
- Evaluated the model on a test set to check its performance in detecting fabric defects.
- The model visualizes the detected defects in **red** and non-defective areas in **green**, providing a clear indication of the fabric's quality.

## Deliverables

- A **trained YOLOv5 model** that can detect fabric defects.
- **Color-coded output** where defective areas are marked in red and non-defective areas in green.
- **Evaluation metrics** such as **precision**, **recall**, and **mAP** to assess model performance.

### Example:

- **Detected Defect**: **Red** highlight for defects such as cut, hole, or stain.
- **Non-Defective Fabric**: **Green** highlight indicating no defects.

## Technologies Used

- **Model**: [YOLOv5](https://github.com/ultralytics/yolov5)  
- **Libraries**: **PyTorch**, **OpenCV**, **NumPy**, **Matplotlib**
- **Dataset**: Custom dataset of fabric images with defect annotations
- **Other Tools**: **Wandb** (for tracking experiments), **Git LFS** (for handling large image files)

## How to Run

1. Clone the repository:  
   `git clone https://github.com/shaiiikh/Fabric-Defect-Detection-using-YOLOv5.git`

2. Install dependencies:  
   `pip install -r requirements.txt`

3. Train the model:
   - Run the **training cell** in **Untitled.ipynb** to start training the YOLOv5 model on the custom dataset.

4. Test the model:
   - Use the trained model to **predict defects** in new fabric images. The detected defects will be visualized with red highlights, while non-defective areas will appear green.

## Conclusion

The **Fabric Defect Detection using YOLOv5** project demonstrates how deep learning can be applied to real-world industrial problems such as fabric quality control. By fine-tuning the **YOLOv5** model on a custom dataset, we were able to effectively identify common fabric defects and visualize them in real-time, improving the process of quality assurance in textile production.
