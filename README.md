📘 Project Overview
This project explores regularization techniques in deep learning to combat overfitting and improve model generalization. Using the CIFAR-10 dataset and a ResNet-18 architecture, the study evaluates a wide range of regularization methods categorized into four main types: input-level, parameter-level, architectural, and label-based. Each method is assessed individually and in hybrid combinations to analyze their impact on training/test accuracy, convergence speed, and generalization gap.

DL-Regularization-Study/
│
├── data/                    # Scripts or links to download CIFAR-10 dataset
├── models/                  # ResNet-18 model with different regularizations
├── experiments/             # Scripts for individual experiments
├── results/                 # Graphs and evaluation metrics
├── utils/                   # Utility functions (preprocessing, plotting, etc.)
├── requirements.txt         # Dependencies
├── README.md                # Project overview
└── report.pdf               # Detailed paper (your uploaded PDF)

🧠 Regularization Techniques Studied
Input-Level: Cutout, Mixup, CutMix

Parameter-Level: L1, L2 (Weight Decay), Dropout, DropBlock

Architectural: Batch Normalization, Stochastic Pooling

Label-Based: Label Smoothing

🛠️ Tools & Frameworks
Framework: PyTorch 2.0, TensorFlow

Hardware: NVIDIA RTX 3060 GPU

Optimizer: SGD with momentum / Adam

Training Setup:

Epochs: 200 (for PyTorch) / 30 (for TensorFlow)

Batch Size: 128

Loss: CrossEntropy with optional Label Smoothing

📊 Key Findings
CutMix and Mixup showed the best generalization with minimal overfitting.

Batch Normalization accelerated convergence and stabilized training.

Hybrid techniques (e.g., Mixup + Dropout + L2) provided additive benefits.

L2 Regularization improved test accuracy consistency with reduced generalization error.

📈 Evaluation Metrics
Training/Test Accuracy & Loss

Generalization Gap

Convergence Speed (Epochs to 90% training accuracy)

Statistical Significance via paired t-tests

🔍 Future Work
Scaling experiments to datasets like ImageNet or medical/NLP domains

Applying regularization in Transformer-based models

AutoML integration for dynamic regularization tuning

Exploring adversarial robustness and feature interpretability

git clone https://github.com/SHAH/DL-Regularization-Study.git
cd DL-Regularization-Study
pip install -r requirements.txt
