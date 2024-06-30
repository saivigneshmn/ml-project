# ResNet50-DCT for Automated Image Captioning in Telugu


## Brief Description
This project introduces an innovative automated image captioning system that leverages a unique combination of ResNet50 and Discrete Cosine Transform (DCT) features to generate accurate and descriptive captions in Telugu. The system employs a dual-feature extraction approach, incorporating both ResNet50 for high-level semantic information and DCT for low-level visual details, to create comprehensive feature vectors for input images.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Dataset](#dataset)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Installation
- Clone the repository
git clone https://github.com/saivigneshmn/ml-project.git

- Navigate to the project directory 
cd resnet50-dct-telugu-captioning

- Install required packages
pip install -r requirements.txt

## Usage
- To train the model:
python src/train.py --data_path /path/to/dataset --epochs 50

- To generate captions for new images:
python src/generate_caption.py --image_path /path/to/image.jpg

## Model Architecture
The model architecture consists of three main components:
1. ResNet50 for high-level feature extraction
2. DCT for low-level feature extraction
3. LSTM-based caption decoder

The features from ResNet50 and DCT are concatenated to form a comprehensive feature vector, which is then fed into the LSTM decoder to generate captions in Telugu.

## Dataset
The model was trained on a dataset of diverse images annotated with English captions. For Telugu captioning, an English-to-Telugu translation module was incorporated.

## Results
The model achieved the following performance metrics:
- BLEU-1 Score: 0.435
- BLEU-2 Score: 0.50

Comparative analysis showed that our ResNet50-LSTM model outperformed other architectures such as Xception-LSTM and VGG16-LSTM across different epochs.

## Contributing
We welcome contributions to improve the model or extend its capabilities. Please see the [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines on how to contribute.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- We thank the Vellore Institute of Technology for supporting this research.
- Special thanks to all the researchers and contributors in the field of image captioning and deep learning whose work has inspired and informed this project.
