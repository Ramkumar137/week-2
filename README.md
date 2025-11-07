# Water Pollution Detection – Week 2: Model Fine-Tuning & Evaluation

## Project Overview
This week focused on improving and evaluating the CNN model for classifying **clean** vs **polluted** water images.  
Using **Transfer Learning (MobileNetV2)**, the model was fine-tuned on the dataset to boost accuracy and generalization.

---

## Steps Performed
1. **Loaded saved model** from Week 1 (`water_pollution_detector.h5`)
2. **Unfroze top 20 layers** of MobileNetV2 for fine-tuning
3. **Used a lower learning rate (1e-5)** for stable training
4. **Applied data augmentation** (rotation, shift, zoom, flip)
5. **Evaluated model** using accuracy/loss graphs, confusion matrix & classification report
6. **Saved improved model** as `water_pollution_detector_v2.h5`

---

## Model Performance
| Metric | Result |
|--------|--------|
| **Validation Accuracy** | 92.86 % |
| **Precision (Clean)** | 1.00 |
| **Precision (Polluted)** | 0.83 |
| **Recall (Clean)** | 0.89 |
| **Recall (Polluted)** | 1.00 |
| **F1-Score (Overall)** | 0.93 |

The fine-tuned model performed strongly, achieving higher precision and recall than Week 1.

---

## Sustainability Relevance
This project contributes to **SDG 6 – Clean Water and Sanitation**, by enabling early detection of water pollution through image-based AI models.  
Such systems can support environmental monitoring and help ensure safe water for all.

---

## Repository Contents

    Week2_Water_Pollution_Detection/
      ├── water_pollution_finetune.ipynb
      ├── water_pollution_detector_v2.h5
      ├── README.md
      └── evaluation_report.txt
---

## Key Learnings
- Importance of **fine-tuning pretrained networks**
- Role of **data augmentation** in small datasets
- Using **confusion matrix & classification metrics** for deeper model evaluation
