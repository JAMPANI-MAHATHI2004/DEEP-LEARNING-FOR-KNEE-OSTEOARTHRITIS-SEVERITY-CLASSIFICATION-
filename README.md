# DEEP-LEARNING-FOR-KNEE-OSTEOARTHRITIS-SEVERITY-CLASSIFICATION-
Knee osteoarthritis (OA) is a degenerative joint disease causing pain, stiffness, and reduced mobility due to cartilage breakdown.

## SUMMARY OF THE PROJECT : 
This project presents a deep learning-based solution for the automated classification of knee osteoarthritis (KOA) severity using X-ray images. Leveraging the power of EfficientNet-B3, a state-of-the-art convolutional neural network pre-trained on ImageNet, the model was fine-tuned to classify knee OA severity based on the Kellgren-Lawrence (KL) grading system (Grades 0–4). To ensure robustness, a wellstructured pipeline was developed including data augmentation, class balancing, and custom dataset handling. The model was trained and evaluated on thousands of knee radiographs from real-world datasets, achieving an overall accuracy of 89%, with particularly strong performance in detecting higher-grade OA cases. To enhance model explainability, the project integrated Grad-CAM visualizations, allowing clinicians and users to interpret which regions of the X-ray influenced the model's decision. This makes the system more transparent and clinically trustworthy. Additionally, the model demonstrated its ability to generalize by successfully predicting KOA severity on an external X-ray image not seen during training.

## DATASET:
This dataset contains knee X-ray data for both knee joint detection and knee KL grading. The dataset is organized from OAI 
Published: 4 September 2018
Contributor: Pingjun Chen
The knee X-ray images used to train the model are sourced from the Knee Osteoarthritis Severity Grading Dataset available on Kaggle. The dataset, contains a total of 9,786 knee images categorized into five severity levels according to the Kellgren-Lawrence (KL) grading system:
- Grade 0 (Healthy): about 40% of images – 3857 images
- Grade 1 (Doubtful): around 18% of images – 1770 images
- Grade 2 (Minimal): approximately 26% of images – 2578 images
- Grade 3 (Moderate): roughly 13% of images – 1286 images
- Grade 4 (Severe): slightly over 3% of images – 295 images
Each image in the dataset is standardized to a resolution of  224 × 224 pixels for model training. This balanced yet skewed class distribution represents a realistic challenge in detecting severe osteoarthritis due to the smaller sample size of higher-grade images.

| KL Grade | Description | Image Count | Percentage |
| -------- | ----------- | ----------- | ---------- |
| 0        | Healthy     | 3,857       | \~40%      |
| 1        | Doubtful    | 1,770       | \~18%      |
| 2        | Minimal     | 2,578       | \~26%      |
| 3        | Moderate    | 1,286       | \~13%      |
| 4        | Severe      | 295         | \~3%       |
