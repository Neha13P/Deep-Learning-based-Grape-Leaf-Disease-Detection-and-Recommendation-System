Grape Leaf Disease Prediction with GAN-Augmented Dataset

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

Final Look of Gradio Interface
![Screenshot 2024-12-27 053730 1](https://github.com/user-attachments/assets/e2a433c7-13be-4b17-af57-5857a45dc5e2)
![Screenshot 2024-12-27 053644 1](https://github.com/user-attachments/assets/fc9b84a3-ffbf-4b47-9cae-eaf78917347c)
