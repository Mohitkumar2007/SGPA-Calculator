# SGPA Calculator 📊

A modern, easy-to-use web app for calculating **Semester Grade Point Average (SGPA)** using your subject list and marks. Built with [Streamlit](https://streamlit.io/) and supports Excel uploads, instant SGPA calculation, and downloadable results.

---

## 🚀 Features

- **Upload Subject List**: Upload your subjects as an Excel file (`.xlsx`) with columns: Code, Credit, Type (Theory/MCQ).
- **Enter Marks**: Input Internal, Practical, and End Semester marks for each subject.
- **Official Calculation Scheme**: SGPA is calculated as per university rules.
- **Download Results**: Download your marks and SGPA as an Excel or CSV file.
- **Sample File**: Download a sample Excel file to see the expected format.
- **Dark Theme UI**: Stylish, responsive, and easy to use!

---

## 📦 Installation

1. **Clone or Download** this repo and save the code as `sgpa_calculator.py`.

2. **Install dependencies**:

```bash
pip install streamlit pandas openpyxl
```

---

## 🏃‍♂️ How to Run

```bash
streamlit run sgpa_calculator.py
```
- Open the link shown in your terminal (usually [http://localhost:8501](http://localhost:8501)).

---

## 📋 How to Use

1. **Download the sample Excel file** from the app or create your own with the following columns:

   | Code   | Credit | Type   |
   |--------|--------|--------|
   | CS101  | 4      | Theory |
   | MA102  | 3      | Theory |
   | PH103  | 3      | Theory |
   | MCQ201 | 2      | MCQ   |

2. **Upload your Excel file** via the uploader.

3. **Enter your marks** for each subject in the provided fields.

4. **Click "Calculate SGPA"** to view your result (with confetti!).

5. **Download your marks and SGPA** as Excel or CSV for your records.

---

## ⚡ SGPA Formula

\[
\text{SGPA} = \frac{\sum (\text{Grade Point} \times \text{Credit})}{\sum \text{Credits}}
\]

Where:

- **Grade Point per subject** = min(10, (Total Marks / Maximum Marks) × 10)
- Weighted by subject credit.

---

## 📝 Notes

- Supported subject types: **Theory** and **MCQ**.
- Maximum marks per subject: 100 (internal + practical + end sem).
- If your university uses a different scheme, modify `max_marks` logic in the code.

---

## 🛠️ Customization

- Change colors, fonts, or logic in `sgpa_calculator.py` as desired.
- Extend for CGPA calculation or additional subject types.

---

## 👨‍💻 Author

Made by [Mohit Kumar](https://github.com/Mohitkumar2007)

---

## 📄 License

MIT License
