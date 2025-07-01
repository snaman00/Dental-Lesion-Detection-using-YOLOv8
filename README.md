# Dental-Lesion-Detection-using-YOLOv8

This project focuses on leveraging **Computer Vision** to automate the detection of **dental caries (cavities)** and **periapical (PA) lesions** in dental radiographs. Early and accurate diagnosis of such conditions is critical for timely treatment planning, reducing complications, and improving patient outcomes. By using **YOLOv8 Large (`yolov8l`)**, we have trained an object detection model capable of localizing and classifying these dental anomalies with strong performance metrics.

## Dataset

- **Total Images:**  
  - **Training:** 7,043  
  - **Validation:** 370  
- **Classes:**  
  - **Cavity:** Dental caries  
  - **PA:** Periapical lesions

Radiographs were annotated to highlight regions of interest (ROIs) where these conditions appear, enabling the model to learn both localization and classification.

## Model & Training

- **Model Used:** YOLOv8 Large (`yolov8l`)
- **Epochs Trained:** 90  
- **Framework:** Ultralytics YOLOv8  
- **Task:** Object Detection (Bounding box regression + Class prediction)

## Results

| Metric           | Overall | Cavity | PA |
|------------------|---------|--------|-----|
| **mAP50**        | 74.30%  | 68.20% | 80.40% |
| **Precision**    | 79%     | 73.70% | 83.60% |

The model achieves an overall **mAP50 of 74.30%** and an average precision of **79%** across both classes, indicating reliable detection capability in real-world scenarios.

## Use Cases

- **Clinical Assistance:** Assist dentists by highlighting potential cavities and PA lesions automatically, saving time and reducing oversight.
- **Screening Tool:** Pre-screen large volumes of dental X-rays in clinics, hospitals, or remote dental camps.
- **Second Opinion:** Provide an AI-powered second opinion to verify manual diagnosis, improving diagnostic confidence.
- **Training & Education:** Aid dental students in understanding radiographic patterns of dental pathologies.
- **Tele-Dentistry:** Enable remote diagnosis by integrating this model with cloud-based dental imaging platforms.

## Future Scope

- **Expand Dataset:** Collect more annotated images from diverse demographics and X-ray machines to improve generalization.
- **Multi-class Detection:** Include more dental conditions such as root canal issues, impacted teeth, bone loss, or cysts.
- **3D Integration:** Extend detection capabilities to 3D Cone Beam CT (CBCT) scans for advanced diagnostics.
- **Clinical Deployment:** Develop a user-friendly web or mobile application for dentists to upload X-rays and get instant AI analysis.
- **Regulatory Approval:** Work towards certification and compliance for use in real-world clinical environments.
- **Continuous Learning:** Implement active learning pipelines to retrain the model with new data, improving accuracy over time.

## How to Use

1. **Train**  
   - Use the provided training scripts to fine-tune YOLOv8 on your dataset.
2. **Detect**  
   - Run inference on new X-ray images to get bounding boxes and class predictions.
3. **Evaluate**  
   - Compare results with benchmark metrics provided above.

## Conclusion

This project demonstrates the feasibility of using modern object detection models like YOLOv8 to assist dental professionals with early and accurate diagnosis of cavities and PA lesions. By combining AI with dentistry, we aim to make dental care more efficient, accessible, and reliable for all.

**Made with 🦷 + 🤖 + ❤️**
