# 🧹 Data Cleaning Project in Google Sheets & Excel

This project documents the step-by-step process I used to clean and prepare raw data for analysis and visualization using **Google Sheets** and **Microsoft Excel**.

The steps cover removing blanks, transposing data, trimming spaces, changing text case, and clearing formatting to make data clean and analysis-ready.

---

## 📌 Steps Followed

### ✅ Step 1: Remove blank cells and rows
- Select all relevant columns (e.g., Columns A–H).
- Go to **Data → Create a filter**.
- For each column:
  - Click the filter icon → **Filter by condition → Is empty**.
  - Review and select the filtered blank rows.
  - Right-click → **Delete rows**.
- Repeat for each column to remove all rows with blank cells.

---

### 🔄 Step 2: Transpose the data
- Copy the data (including headers).
- Right-click on the destination cell (e.g., I1).
- Select **Paste special → Transposed**.
- Delete the original columns (e.g., Columns A–H).

---

### ✂️ Step 3: Trim extra spaces
- Select the cleaned dataset.
- Go to **Data → Data cleanup → Trim whitespace**.
- *In Excel*: use `=TRIM(A1)` formula and drag to apply.

---

### 🔠 Step 4: Change text case
**Google Sheets:**
- Install the **ChangeCase** add-on.
- Select the column you want to change.
- Go to **Add-ons → ChangeCase → All uppercase** (or other case options).

**Excel:**
- Use formulas like `=UPPER()`, `=LOWER()`, or `=PROPER()` to change case.

---

### 🧽 Step 5: Clear formatting
- Select the cleaned data.
- Go to **Format → Clear formatting**.
- *In Excel*: Home → Clear → Clear Formats.

---

## 📊 Result
✅ Blank rows removed  
✅ Data converted to wide format  
✅ Extra spaces trimmed  
✅ Text case standardized  
✅ Formatting cleared  

Data is now clean and ready for analysis!

---

## 🛠️ Tools Used
- Google Sheets
- Microsoft Excel

---

## ✏️ Notes
These steps are helpful for cleaning messy tabular data and can be reused for similar projects.

---
