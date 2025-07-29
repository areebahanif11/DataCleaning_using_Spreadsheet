# 🧹 Data Cleaning Project – Spreadsheet Functions & Formatting

This project documents the **step-by-step process** I used to clean and transform messy data using Google Sheets built-in functions and formatting tools.

The project uses two datasets:
- **International Logistics Association Memberships - Data for Cleaning**
- **Cosmetics Inc. - Data for Cleaning**

By applying spreadsheet functions, I optimized the data-cleaning process to make the data ready for analysis.

---

## 📌 Step-by-Step: Optimize the Data-Cleaning Process

### ✅ Example 1: Use the COUNTIF function
- Count how many members pay dues less than \$100:
  - Added label in `H74`: `Member Dues < 100`
  - Formula in `I74`: `=COUNTIF(I2:I72,"<100")`
- Count how many members pay dues greater than \$500:
  - Added label in `H75`: `Member Dues > 500`
  - Formula in `I75`: `=COUNTIF(I2:I72,">500")`

This helps quickly identify outliers or unusual values.

---

### 🔢 Example 2: Use the LEN function
- Inserted a new column named **LEN** to calculate the length of each Member ID:
  - Formula in `B2`: `=LEN(A2)`
- Dragged down to apply to all rows.

This helps check data consistency (e.g., all IDs should be the same length).

---

### 🎨 Example 3: Use Conditional Formatting
- Applied conditional formatting to column **B** to highlight cells where the value is **not equal to 6**.
- Helps visually spot invalid Member IDs (e.g., length ≠ 6).

---

### ⬅️➡️ Example 4: Use LEFT and RIGHT functions
**Dataset: Cosmetics Inc.**
- Extracted first 5 characters from `A2`:
  - In `H2`: `=LEFT(A2, 5)`
- Extracted last 4 characters from `A2`:
  - In `I2`: `=RIGHT(A2, 4)`

Used fill handle to apply formulas to the entire column.

---

### ✂️ Example 5: Use the MID function
- Extracted two-letter state code starting at character 4 in `D2`:
  - In `J2`: `=MID(D2, 4, 2)`

---

### 🔗 Example 6: Use the CONCATENATE function
- Combined values from columns H and I into a new column:
  - In `K2`: `=CONCATENATE(H2, I2)`

This joins text fields, useful for creating IDs or codes.

---

### ✂️ Example 7: Use the TRIM function
- Removed extra spaces from text data:
  - In `L2`: `=TRIM(C2)`

Ensures clean text data by eliminating unnecessary spaces.

---

## 🚀 Result
By applying these steps:
✅ Outliers are identified  
✅ Data formats are validated  
✅ Text fields are cleaned and standardized  
✅ New useful columns are created for analysis

The dataset is now cleaner, more reliable, and ready for further processing or visualization.

---

## 🛠 Tools Used
- Google Sheets built-in functions:
  - `COUNTIF`, `LEN`, `LEFT`, `RIGHT`, `MID`, `CONCATENATE`, `TRIM`
- Conditional formatting

---
