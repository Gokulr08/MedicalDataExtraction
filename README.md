# Medical Data Extraction Project

Hey there! 👋 I made this cool project to make dealing with medical documents a breeze. Check it out:

- **PDFs to Clear Images:** Used pdf2image to turn those tricky PDFs into clear pictures.
- **Brightening Images:** OpenCV jumps in to fix dark spots, making sure we don't miss a thing.
- **Text Grabbing with pytesseract:** Snatching text from images using pytesseract.
- **Smart Text Extraction:** Used some fancy regular expression tricks to find the important details in the text.
- **Double-Checked with pytest:** Tested it like crazy with pytest, so we're sure we're getting the right patient and prescription details.
- **FastAPI for Easy Testing:** I added FastAPI so testing with Postman is a piece of cake. No need to mess with front-end uploads!

**Tech Stuff:**
- **Image Conversion:** pdf2image
- **Image Enhancement:** OpenCV
- **Text Extraction:** pytesseract
- **Testing:** pytest
- **API Handling:** FastAPI

**Inside the Toolbox:**
- **Notebooks:** Where I did my thinking and worked on samples.
- **Src:** The main place where all the action happens.
  - **Prescription Parser (prescription_parser.py):** Grabs details from prescription documents.
  - **Patient Details (patient_details.py):** Gets patient info.
  - **Generic Parser (parser_generic.py):** The big boss overseeing other classes.
  - **Computer Vision Magic (util.py):** Where all the cool computer vision stuff is.
  - **FastAPI Handling (main.py):** Manages FastAPI for easy testing.
- **Tests:** A bunch of tests to make sure everything runs smoothly.

**Testing How-To:**
1. Run `main.py` in the `src` folder.
2. Grab Postman.
3. Go to `127.0.0.1:8000/extract_from_doc`.
4. Create a collection and pop in key-value pairs:
   - Key: `file format`, Value: Choose either `prescription` or `patient_details`.
   - Key: File path, Value: Upload your file.

Give it a try and see the magic of medical data extraction! 🚀
