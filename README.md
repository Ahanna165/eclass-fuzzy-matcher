# 🧠 ECLASS Matching with RapidFuzz & Levenshtein

This project helps you **match ECLASS classification codes** between different catalog versions using **fuzzy string matching**. It is especially useful for product catalog managers, e-commerce and procurement engineers, or data specialists working with ECLASS, UNSPSC, or similar classification systems.

---

## 📌 What This Project Does

- Detects columns in Excel/CSV files that contain ECLASS codes and ECLASS descriptions (8-digit values, unique, text of certain length, name logic).
- Matches similar codes between different ECLASS versions.
- Uses fuzzy matching with [RapidFuzz](https://github.com/maxbachmann/RapidFuzz) (faster and better than traditional Levenshtein).
- Scores potential ECLASS columns using Levenstein distance logic.

---

## 📦 Requirements

    Python 3.7+

    pandas

    numpy

    rapidfuzz

    openpyxl

    xlsxwriter

    nltk
    
## 💡 Example Use Cases and ECLASS Version Files

You work with three Excel or CSV files:

1. **Your ECLASS list** – extracted from your product catalog or a sample file in the `/data/` folder.

2. **ECLASS full list – Old version**  
   Contains all official ECLASS codes from the same version used in your product file (e.g., **v5.1**).

3. **ECLASS full list – New version**  
   Contains all official ECLASS codes from the version you want to match to (e.g., **v5.1.4**).

👉 This script helps match codes from **version X** to **version Y**, even if they are slightly different in structure or naming.

## 👩‍💻 Author

Developed by **Hanna Baiker**, combining skills in **e-procurement**, **electronic catalogs**, and **data engineering with a focus on NLP**.

- 🌐 Website: https://ahanna165.github.io/
- 🔗 LinkedIn: Hanna-Baiker



