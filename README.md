# Harnessing-deep-learning-techniques-for-early-prognosis-of-oral-cancer-detection
This study proposes an ensemble model combining EfficientNetB3 and ResNet50 for early detection of Oral Squamous Cell Carcinoma (OSCC). Utilizing transfer learning, selective layer freezing, and dropout techniques, the model achieves high accuracy and generalization, outperforming individual models. 

Introduction
Oral cancer is a major health concern globally, with a significant proportion of cases diagnosed at advanced stages. Early detection can dramatically improve survival rates. This project proposes an ensemble model that combines the strengths of EfficientNetB3 and ResNet50 for detecting Oral Squamous Cell Carcinoma (OSCC) from oral images.

Model Architecture
The proposed model utilizes an ensemble of two deep learning architectures:

EfficientNetB3: A lightweight and highly efficient model for classification tasks.
ResNet50: A deep residual network that mitigates the vanishing gradient problem, improving accuracy for deeper models.
By combining these models, the ensemble approach provides better generalization and robustness, outperforming individual models.

Dataset
The dataset consists of 5,192 images of oral lesions labeled as "Normal" and "OSCC." It is divided into three sets:

Training: 3,634 images
Validation: 779 images
Testing: 779 images
The dataset is publicly available on Kaggle.

Training and Evaluation
The models were trained using transfer learning, where pre-trained weights were used to initialize the models, followed by fine-tuning with the oral cancer dataset. Selective layer freezing was applied to retain the learned features from pre-trained models. Dropout layers were introduced to minimize overfitting. Performance metrics such as accuracy, precision, recall, and loss were used to evaluate the models.

Results
Model	         Epochs	   Training Accuracy	   Validation Accuracy	  
CNN	             30	          94.30%	               76.58%	
ResNet50       	 30	          98.11%	                 89.35%	
Ensemble Model	 30	          99.89%	               97.98%	
The ensemble model outperforms individual models, demonstrating superior performance on both training and validation sets.

Conclusion

The ensemble model combining EfficientNetB3 and ResNet50 achieves high classification accuracy, making it a reliable tool for early oral cancer detection. The model significantly reduces overfitting and improves generalization, offering a promising solution for assisting healthcare professionals.


Future improvements include:

Enhancing the dataset and incorporating multimodal data for better model performance.
Exploring explainable AI for model interpretability.
Implementing real-time clinical applications and federated learning for privacy-preserving solutions.
Installation and Usage
To run this project, follow these steps:

Clone the repository:

git clone https://github.com/your-username/oral-cancer-detection.git
cd oral-cancer-detection
