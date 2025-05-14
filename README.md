 🦾 Object Detection using Faster R-CNN + Pascal VOC 🖼️

Welcome to this 🔍 Object Detection project using PyTorch and the Pascal VOC dataset. The model is trained using the `torchvision` implementation of **Faster R-CNN**. The objective is to detect and localize objects in images from the VOC dataset.

---

## 📁 Project Structure

├── VOCdevkit/ # Pascal VOC dataset
├── train.py # Main training script
├── transforms.py # Data transforms
├── model.py # Model loading and utilities
└── README.md # This file

---

## 🚀 Features

- ✅ Trainable on GPU/CPU
- ✅ Supports Pascal VOC dataset
- ✅ Uses PyTorch + torchvision Faster R-CNN
- ✅ Lightweight training loop for customization
- ✅ Built-in data augmentation

---

## 🧠 Model

The model used is:

- 📦 `torchvision.models.detection.fasterrcnn_resnet50_fpn`
- Backbone: ResNet-50 with Feature Pyramid Network (FPN)
- Pretrained on COCO, finetuned on Pascal VOC

---

## 🏁 Getting Started

### 1. 📦 Install Dependencies

```bash
pip install torch torchvision
2. 📥 Download Pascal VOC Dataset
You can download the dataset from the official PASCAL VOC 2012 site. Extract it under the VOCdevkit/ folder.

3. 🧪 Run Training

python train.py
🔧 Training Loop

for epoch in range(num_epochs):
    for images, targets in dataloader:
        ...
        loss_dict = model(images, targets)
        losses = sum(loss for loss in loss_dict.values())
        ...
📈 Logs example:

Epoch 1, Loss: 2.5432
Epoch 2, Loss: 1.8421
...
📊 Results & Evaluation
Evaluation script is not included here, but you can use:

torchvision evaluation utilities

pycocotools or mAP metrics with a validation split

🙌 Acknowledgements
PyTorch 🔥

Torchvision 🧰

Pascal VOC 🖼️

