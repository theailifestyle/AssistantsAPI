# ChatGPT-like Chat App Using Assistants API

This project is a Streamlit-based web application that leverages OpenAI's Assistants API to provide a ChatGPT-like experience. Users can have real-time conversations with the AI, upload documents to be used as context, and even scrape and convert website content to PDFs to enrich the AI's knowledge base.

OpenAI Assistants API - https://platform.openai.com/docs/assistants/overview

## Features

- **Real-time AI Chat:** Engage in conversations with the AI using OpenAI's GPT models, with the ability to reference uploaded documents.
- **Web Scraping:** Extract text from provided URLs to gather information.
- **PDF Conversion:** Convert scraped text content or any textual data into PDF files.
- **File Upload and Management:** Upload and manage PDF files within the app, which the AI can use as context for the conversations.
- **Contextual Responses:** The AI uses the content of uploaded files to provide informed responses.
- **Citations and References:** The AI includes citations and references to the uploaded documents in its responses, enhancing the reliability of the information provided.

## OpenAI's Assistants API

The Assistants API from OpenAI is a powerful tool that allows developers to integrate conversational AI into their applications. In this app, the Assistants API is used to:

- **Generate Conversations:** Create interactive dialogues with the AI based on the user's prompts.
- **Contextual Understanding:** Utilize the content of uploaded PDFs as context to inform the AI's responses, ensuring that the conversation is relevant and informed by the provided material.
- **File Handling:** Upload and associate files with the AI assistant to be used during conversations.
- **Citations:** Automatically generate citations from the uploaded files when referenced in the AI's responses, allowing for clear sourcing of information.

## Requirements

- Python 3.6 or higher
- Streamlit
- OpenAI Python package
- Requests library
- BeautifulSoup library (for web scraping)
- PDFKit library (for PDF conversion)
- wkhtmltopdf (PDFKit dependency)

## Setup Instructions

1. **Install Dependencies:**

    ```bash
    pip install streamlit openai requests beautifulsoup4 pdfkit
    ```

2. **API Key Configuration:**

    Securely input your OpenAI API key into the Streamlit app's sidebar to authenticate your API requests.

3. **wkhtmltopdf Installation:**

    Ensure that `wkhtmltopdf` is installed and accessible in your system's PATH. This is necessary for PDF conversion with `pdfkit`.

## Usage Guide

1. Run the Streamlit app:

    ```bash
    streamlit run app.py
    ```

2. Input your OpenAI API key in the provided sidebar field.
3. Optionally, scrape web content and convert it to a PDF for the AI to use as context.
4. Upload any documents you want the AI to reference during the conversation.
5. Initiate the chat by clicking "Start Chat" and begin your conversation with the AI.

## Application Notes

- Always ensure you have the right to scrape content from websites and to use any uploaded documents.
- The chat interface activates after the "Start Chat" button is clicked, and the uploaded files are processed.

## Contributing

If you'd like to contribute to the project, please fork the repository and issue a pull request with your suggested changes.

## License

This project is licensed under the [MIT License](LICENSE.md).

---

The inline comments in the source code provide further details and can guide you through the application's functionality and structure.
