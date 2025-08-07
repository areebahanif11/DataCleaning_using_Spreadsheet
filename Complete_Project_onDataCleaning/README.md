# Excel Data Cleaning Project: Customer Sales Data

This repository documents a data cleaning project performed in Microsoft Excel. The goal was to take a raw, messy customer sales dataset and transform it into a clean, reliable, and analysis-ready format. This process is a fundamental first step in any data analysis workflow, ensuring that insights are accurate and trustworthy.

## Project Overview

The raw dataset contained several common data quality issues, including:
*   Duplicate records
*   Inconsistent and ambiguous column headers
*   Leading/trailing white spaces
*   Inconsistent text casing and formatting
*   Mixed data types within a single column
*   Inconsistent categorical data (e.g., 'F' and 'Female' for the same category)
*   Typographical errors
*   Inconsistent date formats
*   Missing values (blanks)

This README outlines the step-by-step methodology used to identify and rectify these issues.

## Data Cleaning Steps

The entire cleaning process was performed using built-in Excel tools and functions. The key steps are detailed below.

### 1. Initial Setup: Preserving the Original Data

The first and most critical step is to never work directly on the raw data. This preserves the original file as a source of truth.

*   **Action:** Duplicated the original "Raw Data" worksheet.
*   **Method:** Right-clicked the worksheet tab, selected "Move or Copy," and checked the "Create a copy" option.
*   **Outcome:** A new worksheet was created, which was renamed to "Cleaned Data." All subsequent cleaning operations were performed on this new sheet.

### 2. Removing Duplicate Records

To ensure each record was unique, full-row duplicates were identified and removed.

*   **Action:** Removed duplicate rows from the dataset.
*   **Tool Used:** Excel's **Remove Duplicates** feature.
*   **Process:**
    1.  Selected the entire dataset.
    2.  Navigated to `Data > Data Tools > Remove Duplicates`.
    3.  Ensured all columns were selected to check for duplicates across the entire record.
*   **Result:** 18 duplicate rows were found and removed, leaving only unique records.

### 3. Standardizing Column Headers

Column headers were made clear, descriptive, and consistent for better readability and usability.

*   **Action:** Manually renamed the following headers:
    *   `cust` was changed to `Customer_ID`
    *   `marital stat` was changed to `Marital Status`
    *   `Pur Date` was changed to `Purchase_Date`
    *   `Amt` was changed to `Amount`

### 4. Cleaning Text and Categorical Data

Several columns required cleaning to standardize formats, correct typos, and remove inconsistencies.

*   **Customer ID & Customer Name (Extra Spaces & Casing):**
    *   **Issue:** Inconsistent spacing and capitalization (e.g., lowercase, UPPERCASE, and Proper Case all present).
    *   **Functions Used:** A nested `PROPER(TRIM())` formula was applied in a helper column.
        *   `TRIM()` removed all leading and trailing spaces.
        *   `PROPER()` converted the text to Proper Case (capitalizing the first letter of each word).
    *   **Process:** The cleaned data from the helper column was copied and pasted as **values** over the original column.

*   **Age (Mixed Data Types):**
    *   **Issue:** The column contained both numerical values and text (e.g., "twenty").
    *   **Tool Used:** **Find and Replace** (`Ctrl + H`).
    *   **Process:** Found all instances of "twenty" and replaced them with the numerical value "20".

*   **Gender & Marital Status (Inconsistent Categories & Typos):**
    *   **Issue:** Inconsistent abbreviations ('F', 'M') and typos ('Marrd', 'Sungle').
    *   **Tool Used:** **Find and Replace** (`Ctrl + H`) with the "Match entire cell contents" option enabled.
    *   **Process:**
        *   Replaced all instances of "F" with "Female".
        *   Replaced all instances of "M" with "Male".
        *   Corrected "Marrd" to "Married".
        *   Corrected "Sungle" to "Single".

### 5. Standardizing Date Formats

The `Purchase_Date` column had multiple formats (e.g., `DD-MM-YYYY`, `MM/DD/YYYY`).

*   **Action:** Converted all date entries into a single, consistent format.
*   **Tool Used:** **Text to Columns** feature.
*   **Process:**
    1.  Selected the `Purchase_Date` column.
    2.  Navigated to `Data > Text to Columns`.
    3.  In the wizard's third step, selected "Date" and specified the `DMY` (Day-Month-Year) format to correctly interpret all variations.
    4.  After conversion, the column was formatted as a "Short Date" for uniformity.

### 6. Handling Missing Values

Blank cells were present across multiple columns (`Age`, `Amount`, `Location`).

*   **Action:** Identified and filled all blank cells.
*   **Tool Used:** **Go To Special** feature (`Ctrl + G` > `Special`).
*   **Process:**
    1.  Selected the entire data range.
    2.  Opened the "Go To Special" dialog and selected "Blanks." This highlighted all empty cells.
    3.  Typed "N/A" and pressed `Ctrl + Enter` to fill all selected blank cells simultaneously. This is preferable to leaving them empty, as it explicitly marks the data as "Not Available."

## Final Result

The final "Cleaned Data" sheet is now a well-structured, consistent, and reliable dataset, ready for further analysis, visualization, or modeling. This cleaning process has eliminated potential errors and ensures that any conclusions drawn from this data will be based on accurate information.
