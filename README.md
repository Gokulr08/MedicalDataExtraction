# Medical Data Extraction Project
This is a Codebasics assignment that I handled fully on my own.

### How I Tackled It:
- **PDFs to Clear Images:** I used pdf2image to convert tricky PDFs into clear images.
- **Brightening Images:** OpenCV helped me fix dark spots so I wouldn’t miss any details.
- **Text Extraction with Pytesseract:** I pulled text from the images using pytesseract.
- **Smart Text Extraction:** With some clever regex, I pinpointed key details in the text.
- **Reliable Testing with Pytest:** I rigorously tested with pytest to ensure accurate patient and prescription details.
- **FastAPI for Quick Testing:** I integrated FastAPI to make testing a breeze with Postman—no need for front-end file uploads!

### Tools and Tech:
- **Image Conversion:** pdf2image
- **Image Enhancement:** OpenCV
- **Text Extraction:** pytesseract
- **Testing:** pytest
- **API Handling:** FastAPI

### Project Layout:
- **Notebooks:** Where I brainstormed and tested sample data.
- **Src:** The core of the project.
  - **Prescription Parser (prescription_parser.py):** Extracts details from prescriptions.
  - **Patient Details (patient_details.py):** Pulls patient info.
  - **Generic Parser (parser_generic.py):** Manages all parsing classes.
  - **Computer Vision Magic (util.py):** Handles the image processing tasks.
  - **FastAPI Handling (main.py):** Runs FastAPI for testing.
- **Tests:** A suite of tests to ensure everything works well.

### Testing Instructions:
1. Run `main.py` in the `src` folder.
2. Open Postman.
3. Go to `127.0.0.1:8000/extract_from_doc`.
4. Add key-value pairs:
   - Key: `file format`, Value: `prescription` or `patient_details`.
   - Key: File path, Value: Upload your file here.
