# Neural Machine Translation for Date Normalization

This project focuses on Neural Machine Translation (NMT) using a Sequence-to-Sequence (Seq2Seq) model with an optional Attention Mechanism. The goal is to translate human-readable dates (e.g., "Monday May 7 1983") into machine-readable formats (e.g., "1983-05-07"). The project includes data generation, model training, and evaluation using PyTorch.

## Project Structure
The project is organized into the following files:

| File Name | Description |
|-----------|-------------|
| **dataloader.py** | Handles data generation, preprocessing, and vocabulary creation. |
| **models.py** | Contains the implementation of the Seq2Seq model with optional attention. |
| **main.py** | The main script for data loading, model training, and evaluation. |

## Dataset
The dataset is generated synthetically using the **Faker** library. It consists of human-readable dates in various formats (e.g., "Monday May 7 1983") and their corresponding machine-readable formats (e.g., "1983-05-07").

## Features
- **Seq2Seq Model**: A Sequence-to-Sequence model with an Encoder-Decoder architecture.
- **Attention Mechanism**: Optional attention mechanism to improve translation accuracy.
- **Custom Data Generation**: Uses the Faker library to generate synthetic date data.
- **Preprocessing**: Handles tokenization, vocabulary creation, and data batching.
- **Training and Evaluation**: Includes training loops and evaluation metrics.

## Usage
### 1. Clone the Repository
```bash
git clone https://github.com/your-username/DateTranslator.git
cd DateTranslator
```

### 2. Install Dependencies
Ensure you have the required Python libraries installed:
```bash
pip install torch numpy pandas faker tqdm sklearn keras
```

### 3. Run the Project
Execute the `main.py` script to train and evaluate the model:
```bash
python main.py
```

### 4. Test the Model
After training, you can test the model on custom date strings by modifying the `sents` list in `main.py`.

## Results
The project evaluates the performance of the Seq2Seq model with and without the attention mechanism. The results include training loss and the ability to translate new date strings.

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvement, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments
- **PyTorch**: For providing the deep learning framework.
- **Faker**: For generating synthetic date data.
- **Keras**: For utility functions like `to_categorical`.
