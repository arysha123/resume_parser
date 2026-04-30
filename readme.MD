# Resume Parser

An AI-powered resume analysis tool that extracts information from resumes and matches them against job descriptions using the Groq API.

## 📋 Overview

This web application allows users to upload their resumes (PDF or DOCX) along with a job description, and receive an AI-powered analysis of how well the resume matches the job requirements. Built with Flask and powered by Groq's language models, it provides intelligent insights for job seekers and recruiters.

## ✨ Features

- **Multi-format Support**: Accepts both PDF and DOCX resume formats
- **Text Extraction**: Efficiently extracts text content from uploaded resumes
- **AI-Powered Analysis**: Leverages Groq's language models for intelligent resume evaluation
- **Job Matching**: Compares resume content against job descriptions
- **User-Friendly Interface**: Simple web interface for easy interaction
- **Real-time Processing**: Quick analysis and feedback

## 🚀 Getting Started

### Prerequisites

- Python 3.7 or higher
- pip (Python package manager)
- A Groq API key ([Get one here](https://console.groq.com))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/arysha123/resume_parser.git
   cd resume_parser
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   
   Create a `.env` file in the project root:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```

### Running the Application

1. **Start the Flask server**
   ```bash
   python app.py
   ```

2. **Access the application**
   
   Open your browser and navigate to:
   ```
   http://localhost:5000
   ```

3. **Upload and analyze**
   - Upload your resume (PDF or DOCX)
   - Paste the job description
   - Click submit to get your analysis

## 📁 Project Structure

```
resume_parser/
├── app.py                 # Main Flask application
├── resume_extractor.py    # Resume text extraction module
├── groq_client.py        # Groq API integration
├── requirements.txt       # Python dependencies
├── .gitignore            # Git ignore rules
├── templates/            # HTML templates
│   └── index.html        # Main web interface
├── static/               # Static files (CSS, JS)
└── uploads/              # Temporary storage for uploaded files
```

## 🛠️ Technologies Used

- **Flask**: Web framework for Python
- **pdfplumber**: PDF text extraction
- **python-docx**: DOCX file processing
- **Groq API**: AI-powered resume analysis
- **python-dotenv**: Environment variable management

## 📦 Dependencies

```
Flask
requests
pdfplumber
python-docx
python-dotenv
```

## 🔧 Configuration

The application uses environment variables for configuration. Create a `.env` file with the following:

| Variable | Description | Required |
|----------|-------------|----------|
| `GROQ_API_KEY` | Your Groq API key for AI analysis | Yes |

## 🔒 Security Notes

- Never commit your `.env` file or API keys to version control
- The `.gitignore` file is configured to exclude sensitive files
- Uploaded files are stored temporarily and should be cleaned regularly in production

## 📝 Usage Example

1. Prepare your resume in PDF or DOCX format
2. Find a job description you want to match against
3. Open the application in your browser
4. Upload your resume
5. Paste the job description in the text area
6. Submit and review the AI-generated analysis


## 🐛 Known Issues

- Large resume files may take longer to process
- Scanned PDFs without OCR may not extract text properly

## 🔮 Future Enhancements

- [ ] Support for additional file formats (RTF, TXT)
- [ ] Resume scoring and ranking system
- [ ] Export analysis results to PDF
- [ ] Batch processing for multiple resumes
- [ ] Resume optimization suggestions
- [ ] Skills gap analysis
- [ ] ATS (Applicant Tracking System) compatibility checker

## 📄 License

This project is open source. Please check the repository for license details.

## 👤 Author

**arysha123**

- GitHub: [@arysha123](https://github.com/arysha123)

## 🙏 Acknowledgments

- Original project forked from [@assassindiv](https://github.com/assassindiv/resume_parser)
- Powered by [Groq](https://groq.com) for fast AI inference
- Built with Flask and open-source libraries

## ⚠️ Disclaimer

This tool is designed to assist with resume analysis and should not be the sole factor in hiring decisions. Always review results critically and consider human judgment in recruitment processes.

---

**Note**: Make sure to keep your Groq API key secure and never share it publicly.
