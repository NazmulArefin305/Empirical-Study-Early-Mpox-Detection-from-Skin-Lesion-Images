# Early Detection of Monkeypox Using Pre-trained CNNs with XAI

This project presents an **empirical study on early detection of monkeypox (Mpox)** from skin lesion images using **pre-trained Convolutional Neural Network (CNN) models** and **Explainable AI (XAI)** techniques. Given the challenges of differentiating monkeypox from other similar skin conditions, the study leverages deep learning to improve diagnostic accuracy and interpretability.

## Objectives

* Evaluate the performance of pre-trained CNN models (VGG16, VGG19, InceptionV3, MobileNetV2).
* Compare results across binary (Monkeypox vs Others) and multi-class (6 skin conditions) datasets.
* Apply **Grad-CAM** to enhance transparency and interpretability of model predictions.

## Methodology

* **Datasets**:

  * Monkeypox Skin Lesion Dataset (binary, 3,192 images after augmentation).
  * Mpox Skin Lesion Dataset v2.0 (multi-class, 7,532 images after augmentation).
* **Approach**: Transfer learning with frozen base layers and custom classification layers.
* **Training**: Conducted in Google Colab (GPU-enabled) with TensorFlow/Keras, using Adam optimizer, early stopping, and data augmentation to improve generalization.
* **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score, ROC/AUC, execution time.

## Results

* **Binary Classification**: InceptionV3 achieved the highest accuracy (95%), outperforming other models.
* **Multi-class Classification**: MobileNetV2 performed best with 93% accuracy and the lowest computational cost.
* **Explainability**: Grad-CAM highlighted critical lesion regions influencing predictions, improving model trustworthiness.

## Key Insights

* Transfer learning significantly reduced model complexity and training time.
* MobileNetV2 proved most efficient for real-world applications due to its lightweight design.
* Despite high accuracy, some models showed overfitting risks, mitigated by augmentation and early stopping.
* XAI visualization bridges the gap between AI predictions and clinical interpretability.

## Conclusion

This study demonstrates the **potential of pre-trained CNNs combined with XAI** for early and accurate monkeypox detection. Future work will explore larger and multimodal datasets, advanced interpretability methods, and clinical validation for deployment.

Do you want me to also prepare a **shorter, one-paragraph abstract version** for the very top of your README (before this detailed summary), similar to how GitHub projects often start?
