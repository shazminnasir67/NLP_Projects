# Named Entity Recognition with BiLSTM-CRF

This project focuses on Named Entity Recognition (NER) using a Bidirectional LSTM (BiLSTM) combined with a Conditional Random Field (CRF). The goal is to identify and classify entities (e.g., names, locations, organizations) in text data. The project includes data preprocessing, model training, and evaluation using PyTorch.


## Project Structure
The project is organized into the following files:

| File Name | Description |
|-----------|-------------|
| **dataloader.py** | Handles data loading, preprocessing, and vocabulary creation for NER tasks. |
| **models.py** | Contains the implementation of the BiLSTM-CRF model for NER. |
| **main.py** | The main script for data loading, model training, and evaluation. |
| **model.pkl** | A pre-trained model file saved after training. |

## Dataset
The dataset used in this project is the **CoNLL-2003 NER dataset**, which contains annotated text data with entities categorized into four classes:
- **PER** (Person)
- **LOC** (Location)
- **ORG** (Organization)
- **MISC** (Miscellaneous)

## Features
- **BiLSTM-CRF Model**: Combines the power of Bidirectional LSTM for sequence modeling with CRF for structured prediction.
- **Pre-trained Word Embeddings**: Uses GloVe word vectors to initialize the embedding layer for better performance.
- **Custom Data Loader**: Handles tokenization, vocabulary creation, and data batching.
- **Model Saving and Loading**: The trained model is saved as `model.pkl` for future use.

## Usage
### 1. Clone the Repository
```bash
git clone https://github.com/your-username/NER-BiLSTM-CRF.git
cd NER-BiLSTM-CRF
```

### 2. Install Dependencies
Ensure you have the required Python libraries installed:
```bash
pip install torch torchtext spacy pandas numpy
python -m spacy download en_core_web_sm
```

### 3. Run the Project
Execute the `main.py` script to train and evaluate the model:
```bash
python main.py
```

### 4. Test the Model
After training, you can test the model on custom sentences by modifying the `test_sents` list in `main.py`.

## Results
The project evaluates the performance of the BiLSTM-CRF model on the CoNLL-2003 NER dataset. The results include training and validation accuracy, as well as the ability to predict entities in new sentences.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- **PyTorch**: For providing the deep learning framework.
- **GloVe**: For pre-trained word embeddings.
- **CoNLL-2003**: For providing the NER dataset.

## Example Output
After training, the model can predict entities in custom sentences. For example:

```python
test_sents = ["My name is Phil , I am from European Union ."]
# Output:
# My name is Phil , I am from European Union . --> ['O', 'O', 'O', 'B-PER', 'O', 'O', 'O', 'B-ORG', 'I-ORG', 'O']
