# PDF Summarization App using GPT-2
This project is a Python-based application that extracts text from PDF files and generates summaries using the GPT-2 model from Hugging Face's transformers library. The summaries are saved in a text file for easy access.

## Features
* Extracts text from PDF files.
* Summarizes large chunks of text using GPT-2.
* Saves the summary in a separate .txt file.

## Requirements

Ensure you have the following libraries installed:

* Python 3.8+
* PyPDF2 for extracting text from PDFs
* transformers for loading the GPT-2 model
* torch for running GPT-2 model
* PyTorch (see PyTorch installation guide)

You can install the necessary dependencies using pip:

<code> pip install PyPDF2 transformers torch </code>

## Usage

1. Clone the repository or download the code.
2. Place the PDF you want to summarize in the project folder.
3. Open the script file and change the path of the PDF in the main section to point to your file.
4. Run the script:
<code> python summarize_app.ipynb </code>

## Known Issues
* Large PDF files: The summarization works by breaking large PDFs into chunks. For extremely large PDFs, the process might take a while.
* Padding Token Warning: GPT-2 doesn't have a native padding token. This is handled by setting the pad_token to eos_token, but it's worth noting in case of any unexpected behavior.
  
## License

This project is licensed under the MIT License. Feel free to use it and modify it as needed.

## Contributing

Feel free to open issues or submit pull requests if you would like to contribute to the project!

Thank you,
Ashen

