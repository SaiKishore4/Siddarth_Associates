# Analysis Code Bundle

Files:
- analysis.py    : Python script (pandas) to parse Excel, create cleaned data and summary sheets.
- analysis.sql   : SQLite-compatible schema and queries for yearwise/hsn/model analysis.
- README.md      : This instructions file.

How to use (Python):
1. Ensure Python 3.8+ is installed.
2. Install required packages:
   pip install pandas openpyxl xlsxwriter
3. Place `Sample Data 2.xlsx` in the same folder as analysis.py.
4. Run:
   python analysis.py
5. Output: analysis_output.xlsx (contains Raw Data, Cleaned Data, and summary sheets).

How to use (SQLite / SQL):
- Load your data into the `imports` table (e.g., via CSV import or programmatically).
- Run the queries in analysis.sql to get the requested summaries.

How to zip:
- Windows:
  * Select files, right-click -> Send to -> Compressed (zipped) folder.
- macOS:
  * Select files, right-click -> Compress items.
- Linux:
  * From the folder containing the files:
    zip analysis_code_bundle.zip analysis.py analysis.sql README.md
