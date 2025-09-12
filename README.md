# ATS Resume Expert
<img width="1365" height="602" alt="Screenshot 2025-09-08 144508" src="https://github.com/user-attachments/assets/4a947d54-85fd-412b-93f4-48760e74e8bd" />

A Streamlit application that analyzes resumes against job descriptions using Google's Gemini AI model to provide professional feedback and ATS compatibility scoring.

## Features

- Resume analysis against job descriptions
- Professional HR manager feedback
- ATS compatibility percentage scoring
- Missing keywords identification
- PDF resume support with image processing

## Requirements

```txt
python >= 3.7
streamlit
python-dotenv
google-generativeai
pdf2image
Pillow
```

## Setup

1. Clone the repository
2. Install the required packages:
```bash
pip install streamlit python-dotenv google-generativeai pdf2image Pillow
```

3. Create a `.env` file in the root directory and add your Google API key:
```
GOOGLE_API_KEY=your-google-api-key-here
```

4. Run the Streamlit app:
```bash
streamlit run resume.py
```

## Usage

1. Enter the job description in the text area
2. Upload your resume in PDF format
3. Choose one of the analysis options:
   - "Tell Me About the Resume" - Get detailed HR feedback
   - "Percentage match" - Get ATS compatibility score

## How it Works

The application:
1. Converts uploaded PDF resumes to images
2. Processes the images for AI analysis
3. Uses Google's Gemini Pro model to analyze the content
4. Provides detailed feedback and scoring based on job requirements

## Note

Make sure you have a valid Google API key with access to the Gemini Pro model. The application uses Gemini 1.5 Pro for analysis.
![Uploading Screenshot 2025-09-08 144508.png…]()

## License
