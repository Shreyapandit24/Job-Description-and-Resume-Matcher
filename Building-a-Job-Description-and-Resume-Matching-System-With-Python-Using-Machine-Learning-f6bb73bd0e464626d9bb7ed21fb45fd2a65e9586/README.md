# Job Description and Resume Matching System

A web-based application that uses machine learning to match job descriptions with resumes, streamlining the recruitment process by automatically identifying suitable candidates based on similarity scores.

## Features

- **Job Description Input:** Recruiters can enter job descriptions directly into the system.
- **Resume Upload:** Supports uploading multiple resumes in PDF, DOCX, or TXT formats.
- **Intelligent Matching:** Utilizes TF-IDF vectorization and cosine similarity to compute match scores.
- **Top Results Display:** Shows the top 5 matching resumes with their similarity scores.
- **Responsive UI:** Built with Bootstrap for a clean, user-friendly interface.

## Technologies Used

- **Backend:** Python, Flask
- **Machine Learning:** scikit-learn (TF-IDF, Cosine Similarity)
- **Document Processing:** PyPDF2, docx2txt
- **Frontend:** HTML, CSS, Bootstrap
- **Deployment:** Heroku-ready with Procfile and requirements.txt

## Installation

### Prerequisites
- Python 3.8 or higher
- pip (Python package installer)

### Local Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/job-resume-matcher.git
   cd job-resume-matcher
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the application:
   ```bash
   python main.py
   ```

4. Open your browser and navigate to `http://localhost:5000`

## Usage

1. On the home page, enter a job description in the text area.
2. Upload one or more resume files (PDF, DOCX, or TXT format).
3. Click "Match Resumes" to process the matching.
4. View the top 5 matching resumes with their similarity scores.

## Deployment

### Heroku Deployment
1. Ensure you have a Heroku account and Heroku CLI installed.
2. Create a new Heroku app:
   ```bash
   heroku create your-app-name
   ```
3. Push your code to Heroku:
   ```bash
   git push heroku main
   ```
4. Open the deployed app:
   ```bash
   heroku open
   ```

### Other Platforms
The application can be deployed to any platform supporting Python/Flask apps (e.g., AWS, DigitalOcean, etc.) using the provided `Procfile` and `requirements.txt`.

## Project Structure

```
├── main.py                 # Main Flask application
├── matchresume.html        # Frontend template
├── requirements.txt        # Python dependencies
├── Procfile               # Heroku deployment configuration
├── .gitignore             # Git ignore file
├── README.md              # Project documentation
└── Resume_List/           # Sample resume files
```

## API Endpoints

- `GET /`: Home page with upload form
- `POST /matcher`: Process resume matching

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Built with Flask web framework
- Machine learning powered by scikit-learn
- UI styled with Bootstrap



