# QueryBot for Godrej

## Overview

QueryBot for Godrej is a Streamlit-based application that allows users to upload PDF, Word, or PowerPoint documents, extract text and images, summarize the text using the Cohere API, and answer questions related to the document's content. The app also includes a text-to-speech feature to convert summarized text or answers into audio, making it accessible for a wider audience. Designed for ease of use, QueryBot helps streamline the process of extracting and understanding document information.

## Features

- **Document Upload**: Supports PDF, Word, and PowerPoint files.
- **Text Extraction**: Extracts text from uploaded documents.
- **Summarization**: Summarizes extracted text using Cohere API.
- **Question Answering**: Answers questions based on the document's content.
- **Text-to-Speech**: Converts summarized text or answers to speech.

## Installation

1. Clone the repository:

   ```sh
   git clone https://github.com/your-username/your-repository.git
   cd your-repository
2. Install the required packages:
   pip install -r requirements.txt
Run the Streamlit app:

sh

    streamlit run app.py

    Open your web browser and go to http://localhost:8501.

    Upload a document (PDF, Word, or PowerPoint) and use the various features provided by the app.

Configuration

Ensure you have your Cohere API key set up in the app.py file:

python

COHERE_API_KEY = 'your-cohere-api-key'
co = cohere.Client(COHERE_API_KEY)

Replace 'your-cohere-api-key' with your actual API key from Cohere.
File Structure

bash

├── app.py                 # Main application file
├── requirements.txt       # List of required Python packages
└── README.md              # Project documentation

Dependencies

    streamlit: Streamlit library for building interactive web applications.
    pdf2image: Convert PDF pages to images.
    cohere: Cohere API for text summarization and question answering.
    Pillow: Python Imaging Library (PIL) for image processing.
    python-docx: To handle Word documents.
    python-pptx: To handle PowerPoint presentations.
    gtts: Google Text-to-Speech for converting text to audio.
