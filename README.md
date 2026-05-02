# Praveen George — Professional Portfolio & Content Hub

Welcome to the professional portfolio workspace of **Praveen George**, Research Analyst and Financial Content Creator. 

This repository contains a dynamic, automated system designed to maintain an updated collection of written articles, industry reports, and video content, presenting them across high-performance, visually premium media.

---

## 📂 Repository Contents

The workspace contains the source materials, deployment files, and automation scripts used to build and refresh the digital portfolio:

```
Praveen Portfolio/
├── deploy/
│   └── index.html                       # Modern, animated digital portfolio web application
├── Praveen_George_Portfolio.xlsx        # Automatically generated unified Excel portfolio
├── Praveen_George_Resume.docx           # Source/Working resume file
├── Praveen_George_Resume_Updated.docx   # Updated professional resume
├── Praveen_George_Resume_Updated.pdf    # Print-ready professional resume in PDF format
├── refresh_portfolio.py                 # Core Python script to compile source content
├── Refresh Portfolio.bat                # One-click Windows execution script
└── README.md                            # Documentation and usage guide (this file)
```

---

## 🛠️ Portfolio Automation Engine

The core logic of the portfolio is powered by `refresh_portfolio.py`, which integrates content from separate sources (Excel files, web archives, video catalogs) into a single master layout file:

### 1. Unified Excel Portfolio Generator
The script aggregates your authored articles (Tradejini Blog) and YouTube videos. It updates `Praveen_George_Portfolio.xlsx` automatically:
- **Summary Tab**: High-level dashboard showcasing featured content, key statistics, and blog categories.
- **Featured Tab**: Customizable section where you can select specific best-performing blogs and videos.
- **All Content Tab**: Chronologically sorted historical feed of all pieces.
- **Category Specific Tabs**: Individual sheets for pure blogs and pure videos, completely styled and formatted.

### 2. High-End Web Portfolio
The `deploy/index.html` file acts as the public web-facing showcase of this portfolio. It is designed with:
- **Rich Aesthetics**: Custom dark-mode interface with elegant gradients, neon highlights, and frosted-glass components.
- **Dynamic Content Tabs**: Switch cleanly between written articles and videos.
- **Advanced Filtering**: Categorical pills to isolate specific analytical topics (e.g., Company Analysis, Sector Reports).
- **SEO & Responsiveness**: Optimized metadata, fast rendering, and full responsiveness on mobile screens.

---

## 🔄 How to Update the Content

Updating your digital presence or adding newly published blogs/videos takes only a few steps:

### Step 1: Add New Content
- **New Blogs**: Add new articles to your source Blogs Excel file (`Praveen_George_Blogs_v8.xlsx`).
- **New Videos**: Enter new videos directly into the "Videos Only" tab of the master portfolio file.

### Step 2: Configure Paths (One-Time Setup)
Open `refresh_portfolio.py` in a text editor (e.g., VS Code or Notepad) and update the exact absolute file paths to your source spreadsheets at the top of the file:
```python
BLOGS_FILE     = r"C:\Users\YourName\Documents\Praveen_George_Blogs_v8.xlsx"
PORTFOLIO_FILE = r"C:\Users\YourName\Desktop\Praveen Portfolio\Praveen_George_Portfolio.xlsx"
```

### Step 3: Run the Refresh Script
You can regenerate both the unified Excel file and update the core data source by using any of the following methods:

- **Option A (One-click Windows Execution)**: 
  Double-click **`Refresh Portfolio.bat`** in the workspace.
- **Option B (Python Command Line)**:
  Open a terminal inside the project directory and run:
  ```powershell
  python refresh_portfolio.py
  ```

Once complete, your master Excel portfolio is immediately regenerated, formatted, and ready for distribution!

---

## 📋 Requirements & Dependencies

To run the Python automation scripts locally, ensure the following tools and packages are installed:

- **Python**: Version 3.8 or higher.
- **Packages**:
  ```bash
  pip install pandas openpyxl
  ```
