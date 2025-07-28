# 🧹 Data Cleaning Project in Google Sheets

This project demonstrates how to clean and prepare messy spreadsheet data using built-in **Google Sheets** tools and features.

The data used in this project is from the **International Logistics Association Memberships - Data for Cleaning** dataset.

---

## 📌 Step-by-Step Data Cleaning Process

### ✅ Example 1: Use Conditional Formatting to Highlight Blank Cells
- Open the dataset.
- Select columns **A–L**, except for columns **F** and **H**:
  - Click column A.
  - Hold `Shift` and click column E (selects A–E).
  - Hold `Control` (Windows) or `Command` (Mac) and click columns G, I, J, K, and L.
- Go to **Format → Conditional formatting**.
- In the **Format cells if** dropdown, select `Cell is empty`.
- Choose a bright color under **Formatting style** to highlight blank cells.
- Click **Done**.

This helps visually identify missing data quickly.

---

### 🗑 Example 2: Remove Duplicates
- Duplicate your sheet to keep the original data safe:
  - Right-click on the sheet tab → **Duplicate**.
- Work on the new sheet.
- Go to **Data → Data cleanup → Remove duplicates**.
- Check **Data has header row**.
- Click **Select All** to check all columns.
- Click **Remove duplicates**.

This ensures each record in your dataset is unique.

---

### 📅 Example 3: Format Dates Consistently
- Select column **J** (Membership valid through).
- Go to **Format → Number → Date**.

This makes all dates uniform and easier to work with in analysis.

---

### ✂️ Example 4: Split Text to Columns
- Select column **L** (Certification).
- Go to **Data → Split text to columns**.
- Google Sheets will auto-detect the delimiter (e.g., comma).  
- If needed, manually select the correct separator.

This separates combined data into individual columns for better clarity and analysis.

---

## 🚀 Result
By applying these steps:
- Blank cells are clearly highlighted.
- Duplicate records are removed.
- Dates are formatted consistently.
- Text data is separated into distinct columns.

The dataset is now **clean, structured, and ready for analysis**.

---

## 🛠 Tools Used
- Google Sheets built-in features:
  - Conditional formatting
  - Remove duplicates
  - Split text to columns
  - Format dates

---

