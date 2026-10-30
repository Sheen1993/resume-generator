# Resume Generator

Generates `Sheen_Michael_Aking_Resume.html` and `Sheen_Michael_Aking_Resume.pdf` from the HTML/CSS embedded in `generate_resume.py`, using [WeasyPrint](https://weasyprint.org/).

## Requirements

- Python 3.9+
- WeasyPrint system libraries (Pango). On Ubuntu/Debian/WSL:

  ```bash
  sudo apt install python3-venv libpango-1.0-0 libpangoft2-1.0-0 fonts-liberation
  ```

  For macOS/Windows, see the [WeasyPrint install guide](https://doc.courtbouillon.org/weasyprint/stable/first_steps.html).

## Setup

```bash
python3 -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

## Run

```bash
python generate_resume.py
```

Output files are written to the current directory:

- `Sheen_Michael_Aking_Resume.html`
- `Sheen_Michael_Aking_Resume.pdf`

## Editing

Edit the `html_content` string in `generate_resume.py` to change the resume's content or styling, then run the script again.
