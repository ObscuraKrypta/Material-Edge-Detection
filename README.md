# Material-Edge-Detection

This project implements a YOLOv11-based model for detecting and classifying the **shape** of small materials (1–4 mm), such as *sharp-edged* or *smooth* particles, moving on a conveyor belt. The system is developed for use in eddy current separator (ECS) machines in industrial recycling environments.

##  Model Overview

- **Model**: YOLOv11n-seg (custom-trained)
- **Framework**: PyTorch
- **Purpose**: Real-time detection of material shapes (sharp vs. smooth)
- **Application**: Improving separation quality and preventing damage in ECS systems

##  Files

- `Material-Edge-Detection-YOLO.v11`: Main Python file containing model architecture and inference logic
- `data.yaml`: YOLO-format dataset configuration file

##  Dataset

The dataset used in this project includes:
- Annotated images of sharp and smooth materials
- Segmentation masks and bounding boxes
- YOLO-compatible format

 **Hosted on Kaggle**  
Due to GitHub's file size limitations, the complete dataset is hosted on Kaggle.  
 [Kaggle Dataset Link](https://www.kaggle.com/USERNAME/DATASET-NAME)  
*(Replace with the actual link once available)*

##  How to Run

 # Clone the repository:
   ```bash
   git clone https://github.com/ObscuraKrypta/Material-Edge-Detection.git
   cd Material-Edge-Detection
    ```



#Install dependencies
```bash
pip install -r requirements.txt
    ```

Download the dataset from Kaggle and extract into datasets/ folder.

# Train the model
```bash
python train.py --data data.yaml --weights yolov11n-seg.pt --epochs 100
    ```

#Run inference
```bash
python detect.py --source path/to/image_or_video --weights best.pt
    ```


##Use Cases
- Industrial recycling optimization

- Smart ECS machine control

- Preventive maintenance via edge shape analysis

## Development Info
Author: Shohreh Kia

Version: v1.0

Development Location: Clausthal-Zellerfeld, Germany

Date: November 2024 – March 2025

License
This project is open-source and free to use for academic and research purposes.





