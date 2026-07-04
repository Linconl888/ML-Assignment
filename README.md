# ML-Assignment

This is an assignment for the Machine Learning course (Course Code: 2706106).

## Project Description

This project reproduces the paper **"Dual Contrastive Learning: Text Classification via Label-Aware Data Augmentation"** (DualCL) and evaluates its robustness on our own dataset:

- **Base Model**: Dual Contrastive Learning (DualCL) for text classification with label-aware data augmentation.
- **Training**: The model is trained on our own dataset using the DualCL framework.
- **Robustness Evaluation**: 
  - Fraud-R1 strategy applied to generate augmented test samples.
  - TextFooler used to craft adversarial examples for the test set.

## Acknowledgements

This project is based on the following open-source repositories:

- **DualCL**: [hiyouga/Dual-Contrastive-Learning](https://github.com/hiyouga/Dual-Contrastive-Learning)
  - The model architecture and training framework are adapted from this repository.
- **Fraud-R1**: [kaustpradalab/Fraud-R1](https://github.com/kaustpradalab/Fraud-R1/tree/main)
  - Used for generating augmented test samples to evaluate model robustness.
- **TextFooler**: [jind11/TextFooler](https://github.com/jind11/TextFooler)
  - Used for generating adversarial test examples to evaluate model robustness.

Thanks to the authors for making their code publicly available.

## Preparation
### Clone
```
git clone https://github.com/Linconl888/ML-Assignment.git
```

### Create an anaconda environment
```
conda create -n ML python=3.7
conda activate ML
pip install -r requirements.txt
```

### Usage
```
python main.py --method dualcl --dataset fraud --model_name bert_chinese
```

## License

This project is released under the MIT License. Parts of the code are adapted from DualCL (MIT License) .
