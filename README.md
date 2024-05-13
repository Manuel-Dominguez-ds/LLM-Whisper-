Testing Language Models (LLMs) in Google Colab
This repository contains code for testing and utilizing Language Models (LLMs) using Google Colab. It demonstrates how to use different models for automatic speech recognition (ASR) and text summarization tasks.

Setup
To run the provided code, follow these steps:

1. Clone the Repository
Clone this repository to your local machine using Git:

git clone https://github.com/your-username/llm-testing.git
2. Install Dependencies
Ensure you have the required Python packages installed. You can use the following commands to install them:

 !pip install -q -U bitsandbytes
 !pip install -q -U git+https://github.com/huggingface/transformers.git
 !pip install -q -U git+https://github.com/huggingface/peft.git
 !pip install -q -U git+https://github.com/huggingface/accelerate.git
 !pip install -q -U einops
 !pip install -q -U safetensors
 !pip install -q -U torch
 !pip install -q -U xformers
 !pip install -q -U langchain
 !pip install -q -U ctransformers[cuda]
 !pip install chromadb
 !pip install sentence-transformers

3. Set Up Google Colab
You will need access to Google Colab to run the provided code interactively in a Jupyter notebook environment.

4. Upload Audio File
Upload an audio file (heard.mp3) containing the conversation you want to process to the root directory of your Google Colab notebook.

Usage
Open the llm_testing.ipynb notebook in Google Colab.
Run each cell sequentially to execute the code.
The notebook will perform automatic speech recognition (ASR) on the uploaded audio file and generate a textual transcript (new_text).
The code will then use a pretrained language model (LLM) to summarize the main points discussed in the conversation.

The summarized text will be displayed as the output.
Repository Structure

llm-testing/
│
├── llm_testing.ipynb      # Jupyter notebook for testing LLMs in Google Colab
├── heard.mp3              # Sample audio file containing the conversation
├── requirements.txt       # List of Python dependencies
└── README.md              # Repository README file (you are here)

References
Hugging Face Transformers
Google Colab
PyTorch

License
This project is licensed under the MIT License - see the LICENSE file for details.
