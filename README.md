Pedestrian Detection & Segmentation using Mask R-CNN

This project fine-tunes a Mask R-CNN model to detect and segment pedestrians in images. Given an input image, it generates instance masks and bounding boxes around pedestrians with visual overlays.

📌 Problem Statement

Detecting pedestrians in images is critical for applications like autonomous driving, surveillance, and smart cities. Traditional object detectors identify pedestrians but don’t provide precise shape information. This project addresses that by leveraging Mask R-CNN for accurate instance segmentation of pedestrians.

📘 [View Notebook on Google Colab](https://colab.research.google.com/drive/1AZ6JB6SxymOzsrn8YXvbGOV27lbYAgrT?usp=sharing)

References

PennFudanPed dataset: https://www.cis.upenn.edu/~jshi/ped_html/

🔍 Use Case

Input an image containing pedestrians

The model outputs segmented masks and bounding boxes

Helps in pedestrian tracking, safety monitoring, and scene understanding

🧠 Approach

Dataset: PennFudanPed pedestrian dataset

Model: Fine-tuned Mask R-CNN with a ResNet-50 backbone and Feature Pyramid Network (FPN)

Training: Custom PyTorch Dataset, data augmentation during training, SGD optimizer with learning rate scheduling

Inference: Generates masks, bounding boxes, and class labels; visualizes results with color-coded masks overlaid on images

How to Run

Clone the repo:

git clone https://github.com/yourusername/maskrcnn-pedestrian-segmentation.git
cd maskrcnn-pedestrian-segmentation
