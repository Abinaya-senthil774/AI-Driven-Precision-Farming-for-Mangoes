# Project Structure

This document describes the restructured Mango AI project organization.

## Directory Structure

```
mango_code/
├── src/                          # Main application source code
│   ├── __init__.py
│   ├── app.py                    # Main Streamlit application entry point
│   ├── config/                   # Configuration module
│   │   ├── __init__.py
│   │   └── settings.py           # All configuration settings and paths
│   ├── pages/                    # Streamlit page modules
│   │   ├── __init__.py
│   │   ├── welcome.py            # Welcome/home page
│   │   ├── about.py              # About page
│   │   ├── variety.py            # Mango variety classification page
│   │   ├── disease.py            # Disease detection page
│   │   ├── ripeness.py           # Ripeness analysis page
│   │   └── damage.py             # Fruit damage/grading page
│   └── utils/                    # Utility modules
│       ├── __init__.py
│       ├── ripeness.py           # Ripeness detection utilities
│       ├── disease_detection.py  # Disease detection utilities
│       ├── fruit_grading.py      # Fruit grading utilities
│       └── variety_prediction.py # Variety prediction utilities
├── assets/                       # Static assets
│   └── images/                   # Image assets for the UI
├── models/                       # Model files (not in git)
│   ├── disease_detection/
│   ├── fruit_variety/
│   ├── fruit_grading/
│   └── ripeness/
├── training/                     # Training scripts (kept separate)
│   ├── disease_detector/
│   ├── fruit_grading/
│   ├── mango_classifier/
│   └── mango_ripeness/
├── temp/                         # Temporary files directory
├── main.py                       # Main entry point (run: streamlit run main.py)
├── requirements.txt              # Python dependencies
├── .gitignore                   # Git ignore rules
└── PROJECT_STRUCTURE.md         # This file
```

## Running the Application

```bash
# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run main.py
```


