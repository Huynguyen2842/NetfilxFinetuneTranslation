# Netflix Fine-Tuned Translation Script

## Overview

This script is designed to utilize a fine-tuned translation model to translate text from one language to another. It is based on the `transformers` library and supports various language pairs through the fine-tuned models available on the `transformers` model hub.

## Prerequisites

- Python 3.x
- `transformers` library
- `datasets` library
- Internet connection (for downloading the model and tokenizer)

## Setup

1. Install the required libraries:
   ```shell
   pip install transformers datasets
2. Clone the repository or download the script to your local machine.

## Usage 
To use the script for translation, you need to specify the source and target languages. The script is currently set up for English to Chinese translation (en to zh). To change the language pair, modify the SOURCE_LANG and TARGET_LANG variables in the script.

For example, to translate from English to Vietnamese:

**Example for English to Vietnamese translation:**
```python
SOURCE_LANG = "en"
TARGET_LANG = "vi"
```
## Prepare Your Text File
Place the text you want to translate in a file named `original_english_text.txt` (or any name you prefer, but make sure to update the script accordingly).

## Usage
Run the script using the following command:
```bash
python3 validate.py
```
The script will process the text and save the translated content in a file named netflix_[SOURCE_LANG]_[TARGET_LANG]_translation.txt (e.g., netflix_en_vi_translation.txt for English to Vietnamese translation).

## Notes

- The script relies on models from the transformers model hub. Make sure that the model you choose supports your language pair.
- Translation quality varies depending on the model's capabilities. Some language pairs may yield better results than others.

## Troubleshooting
If you encounter any issues:

- Check if the transformers and datasets libraries are correctly installed.
- Ensure that the source text file exists and is correctly named in the script.
- Verify that the chosen model supports your language pair and is correctly named in the script.

## Support
For more information, consult the transformers library documentation or reach out to the repository maintainer for assistance.
