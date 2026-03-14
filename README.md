<p><small>Best viewed in <a href="https://github.com/settings/appearance">Light Mode</a> and Desktop Site (Recommended)</small></p>

<div align="center">
  <h1>🌴 AI Resume Analyzer 🌴</h1>
  <p>A tool to parse resumes, extract key data, and provide actionable improvements.</p>

  <h4>
    <a href="#features">Features</a>
    <span> · </span>
    <a href="#setup">Setup</a>
    <span> · </span>
    <a href="#usage">Usage</a>
  </h4>

  <small align="justify">🚀 Built and maintained by <strong>Pramod Kumar</strong></small>
</div>

---

## About
<div align="center">
    <br/><img src="screenshots/RESUME.png" alt="screenshot" /><br/><br/>
    <p align="justify">
      Upload a resume (PDF/DOCX/TXT) and get structured data, scoring, and recommendations powered by NLP.
    </p>
</div>

## Scope

- Convert resumes into structured, tabular data (CSV/DB) for analytics.
- Provide resume scoring and actionable recommendations.
- Help users iterate on their resume by highlighting missing skills and keywords.
- Enable organizations to analyze resume trends (roles, locations, skills).

<!-- TechStack -->
## Tech Stack 🍻
<details>
  <summary>Frontend</summary>
  <ul>
    <li><a href="https://streamlit.io/">Streamlit</a></li>
    <li><a href="https://developer.mozilla.org/en-US/docs/Learn/HTML">HTML</a></li>
    <li><a href="https://developer.mozilla.org/en-US/docs/Web/CSS">CSS</a></li>
    <li><a href="https://developer.mozilla.org/en-US/docs/Learn/JavaScript">JavaScript</a></li>
  </ul>
</details>

<details>
  <summary>Backend</summary>
  <ul>
    <li><a href="https://streamlit.io/">Streamlit</a></li>
    <li><a href="https://www.python.org/">Python</a></li>
  </ul>
</details>

<details>
<summary>Database</summary>
  <ul>
    <li><a href="https://www.mysql.com/">MySQL</a></li>
  </ul>
</details>

<details>
<summary>Modules</summary>
  <ul>
    <li><a href="https://pandas.pydata.org/">pandas</a></li>
    <li><a href="https://github.com/OmkarPathak/pyresparser">pyresparser</a></li>
    <li><a href="https://pypi.org/project/pdfminer3/">pdfminer3</a></li>
    <li><a href="https://plotly.com/">Plotly</a></li>
    <li><a href="https://www.nltk.org/">NLTK</a></li>
  </ul>
</details>

<!-- Features -->
## Features 🤦‍♂️
### Client: -
- Fetching Location and Miscellaneous Data

  Using Parsing Techniques to fetch
- Basic Info
- Skills
- Keywords

Using logical programs, it will recommend
- Skills that can be added
- Predicted job role
- Course and certificates
- Resume tips and ideas
- Overall Score
- Interview & Resume tip videos

### Admin: -
- Get all applicant’s data into tabular format
- Download user’s data into csv file
- View all saved uploaded pdf in Uploaded Resume folder
- Get user feedback and ratings
  
  Pie Charts for: -
- Ratings
- Predicted field / roles
- Experience level
- Resume score
- User count
- City
- State
- Country

### Feedback: -
- Form filling
- Rating from 1 – 5
- Show overall ratings pie chart
- Past user comments history 

## Requirements 😅
### Have these things installed to make your process smooth 
1) Python (3.9.12) https://www.python.org/downloads/release/python-3912/
2) MySQL https://www.mysql.com/downloads/
3) Visual Studio Code **(Prefered Code Editor)** https://code.visualstudio.com/Download
4) Visual Studio build tools for C++ https://aka.ms/vs/17/release/vs_BuildTools.exe

## Setup & Installation 👀

To run this project, perform the following tasks 😨

Download the code file manually or via git
```bash
git clone https://github.com/PRAMODKUMAR/AI-Resume-Analyzer.git
```

Create a virtual environment and activate it **(recommended)**

Open your command prompt and change your project directory to ```AI-Resume-Analyzer``` and run the following command 
```bash
python -m venv venvapp

cd venvapp/Scripts

activate

```

Downloading packages from ```requirements.txt``` inside ``App`` folder
```bash
cd../..

cd App

pip install -r requirements.txt

python -m spacy download en_core_web_sm

```

After installation is finished create a Database ```cv```

And change user credentials inside `App/App.py` (look for the `mysql.connector.connect(...)` call).

If you encounter parsing issues, replace the installed `pyresparser` parser with the version included in this repo:

- Copy `pyresparser/resume_parser.py` from this project into your virtual environment's `Lib\site-packages\pyresparser/` folder (overwrite if prompted).

Once dependencies are installed, you should be ready to run the app.

Run the ```App.py``` file using
```bash
streamlit run App.py

```

## Troubleshooting

- If you see `GeocoderUnavailable`, ensure your machine has an active internet connection.
- If resume parsing fails, try a different file format (PDF, DOCX, TXT).

---

## Usage

- Run the app (see **Setup** section).
- Upload a resume in the **Upload Resume** section.
- View parsed details, resume score, and improvement suggestions.
- (Optional) Use sample resumes in `App/Uploaded_Resumes/`.

---

## Contributing 🤘

Pull requests are welcome.

For significant changes, please open an issue first to discuss the plan.
