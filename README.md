# SGPA Calculator

A modern Streamlit web app to calculate Semester Grade Point Average (SGPA) according to the official university formula. Upload your subject list as an Excel file, enter your marks, and instantly see your SGPA. Beautiful, interactive, and easy to use!

---

## Features

- **Excel Upload:** Upload your subjects with their respective codes, credits, and types.
- **Interactive Inputs:** Enter marks for Internal, Practical, and End Semester exams.
- **Accurate Calculation:** Uses the official SGPA formula, with weighted credits.
- **Sample Download:** Demo Excel file provided for quick setup.
- **Modern UI:** Custom styling for a sleek, dark-themed experience.
- **Explanation Included:** Built-in guide explaining SGPA and the calculation steps.
- **Error Handling:** Friendly messages for invalid files, missing data, or incorrect marks.
- **Animated Results:** Celebrate your achievement with balloons and a clear SGPA display.
- **Made by Mohit Kumar**

---

## Getting Started

### 1. Requirements

- Python 3.7 or higher
- [Streamlit](https://streamlit.io/)
- [pandas](https://pandas.pydata.org/)
- [openpyxl](https://openpyxl.readthedocs.io/en/stable/)

Install via pip:

```bash
pip install streamlit pandas openpyxl
```

### 2. Prepare Your Subject List

Create an Excel file (`.xlsx`) with the following columns:

| Code   | Credit | Type   |
|--------|--------|--------|
| CS101  | 4      | Theory |
| MA102  | 3      | Theory |
| PH103  | 3      | Theory |
| MCQ201 | 2      | MCQ   |

Only “Theory” and “MCQ” types are supported.

You can download a sample Excel file via the app.

### 3. Run the App

Save the code as `app.py` and run:

```bash
streamlit run app.py
```

Then open [http://localhost:8501](http://localhost:8501) in your browser.

---

## How It Works

1. **Upload Excel:** Choose your subject file with codes, credits, and types.
2. **Enter Marks:** For each subject, input your Internal, Practical, and End Semester marks.
3. **SGPA Calculation:**  
   - Grade Point (per subject):  
     `min(10, (Total Marks / Max Marks) × 10)`
   - Weighted by subject credit.
   - SGPA:  
     `SGPA = ∑(grade_point × credit) / ∑credits`
4. **Result:** Your SGPA is displayed and celebrated!

---

## Screenshots

*(Replace with real screenshots if desired)*

- Upload page with sample download
- Marks entry table
- SGPA result balloon animation

---

## Customization

- **Max Marks:** Default is 100 for all subjects, change in code if your scheme differs.
- **Subject Types:** Only Theory and MCQ supported. Extend by modifying `load_subjects_from_excel()`.

---

## Troubleshooting

- **Excel File Issues:** Ensure columns are named exactly as `Code`, `Credit`, `Type`.
- **Valid Types:** Only rows with `Theory` or `MCQ` are processed.
- **Marks Input:** Negative marks or missing credits will trigger errors.

---

## Credits

Made by Mohit Kumar

---

## License

MIT License (add your license here if you wish)

---

## Contact

For feedback and improvements: Contact : @Mohitkumar2007
