# Automated Plant Disease Detection

This project focuses on **automated detection of plant diseases** using Machine Learning and Deep Learning. The goal is to provide an accurate and scalable solution for identifying plant diseases, reducing reliance on manual inspection.

---

## Problem Statement
Plant diseases reduce crop yield and threaten food security. Manual diagnosis is slow, subjective, and error-prone. This project applies computational methods to improve speed and accuracy in disease detection.

---

## Dataset
- **New Plant Diseases Dataset (Augmented)**  
- Organized into training and validation sets  
- Images of plant leaves labeled by disease class  
- Preprocessing includes resizing, normalization, and label encoding
- Preprocessed data from what run I prepare for leaning is call preproccesed_data

---

## Methodology
1. **Traditional Machine Learning**
   - Random Forest and Logistic Regression  
   - PCA for dimensionality reduction  

2. **Convolutional Neural Network (CNN)**
   - Three convolutional layers with max pooling  
   - Dense layer with dropout  
   - Softmax output  

3. **Transfer Learning**
   - Pretrained **ResNet50** model  
   - Frozen base layers with custom dense classifier  
   - Dropout for overfitting prevention  

---

## Experiments
- Images were processed according to model requirements  
- Traditional ML: scaling + PCA  
- CNN: trained from scratch with early stopping  
- Transfer Learning: fine-tuned with frozen base and early stopping  

---

## Results

| Model                  | Validation Accuracy |
|------------------------|------------------|
| Random Forest          | 52.6%            |
| Logistic Regression    | 52%              |
| CNN from Scratch       | 73.4%            |
| Transfer Learning (ResNet50) | 93%       |

- Traditional ML models underfit and struggled with complex visual patterns  
- CNN improved accuracy but misclassified some classes  
- Transfer Learning using ResNet50 achieved the best performance  

---

## Conclusion
- Transfer Learning is most effective for plant disease classification  
- CNN from scratch is promising but less accurate  
- Traditional ML is not suitable for complex image tasks  

---

## Repository & Presentation Video
- GitHub repository: [link]  
- Presentation video (5–10 minutes): [link]  

---

## References
- New Plant Diseases Dataset (Augmented)  
- TensorFlow and Keras documentation  
- Scikit-learn documentation

## Future improvement
- increase the validation and overall performance of the models.
- Usable AI for farmers
