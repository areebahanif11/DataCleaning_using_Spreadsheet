# 📊 Data Cleaning Project – Using Pivot Tables, VLOOKUP & Plotting

This project documents how I cleaned and explored data from the **Cosmetics Inc.** dataset using Google Sheets tools like:
- Pivot tables
- VLOOKUP
- Plotting & charts

These steps help view the data from different perspectives, identify outliers, and enrich data by connecting multiple sheets.

---

## 📌 Step-by-Step: Different Data Perspectives

### ✅ Example 1: Pivot Tables
Pivot tables help summarize and reorganize data easily.

- Selected the entire dataset in **Sheet 1** (A1:F31).
- Went to **Insert → Pivot Table → New sheet → Create**.
- In the Pivot Table editor:
  - Added **Total** to Rows.
  - Sorted by **Descending** order (to see highest totals at the top).
  - Added **Products** below Rows.
- Result: identified top two most profitable products:
  - `15143Exfo`
  - `32729Masc`

---

### 🔍 Example 2: VLOOKUP
VLOOKUP brings information from another sheet.

- Switched back to **Sheet 1**.
- In cell `H2`, used:
# 📊 Data Cleaning Project – Using Pivot Tables, VLOOKUP & Plotting

This project documents how I cleaned and explored data from the **Cosmetics Inc.** dataset using Google Sheets tools like:
- Pivot tables
- VLOOKUP
- Plotting & charts

These steps help view the data from different perspectives, identify outliers, and enrich data by connecting multiple sheets.

---

## 📌 Step-by-Step: Different Data Perspectives

### ✅ Example 1: Pivot Tables
Pivot tables help summarize and reorganize data easily.

- Selected the entire dataset in **Sheet 1** (A1:F31).
- Went to **Insert → Pivot Table → New sheet → Create**.
- In the Pivot Table editor:
  - Added **Total** to Rows.
  - Sorted by **Descending** order (to see highest totals at the top).
  - Added **Products** below Rows.
- Result: identified top two most profitable products:
  - `15143Exfo`
  - `32729Masc`

---

### 🔍 Example 2: VLOOKUP
VLOOKUP brings information from another sheet.

- Switched back to **Sheet 1**.
- In cell `H2`, used:
# 📊 Data Cleaning Project – Using Pivot Tables, VLOOKUP & Plotting

This project documents how I cleaned and explored data from the **Cosmetics Inc.** dataset using Google Sheets tools like:
- Pivot tables
- VLOOKUP
- Plotting & charts

These steps help view the data from different perspectives, identify outliers, and enrich data by connecting multiple sheets.

---

## 📌 Step-by-Step: Different Data Perspectives

### ✅ Example 1: Pivot Tables
Pivot tables help summarize and reorganize data easily.

- Selected the entire dataset in **Sheet 1** (A1:F31).
- Went to **Insert → Pivot Table → New sheet → Create**.
- In the Pivot Table editor:
  - Added **Total** to Rows.
  - Sorted by **Descending** order (to see highest totals at the top).
  - Added **Products** below Rows.
- Result: identified top two most profitable products:
  - `15143Exfo`
  - `32729Masc`

---

### 🔍 Example 2: VLOOKUP
VLOOKUP brings information from another sheet.

- Switched back to **Sheet 1**.
- In cell `H2`, used:
- =VLOOKUP(A2, 'Sheet 2'!A1:B31, 2, false)
- Looks up the product code from A2 in `Sheet 2` (columns A–B).
- Returns the product name if found.
- Dragged the fill handle to apply the formula to other rows.

---

### 📈 Example 3: Plotting
Plotting helps quickly spot outliers.

- Selected column **B** (prices).
- Went to **Insert → Chart**.
- In Chart Editor, selected **Column chart**.
- Noticed an obvious outlier: price `$0.73` in cell `B14`.
- Corrected it to `$7.30`.
- Chart updated automatically to reflect the correction.

---

## 🚀 Result
By applying these steps:
✅ Identified and corrected outliers  
✅ Enriched data with product names  
✅ Visualized sales distribution and focused on most profitable products

The dataset became cleaner, better structured, and ready for further analysis.

---

## 🛠 Tools Used
- Google Sheets built-in features:
- Pivot tables
- VLOOKUP
- Find & Replace
- Chart plotting

---

