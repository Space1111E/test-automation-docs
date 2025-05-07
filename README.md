# 🐞 Bug Reports Generator

A simple and helpful tool that turns bug reports written in Excel into a professional Word document using Python.

Ideal for **manual QA testers** who want to generate clean, readable bug reports quickly!

---

## ✨ What Does It Do?

- ✅ Reads bug report data from an Excel file (`bug_reports.xlsx`)
- 📄 Converts each bug into a nicely formatted Word document
- 🖼️ Adds screenshots if a file path is included
- 💾 Saves everything in `Generated_Bug_Reports.docx`

---

## 🧰 What You Need

- Python 3.x  
- Packages:
  - `pandas`
  - `python-docx`
  - `openpyxl`

Install them by running:

```bash
pip install pandas python-docx openpyxl

```

## 📥 Excel Format
Your Excel file should include these columns:

- Bug_ID
- Title
- Environment
- Steps_to_Reproduce
- Actual_Result
- Expected_Result
- Severity
- Priority
- Status
- Screenshot_Path (optional)

✅ Example row:

| Bug\_ID | Title         | Severity | Steps\_to\_Reproduce                                                 | Actual\_Result         | Expected\_Result   |
| :------ | :------------ | :------- | :------------------------------------------------------------------- | :--------------------- | :----------------- |
| BUG001  | Login failure | High     | 1. Go to login page <br> 2. Enter wrong password <br> 3. Click login | Redirects to dashboard | Show error message |

---
## ▶️ How to Run

1. Save your Excel file as bug_reports.xlsx
2. Place it in the same folder as generate_bug_reports.py
3. Run the script:
```bash
python generate_bug_reports.py
```
4. Open your generated Word report:
   📄 Generated_Bug_Reports.docx

   ---
   
## 🔍 Key Features
- **Excel Integration:** Automatically reads bug and test case data from an Excel file.
- **Word Document Generation:** Converts data into a structured and easy-to-read Word document.
- **Customizable:** You can modify the script to suit your testing needs, adding or removing fields as required.
- **Screenshot Integration:** Optionally includes paths to screenshots in the reports.
- **Test Case Documentation:** Allows you to document the entire testing process with detailed steps and expected outcomes.

## 🎯 Future Improvements
- **📧 Automated Email Integration:** Send the generated reports via email.
- **✅ Validation:** Add data validation for bug report fields to ensure consistency.
- **🌐 Web Interface:** Develop a simple web interface for users to upload Excel files and download the generated reports.



