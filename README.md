# ISL META Learning

This repository provides a comprehensive collection of meta-learning algorithms applied to Indian Sign Language (ISL) recognition tasks. The goal is to enable few-shot learning—where models can quickly adapt to new classes with very few labeled examples—using state-of-the-art meta-learning techniques. The project is designed for researchers, students, and practitioners interested in meta-learning, computer vision, and sign language recognition.

## Project Overview

Meta-learning, or "learning to learn," is a paradigm in machine learning where models are trained to rapidly adapt to new tasks with minimal data. This repository implements and compares several influential meta-learning algorithms using a real-world ISL dataset. Each notebook demonstrates a different approach, providing both code and explanations to facilitate understanding and experimentation.

## Dataset

The models in this repository are trained and evaluated on the [Indian Sign Language - Real-life Words dataset](https://data.mendeley.com/datasets/s6kgb6r3ss/2) ([DOI: 10.17632/s6kgb6r3ss.2](https://doi.org/10.17632/s6kgb6r3ss.2)).

- **Description:** The dataset contains 18,000 RGB images of hand gestures representing 20 commonly used ISL words, captured from 8 individuals (6 males, 2 females, ages 9–30). Each image is labeled in the format `ISLword_X_YYYY_Z`, where `ISLword` is the word, `X` is the image number, `YYYY` is the participant ID, and `Z` is the sample number. All gestures are static, and the dataset is suitable for computer vision and machine learning research.
- **License:** CC BY 4.0
- **Source:** [Mendeley Data](https://data.mendeley.com/datasets/s6kgb6r3ss/2)

## Notebooks

- **Dataset Labeller.ipynb:** Utility notebook for labeling and preprocessing the ISL dataset, preparing it for meta-learning experiments.
- **MAML_Model.ipynb:** Implementation of Model-Agnostic Meta-Learning (MAML), which enables models to quickly adapt to new sign language gestures with minimal data.
- **Matching Networks.ipynb:** Implementation of Matching Networks, leveraging attention and memory for one-shot classification of ISL gestures.
- **Prototypical_Network.ipynb:** Implementation of Prototypical Networks, which learn a metric space for classifying ISL gestures by computing distances to class prototypes.
- **Relation_Network.ipynb:** Implementation of Relation Networks, which learn to compare gesture samples and perform few-shot classification using a deep distance metric.
- **Reptile_Model.ipynb:** Implementation of Reptile, a simple and efficient first-order meta-learning algorithm for rapid adaptation to new ISL gesture classes.

## Getting Started

1. **Clone this repository:**
   ```bash
   https://github.com/tej2612/Meta-Learning-Indian-Sign-Language-Recognition.git
   ```
2. **Download the ISL dataset:**
   - Visit [this link](https://data.mendeley.com/datasets/s6kgb6r3ss/2) and follow the instructions to download the dataset.
   - Place the dataset in an accessible directory and update the notebook paths as needed.
3. **Open the desired notebook in Jupyter:**
   ```bash
   jupyter notebook
   ```
4. **Install required dependencies:**
   - See the first cells of each notebook for required Python packages and installation instructions.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Citation

If you use the ISL dataset, please cite:
> Tyagi, A., & Bansal, S. (2022). Indian sign Language-Real-life Words [Data set]. Mendeley Data. https://doi.org/10.17632/s6kgb6r3ss.2

## Acknowledgements

- The dataset is provided by Akansha Tyagi and Sandhya Bansal, available under CC BY 4.0.
- The implementations are inspired by original research papers and open-source projects in the meta-learning and sign language recognition communities. 
