# Stress-Analysis
Stress Classification using WorkStress3D dataset

Dataset used: 

->Physiological Signals and Facial Expressions Data (2 classes)

link: https://data.mendeley.com/datasets/t93xcwm75r/8

Stress classes: 0 (stress-free) 1 (stressed)

Models:

Independent-models:

  For Physiological Data: LSTM, SVM

  For Facial Expressions Data: VGG16, Basic CNN

Fusion-approach:
- Both LSTM and VGG16 outputs are combined to provide as inputs to the fusion layer.
- The physiological and facial data are combined to train the fusion layers. Note that: LSTM and VGG16 are independently trained on physiological and facial data respectively at first. Only their predictions/features are used for training fusion layer.
