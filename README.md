
# Medical Assistant Chatbot

A Streamlit-based medical assistant chatbot that analyzes blood test results, provides expected diagnoses, and answers user queries based on the provided context and document data. This chatbot integrates LangChain, FAISS vector stores, OpenAI GPT models, and PDF parsing for enhanced functionality.

## Features

- Analyze blood test results and provide medical insights.
- Generate recommendations and disclaimers.
- Interactive follow-up question support.
- Ability to upload and process PDF documents for medical context.
- Export chatbot responses as PDF files.
- Dynamic user interface with a customized background.

## Technologies Used

- **Streamlit**: For creating an interactive web app.
- **LangChain**: For document retrieval and question answering.
- **OpenAI GPT-4o-mini**: For natural language processing.
- **FAISS**: For efficient vector similarity search.
- **PDFPlumber**: For extracting text and tables from PDF files.
- **ReportLab**: For generating downloadable PDF responses.

## Requirements

- Python 3.8 or higher
- OpenAI API Key

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/YourRepoName/MedicalAssistantChatbot.git
   cd MedicalAssistantChatbot
   ```

2. **Set Up Virtual Environment**:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Prepare the PDF File**:
   - Place your PDF file (e.g., `interpretation-of-full-blood-count-parameters-in-health-and-disease.pdf`) in the project directory.

5. **Run the App**:
   ```bash
   streamlit run Project_8_streamlit.py
   ```

## Usage

1. **Enter Your OpenAI API Key**:
   - Input your API key in the sidebar to initialize the chatbot.

2. **Analyze Blood Test Results**:
   - Enter blood test parameters like WBC, RBC, Hgb, etc.
   - Click "Analyze Blood Test Results" to get insights.

3. **Ask Follow-up Questions**:
   - Type your follow-up questions in the provided field and receive answers.

4. **Download Analysis as PDF**:
   - After analysis, click "Download Response as PDF" to save the results locally.

## File Structure

- `Project_8_streamlit.py`: Main application code.
- `requirements.txt`: List of dependencies.
- `README.md`: Documentation.
- `faiss_index`: Local FAISS index for document retrieval (generated dynamically).
- PDF file (e.g., `interpretation-of-full-blood-count-parameters-in-health-and-disease.pdf`): Medical document for context.

## Dependencies

The following dependencies are required to run the chatbot:

- `streamlit`
- `langchain`
- `faiss-cpu`
- `openai`
- `pdfplumber`
- `reportlab`

Install them using the command:
```bash
pip install -r requirements.txt
```

## Notes

- The chatbot is designed for educational and informational purposes only.
- It does not provide definitive medical diagnoses. Always consult a medical professional for health-related concerns.

