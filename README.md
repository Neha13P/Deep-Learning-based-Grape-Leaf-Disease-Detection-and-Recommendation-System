Grape Leaf Disease Prediction with GAN-Augmented Dataset

![Esca_measles(interface)](https://github.com/user-attachments/assets/1484d9a6-b56d-42fb-9fcd-018747d3853b)

This project focuses on grape leaf disease detection using a deep learning(GAN + ResNet) model. The dataset used includes both the original dataset from Kaggle and GAN-generated images to improve model performance through augmentation.

Dataset Sources

1. Original Dataset
   
Name: Grape Plant from Plant Village Dataset

Link: https://www.kaggle.com/datasets/zienabesam/grape-plant-from-plant-village-dataset

Description: This dataset consists of images of grape leaves categorized into four disease classes:

Grape___Black_rot

Grape___Esca_(Black_Measles)

Grape___healthy

Grape___Leaf_blight_(Isariopsis_Leaf_Spot)


2. GAN-Generated Images
   
Source: https://www.kaggle.com/code/vasudevkrishna385964/dcgan-final

Project Workflow:

1. Model Training (Grape_Disease_Prediction.ipynb)
   
The model is trained on the original dataset and GAN-augmented images.

After training, the model is saved as fused_model.h5.

2. Model Deployment (Model_testing.ipynb)
   
The trained model (fused_model.h5) is imported for testing.

A Gradio-based UI is built for user interaction.

3. Disease Analysis with LangChain + Groq’s LLaMA
   
Upon detecting a disease, Groq’s LLaMA model via LangChain generates a detailed analysis report with:

Brief description

Treatment measures

Preventive measures

Monitoring guidelines


How to Run

1️⃣ Train the model in Grape_Disease_Prediction.ipynb

2️⃣ Save the model as fused_model.h5

3️⃣ Open Model_testing.ipynb, load the model, and run the Gradio UI

🚀 Now, you can upload grape leaf images and receive disease predictions along with AI-generated reports!

Interface Output:
![InterfaceOutput](https://github.com/user-attachments/assets/21dfad47-c035-42e4-9b61-b4ce8cb7aafc)

Final Look of the Disease Detection and Recommendation System:
![Gradio-diseaseAnalysisReport](https://github.com/user-attachments/assets/7107e911-4c1e-4552-9392-6b5ec92ef84b)
![GradioInterface](https://github.com/user-attachments/assets/c62a1a07-7046-41f2-99d8-efde255ca9e8)

