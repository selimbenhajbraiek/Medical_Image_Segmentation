## Medical Image Segmentation for Cardiac MRI using U-Net

📌 Introduction

Medical image segmentation is crucial for diagnosing heart conditions such as heart failure and myocardial infarction. Cardiac MRI provides detailed insights into the heart's structure, but manual segmentation is time-consuming and error-prone. This project leverages deep learning, specifically U-Net, to automate the segmentation of cardiac structures, including:

Left Ventricular Endocardium

Epicardium

Right Ventricular Endocardium

🏗️ Methodology

1️⃣ Model Architecture: U-Net

Encoder-Decoder Structure: Reduces spatial dimensions and then restores resolution using upsampling layers.

Skip Connections: Helps retain spatial details, crucial for accurate segmentation.

Input Size: 256x256x1 grayscale MRI slices.

Output: 256x256x1 segmentation masks.

2️⃣ Training Details

Dataset: ACDC Challenge (Annotated Cardiac MRI Dataset)

Loss Function: Dice Loss

Optimizer: Adam Optimizer (learning rate = 0.001)

Batch Size: 2

Epochs: 50 (Early stopping applied)

3️⃣ Evaluation Metrics

Dice Coefficient (Measures segmentation accuracy)

Performance on Test Data:

Left Ventricular Endocardium: Dice Score = 0.89

Epicardium: Dice Score = 0.84

Right Ventricular Endocardium: Dice Score = 0.83

🔍 Results & Visualizations

Overlayed segmentation masks on MRI images to visualize model accuracy.

Comparison with ground truth annotations confirms model effectiveness.

Matches state-of-the-art results (similar to ACDC Challenge scores).

🚀 Future Enhancements

🔹 Hybrid Models: Integrating transformers to improve segmentation.
🔹 Data Augmentation: Increasing dataset variety for better generalization.
🔹 Multiclass Segmentation: Extending to multiple cardiac structures.


📜 References

Ronneberger et al. (2015): U-Net for Biomedical Image Segmentation.

Zhu et al. (2018): U-Net for Myocardial Infarction Segmentation.

ACDC Challenge 2017: Automated Cardiac Diagnosis Challenge

Adam Optimizer: Kingma & Ba (2014) - ICLR.

🤝 Contributing

Feel free to contribute to this project! Clone the repo, suggest improvements, or optimize the model.

🔗 Let's connect! Reach out if you're interested in AI for medical imaging! 🚀

#AI #MedicalImaging #DeepLearning #HealthcareAI
