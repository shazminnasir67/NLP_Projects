# Text Classification with Deep Learning Models (RNN, LSTM, CNN)

This project focuses on text classification using deep learning models such as RNN, LSTM, and CNN. The goal is to classify text data (e.g., movie reviews) into different sentiment categories. The project includes data preprocessing, model training, and evaluation using PyTorch.

## Project Name Suggestions
- **Deep Text Classifiers**
- **Text Classification with RNN, LSTM, and CNN**
- **Sentiment Analysis with Deep Learning**
- **Deep Learning for Text Classification**

## Project Structure
The project is organized into the following files:

- **dataloader_byhand.py**: Implements a custom data loader for text classification tasks. It handles tokenization, vocabulary creation, and data batching.
- **dataloader_bytorchtext.py**: Uses the torchtext library to load and preprocess text data, including tokenization and vocabulary creation.
- **models.py**: Contains the implementation of the deep learning models (TextRNN, TextLSTM, and TextCNN) for text classification.
- **main.py**: The main script that ties everything together, including data loading, model training, and evaluation.

## Dataset
The dataset used in this project is the Kaggle Movie Review dataset, which contains phrases from movie reviews along with their sentiment labels. The dataset is stored in a TSV (Tab-Separated Values) format.

## Features
- **Custom Data Loader**: Handles tokenization, vocabulary creation, and data batching without relying on external libraries.
- **Torchtext Data Loader**: Uses the torchtext library for efficient data loading and preprocessing.
- **Deep Learning Models:**
  - **RNN**: A simple Recurrent Neural Network for text classification.
  - **LSTM**: A Long Short-Term Memory network, which is better at capturing long-term dependencies in text.
  - **CNN**: A Convolutional Neural Network that applies filters to capture local features in text.
- **Pre-trained Word Embeddings**: Uses pre-trained GloVe word vectors to initialize the embedding layer for better performance.

## Usage
### Clone the repository:
```bash
git clone https://github.com/your-username/deep-text-classifiers.git
cd deep-text-classifiers
```

### Install dependencies:
Ensure you have the required Python libraries installed:
```bash
pip install torch torchtext spacy pandas numpy scikit-learn
python -m spacy download en_core_web_sm
```

### Run the project:
Execute the `main.py` script to train and evaluate the models:
```bash
python main.py
```

## Results
The project evaluates the performance of different models (RNN, LSTM, CNN) on the text classification task. The results include training and validation accuracy for each model.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
