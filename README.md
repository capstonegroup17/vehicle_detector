**Improved YOLOv5 for Vehicle Detection**

**Introduction**

Welcome to the Improved YOLOv5 for Vehicle Detection GitHub repository. This project is a collaborative effort by Group 17 at Fairleigh Dickinson University, Vancouver Campus, aimed at advancing vehicle detection capabilities within complex traffic management systems. Leveraging the robust YOLOv5 architecture, we introduce significant enhancements to tackle the challenges of detecting vehicles from various angles and under different environmental conditions. Our model focuses on lightweight network design, advanced attention mechanisms, and novel convolution techniques to optimize performance and accuracy.

**Project Description**

This version of YOLOv5 has been re-engineered with the goal of improving performance across varied traffic scenarios. It integrates several cutting-edge technologies and strategies, including:

- **EfficientNet and MobileNet**: These networks reduce the overall computational demand while maintaining high accuracy, making the model suitable for deployment on devices with limited computing resources.
- **PP-LCNet**: Enhances the model's efficiency and speed, crucial for real-time applications.
- **Squeeze-and-Excitation (SE) Attention**: Enhances the model's focus on relevant features by recalibrating channel-wise feature responses.
- **Coordinated Attention (CA)**: Improves the model's spatial awareness by decoupling two-dimensional spatial information, thus enhancing detection accuracy particularly in densely populated traffic scenes.
- **Asymmetric Convolution**: This approach uses convolution kernels of varying sizes to capture detailed features across different orientations, crucial for accurate vehicle detection at odd angles.

**Installation**

Clone the repository and install the required dependencies:

git clone <https://github.com/yourgithub/improved-yolov5-vehicle-detection.git>

```python
cd vehicle-detector

pip install -r requirements.txt
```

**Usage**

Run the vehicle detection model using the following command:

```python
python detect.py --weights path/to/weights --source yourvideofile.mp4 --conf-threshold 0.5 --iou-threshold 0.5
```

Arguments:

- \--weights: Path to the trained model weights.
- \--source: Path to the video file or image directory for detection.
- \--conf-threshold: Confidence threshold for detection.
- \--iou-threshold: IoU threshold for non-max suppression.

**Dataset**

Our training and evaluation are performed on the UA-DETRAC dataset, a challenging real-world dataset for vehicle detection, which consists of various traffic scenarios captured under different lighting and weather conditions.

**Results**

The proposed improvements lead to a mean Average Precision (mAP) increase to 58.1% at IoU=0.5. The model demonstrates high performance in terms of speed and accuracy, making it highly effective for real-time vehicle detection tasks.

**Hardware Requirements**

For optimal performance, we recommend the following hardware configuration:

- **GPU**: NVIDIA GeForce RTX 4060 or better for accelerated model training and inference.
- **CPU**: Intel Core i9 or equivalent.
- **RAM**: Minimum 16 GB, recommended 32 GB for handling large datasets.

**Contributors**

- Jie Zhou (<j.zhou1@student.fdu.edu>)
- Xiaohan Dong (<x.dong@student.fdu.edu>)
- Ruizhe Shang (<r.shang@student.fdu.edu>)
- Yingying Tian (<y.tian@student.fdu.edu>)
- Ran Wang (<r.wang@student.fdu.edu>)

**License**

This project is licensed under the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.  - see the [LICENSE](LICENSE) file for details.