# CareerBridge — Online Recruitment Platform

A visually stunning Python web application for job seekers. Browse roles, view details, and submit applications through a modern, dark-themed interface with smooth animations and polished typography.

## Features

- **Home** — Hero section with search, featured job cards, and call-to-action
- **Jobs** — Search and filter by keyword, location, and job type
- **Job detail** — Full description, requirements, and apply CTA
- **Apply** — Simple application form (name, email, resume, cover letter)
- **My Applications** — List of submitted applications (in-memory for demo)
- **About** — Short platform description

## Tech Stack

- **Backend:** Flask (Python)
- **Frontend:** HTML5, CSS3 (custom design system)
- **Fonts:** Outfit (UI), JetBrains Mono (optional)
- **Design:** Dark theme, teal accent, gradient orbs, subtle noise overlay

## Setup

1. **Create a virtual environment (recommended):**
   ```bash
   cd job_platform
   python -m venv venv
   venv\Scripts\activate   # Windows
   # or: source venv/bin/activate   # macOS/Linux
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the app:**
   ```bash
   python app.py
   ```

4. Open **http://127.0.0.1:5000** in your browser.

## Project Report (DOCX)

A formal project report is generated as a Word document. To create or update it:

```bash
pip install -r requirements.txt   # includes python-docx
python generate_report_docx.py
```

This produces `CareerBridge_Project_Report.docx` in the project folder. The report covers: Requirements analysis, System architecture design, MVP implementation, Testing, Documentation, and Final presentation.

## Project Structure

```
job_platform/
├── app.py                      # Flask app, routes, sample data
├── generate_report_docx.py     # Generates CareerBridge_Project_Report.docx
├── CareerBridge_Project_Report.docx  # Project report (run generate_report_docx.py to regenerate)
├── requirements.txt
├── README.md
├── static/
│   └── style.css       # Main styles
└── templates/
    ├── base.html       # Layout, nav, footer
    ├── index.html      # Home / hero + featured jobs
    ├── jobs.html       # Job listing + search
    ├── job_detail.html # Single job view
    ├── apply.html      # Application form
    ├── applications.html # My applications
    └── about.html      # About page
```

## Notes

- This is a **demo project**. Job data is hardcoded and applications are stored in memory (lost on restart).
- For production: add a database (e.g. SQLite/PostgreSQL), user auth, file upload for resumes, and email notifications.

## License

Demo / educational use.
