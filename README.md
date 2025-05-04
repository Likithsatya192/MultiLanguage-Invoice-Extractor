# MultiLanguage Invoice Extractor

The **MultiLanguage Invoice Extractor** is a Streamlit-based application that uses Google's Gemini AI model to extract and interpret information from invoice images. The application supports multilingual queries, providing responses in the language of the question.

## Features

- Upload invoice images in formats like `.jpg`, `.jpeg`, and `.png`.
- Extract and interpret invoice details using the Gemini AI model.
- Multilingual support for queries and responses.
- Simple and interactive web interface built with Streamlit.

## Project Structure

```
.env
.python-version
main.py
pyproject.toml
README.md
requirements.txt
uv.lock
```

## Installation

Follow these steps to set up and run the project:

1. **Clone the Repository**  
   Clone this repository to your local machine:
   ```sh
   git clone https://github.com/Likithsatya192/MultiLanguage-Invoice-Extractor.git
   cd Multilanguage-Invoice-Extractor
   ```

2. **Install `uv`**  
   Install `uv` for managing the environment:
   ```sh
   pip install uv
   ```

3. **Set Up the Environment**  
   Use `uv` to create and activate the environment:
   ```sh
   uv init
   uv venv
   .venv\Scripts\activate
   ```

4. **Install Dependencies**  
   Install the required libraries:
   ```sh
   pip install -r requirements.txt
   ```

5. **Set Up Environment Variables**  
   Create a `.env` file in the project root (if not already present) and add your Gemini API key:
   ```
   GEMINI_API_KEY="your-api-key-here"
   ```

6. **Run the Application**  
   Start the Streamlit application:
   ```sh
   streamlit run main.py
   ```

## Usage

1. Open the application in your browser (usually at `http://localhost:8501`).
2. Enter a prompt in the input field.
3. Upload an invoice image.
4. Click the "Tell me about the invoice" button to get a response.

## Dependencies

The project requires the following libraries:

- `streamlit>=1.45.0`
- `google-generativeai>=0.8.5`
- `python-dotenv>=1.1.0`
- `langchain>=0.3.25`
- `pypdf2>=3.0.1`
- `chroma>=0.2.0`
