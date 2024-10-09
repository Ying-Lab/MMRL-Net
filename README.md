# AI-Assisted Hypertension Detection with ECG

## Overview

This project aims to develop an AI-driven framework for the early detection of hypertension-mediated heart damage using Electrocardiogram (ECG) signals. The framework utilizes a deep learning model to predict hypertension and identify hypertension-associated ECG segments, which can facilitate early diagnosis and potentially reduce the risk of hypertensive cardiovascular-related mortality and morbidity.

## Key Features

- **MML-Net**: A multi-branch, multi-scale LSTM neural network designed to classify hypertension and non-hypertension individuals based on ECG signals.
- **ECG-XAI**: An explainable AI pipeline that identifies specific ECG segments associated with hypertension.
- **High Accuracy**: Achieves an 82% recall and 87% precision in distinguishing hypertensive individuals from non-hypertensive individuals.
- **Clinical Relevance**: Identifies R-wave and P-wave as the key ECG segments indicative of hypertension.

## Getting Started

### Prerequisites

- Python 3.7+
- Pytorch 11.3
- Keras
- NumPy
- Scikit-learn
- Matplotlib (for visualization)
- [NeuroKit2](https://neurokit.xyz/) for ECG signal processing
- [ECGAccess](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC9120362/) for  ECG QC

### Installation

Clone the repository and install the required packages:

```bash
git clone https://github.com/Ying-Lab/MMRL-Net.git
cd ./MMRL-Net
```

### Model Details

The MML-Net model is located in the `./model` folder. It requires input data in the form of a `5000x12`numpy array, where each row corresponds to a time point and each column corresponds to a different lead of the ECG. The model outputs a `1x2` array, with the first element representing the probability of hypertension and the second element representing the probability of not having hypertension.

### Model Input/Output

- Input: `5000x12 `numpy array (ECG data)
- Output: `1x2 `numpy array (probability of hypertension and not hypertension)
  Ensuring Correct Input Dimensions

## Contributing

Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT License](https://opensource.org/licenses/MIT)

## Contact

For any questions or collaboration inquiries, please contact:

- Dr. Lijuan Zhang at zhangli.jennifer@foxmail.com
- Dr. Ying Wang at wangying@xmu.edu.cn
- ChengweiLiang 23220211151666@stu.xmu.edu.cn

## Acknowledgments

This project is inspired by the research article "AI-Assisted Early Detection of Hypertension-Mediated Heart Damage on ECG" by Chengwei Liang et al., published by Xiamen University.
