📌 Description
This project uses transfer learning via the fastai library to train a binary image classifier on a labeled flower dataset. The model learns to identify whether a given flower image is a daisy or a dandelion, and outputs a prediction along with a confidence score.
It's a beginner-friendly computer vision project that demonstrates the full ML pipeline — from data loading and augmentation to model training and inference.

🚀 Features

Binary flower classification (Daisy 🌼 vs Dandelion 🌻)
Built using fastai v2 (PyTorch backend)
Transfer learning with a pretrained CNN
80/20 train-validation split with reproducible seed
Per-image prediction with confidence scores
Clean folder-based dataset structure


🗂️ Dataset Structure
Flowers_Classification/
├── train/
│   ├── daisy/
│   └── dandelion/
└── test/
    ├── daisy/
    └── dandelion/

Train size: 1020 images
Validation size: 255 images
Classes: daisy, dandelion


🛠️ Tech Stack
ToolPurposePython 3.11Core languagefastaiDeep learning frameworkPyTorchBackendNumPyNumerical operationsJupyter NotebookDevelopment environment

⚙️ Setup & Usage
1. Clone the repo
bashgit clone (https://github.com/KanakSharma0308/Flower-Classifier-Daisy-vs-Dandelion)
2. Install dependencies
bashpip install fastai numpy
3. Prepare your dataset
Update the dataset path in the notebook to point to your local folder:
pythonpath = Path(r'your/path/to/Flowers_Classification/train')
4. Run the notebook
Open flower_classifier.ipynb in Jupyter and run all cells.

🔍 Sample Output
Actual    : daisy
Predicted : daisy
Confidence: 98.72%
----------------------------------------
Actual    : dandelion
Predicted : dandelion
Confidence: 100.00%
----------------------------------------

📈 Results
The model achieves strong performance on the validation set, with most predictions showing >95% confidence. Further improvements can be made by:

Adding more flower classes
Using data augmentation
Fine-tuning more layers
Adding a confusion matrix for detailed evaluation


