[URL to the Dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)

4 Articles Using the Same Dataset:

[Peer-Reviewed Article 1](https://pubmed.ncbi.nlm.nih.gov/33861150/)

[Peer-Reviewed Article 2](https://pmc.ncbi.nlm.nih.gov/articles/PMC9140837/)

[Peer-Reviewed Article 3](https://pmc.ncbi.nlm.nih.gov/articles/PMC10252226/)

[Peer-Reviewed Article 4](https://ieeexplore.ieee.org/document/8741582)


1st Version (ResNet-18-v1 Branch): Used Transfer Learning with ResNet-18: 80.37% Test Accuracy

- ResNet18-L2Reg(.0001)-LR(.0001)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0001. 10 epoch. No data augmentation. 81.09% Test Accuracy
- ResNet18-L2Reg(.0001)-LR(.001)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .001. 10 epoch. No data augmentation. 82.37% Test Accuracy
- ResNet18-L2Reg(.0001)-LR(.01)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .01. 10 epoch. No data augmentation. 84.13% Test Accuracy
- ResNet18-L2Reg(.0001)-LR(.0005)-DA-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0005. 25 epoch. Data augmentation (pre-training). 84.46% Test Accuracy
- ResNet18-L2Reg(.001)-LR(.0005)-DA-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0005. 25 epoch. Data augmentation (pre-training). 83.65% Test Accuracy
- ResNet18-L2Reg(.01)-LR(.0005)-DA-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0005. 25 epoch. Data augmentation (pre-training). 82.53% Test Accuracy
- ResNet18-L2Reg(.0001)-LR(.0005)-DA-DO(.3)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0005. 25 epoch. Data augmentation (pre-training). Dropout (p=.3). 85.90% Test Accuracy. .1687 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0005)-DA-DO(.3)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0005. 25 epoch. Data augmentation (pre-training). Dropout (p=.3). 88.94% Test Accuracy. .1363 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0005)-DA-DO(.2)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0005. 25 epoch. Data augmentation (pre-training). Dropout (p=.2). 84.62% Test Accuracy. .2017 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0005)-DA-DO(.2)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0005. 25 epoch. Data augmentation (pre-training). Dropout (p=.2). 87.02% Test Accuracy. .1287 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DA-DO(.2)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.2). 84.78% Test Accuracy. .2259 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DA-DO(.2)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.2). 84.94% Test Accuracy. .2254 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DA-DO(.3)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.3). 86.22% Test Accuracy. .2131 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DA-DO(.4)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.4). 87.82% Test Accuracy. .2017 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DA-DO(.4)-v3 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.4). 87.34% Test Accuracy. .2113 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DA-DO(.5)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization, LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.5). 87.18% Test Accuracy. .2519 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.001)-DA-DO(.4)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization .0001 , LR initialized to .001. 25 epoch. Data augmentation (pre-training). Dropout (p=.4). 89.58% Test Accuracy. .1253 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.001)-DA-DO(.4)-v3 Branch: Transfer Learning with ResNet18, L2 Regularization .0001 , LR initialized to .001. 25 epoch. Data augmentation (pre-training). Dropout (p=.4). 89.42% Test Accuracy. .1291 Validation Loss
- ResNet18-L2Reg(.001)-LR(.0001)-DA-DO(.4)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization .001 , LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.4). 88.14% Test Accuracy. .1986 Validation Loss
- ResNet18-L2Reg(.01)-LR(.0001)-DA-DO(.4)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization .01 , LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.4). 87.02% Test Accuracy. .2114 Validation Loss
- NOTE: 87.98% accuracy with DAv2 saved to /content/drive/My Drive/chest_xray_models/resnet18_L2Reg0001_001LR_DA2_DO04_v2.pth
- ResNet18-L2Reg(.0001)-LR(.0001)-DAv3-DO(.)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization .0001 , LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.0). 88.78% Test Accuracy. .2861 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DAv3-DO(.4)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization .0001 , LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.4). 88.46% Test Accuracy. .4125 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DAv3-DO(.4)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization .0001 , LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.4). 89.26% Test Accuracy. .3269 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DAv3-DO(.5)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization .0001 , LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.5). 89.42% Test Accuracy. .3205 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DAv3-DO(.6)-v1 Branch: Transfer Learning with ResNet18, L2 Regularization .0001 , LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.6). 89.10% Test Accuracy. .4161 Validation Loss
- ResNet18-L2Reg(.0001)-LR(.0001)-DAv3-DO(.6)-v2 Branch: Transfer Learning with ResNet18, L2 Regularization .0001 , LR initialized to .0001. 25 epoch. Data augmentation (pre-training). Dropout (p=.6). 88.94% Test Accuracy. .3375 Validation Loss

