# English-to-Hinglish-Translation-Using-Transformers

## Overview
This repository contains a simple tool that translates English sentences to Hinglish. Hinglish is a hybrid language that combines Hindi and English, often used in informal communication. This tool allows you to keep specific English words in your sentences while translating the rest to Hinglish.

## Code Explanation
Import Libraries:
We import the necessary libraries from the Transformers library. This includes MarianTokenizer and MarianMTModel.

Load Pretrained Model and Tokenizer:
We load a pre-trained model and tokenizer for English to Hindi translation. The model used here is "Helsinki-NLP/opus-mt-en-hi".

Define English Words to Keep:
We define a list of English words that we want to keep in English when translating to Hinglish. These words won't be translated to Hindi.

Define the Translation Function:
The english_to_hindi_with_selection function takes an English text as input and translates it to Hinglish.

Tokenization and Translation:
Inside the translation function, the input English text is split into words.
We initialize an empty list to store the translated words.

For each word in the input:
If the word (in lowercase) is in the list of English words to keep, we add it to the list of translated words as is.

If the word is not in the list, we proceed to translate it to Hindi:
We tokenize the word.
We use the pre-trained model to generate a Hindi translation for the word.
The translation is decoded and added to the list of translated words.

Reconstruct the Text:
The translated words are joined together to reconstruct the Hinglish output sentence.

Input Sentences:
We provide a list of English sentences that we want to translate to Hinglish.

Translation Loop:
For each sentence in the list of input sentences, we call the english_to_hindi_with_selection function to translate it to Hinglish.
The Hinglish output is printed for each sentence.

## Usage of Transformers

Architecture Overview:
Transformers consist of an encoder and a decoder.
The encoder processes input data, while the decoder generates output.
Each of these consists of multiple layers, and each layer contains multiple attention heads.

Attention Mechanism:
The core innovation of transformers is the attention mechanism.
Attention allows the model to weigh the importance of different parts of the input when making predictions.

Input Encoding:
The input sequence (e.g., a sentence) is first tokenized into subwords or words.
These tokens are then embedded into high-dimensional vectors.
Positional encodings are added to convey the order of tokens.

Attention Layers:
In the encoder, multiple attention layers process the input tokens in parallel.
Each attention layer attends to different parts of the input sequence.

Applications:
Transformers are used in various NLP tasks, including translation, text summarization, sentiment analysis, named entity recognition, and question answering.

Advantages:
Transformers have outperformed traditional NLP models in many benchmarks.
They can capture long-range dependencies in text.
Pre-trained models enable transfer learning for specific tasks.

Challenges:
Transformers require substantial computational resources.
Large models may have millions or even billions of parameters.
Fine-tuning on specific tasks often requires task-specific datasets.


## Table of Contents
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## Getting Started
Follow these steps to get the translator tool up and running on your computer machine.

### Prerequisites
- Python 3.x
- `transformers` library: Install it with `pip install transformers`

### Installation
1. Clone this repository to your local machine. 
2. Navigate to the project directory.
3. Run the translator.

### Output Images
![hinglish](https://github.com/Anjureddyk/English-to-Hinglish-Translation-Using-Transformers/assets/109125485/4d1b7bd5-e35a-4aa0-b4e9-94b3cd1b4c20)

## Contributing
Contributions are welcome! If you'd like to improve this tool, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes.
4. Test your changes.
5. Submit a pull request.





