# My Ballot (Excel-based)

This Excel-based tool allows you to load candidates data for the 2025 Philippine national and local elections and choose them in My Ballot tab. The source data is from the [COMELEC Ballot Face Templates](https://comelec.gov.ph/?r=2025NLE/2025BallotFace) and converted into a structured JSON format. This tool enables you to preview candidates by position and fill out your personalized ballot.

## 📋 Features

- Compatible with **all Philippine legislative districts**
- Converts **official Comelec PDFs to structured JSON**
- Supports bilingual (English and Filipino) voting instructions
- Handles all positions from **Senator** to **City Councilor**
- Excel interface with refreshable **Power Query** integration
- Includes disclaimers and metadata for transparency

---

## 🛠️ How to Use

1. **Get the Ballot PDF:**
   - Visit the official Comelec [Ballot Face Templates](https://comelec.gov.ph/?r=2025NLE/2025BallotFace)
   - Go to your **legislative district** and download the relevant PDF(s)

2. **Convert PDF to JSON:**
   - Use generative AI or Python scripts to extract data from the PDF
   - Ensure the output format follows the strict JSON schema (sample prompt included in Excel file)
   - Validate that all candidates and bilingual instructions are preserved
   - ⚠️ *Watch out for lone candidates being skipped—verify JSON completeness manually or via code*

3. **Save JSON Files:**
   - Place all JSON outputs in a local folder of your choice

4. **Load JSON into Excel:**
   - Open the [Excel file](./My%20Election%20Ballot%20-%20v07.xlsx)
   - Go to the `Instructions and Lookup` tab
   - Set the JSON folder path in **cell C3**
   - Select **Data → Refresh All** to upload and update candidate data

5. **Select Your District:**
   - Still in the `Instructions and Lookup` tab, choose your district’s JSON file
   - Verify correctness by reviewing candidates from **Senator to Councilor**

6. **Fill Out Your Sample Ballot:**
   - Go to the `My Ballot` tab and select your preferred candidates

---
## 📁 Folder Structure

- **My Ballot/**
  - **[GenAI Prompt to convert PDF to JSON/](./GenAI%20Prompt%20to%20convert%20PDF%20to%20JSON)**  
    GenAI prompt you can use to convert from PDF to JSON format
  - **[JSON/](./JSON)**  
    Folder containing JSON files converted from selected 2025 Ballot Face Templates from the Comelec website
  - **[PDF/](./PDF)**  
    Folder containing selected downloaded 2025 Ballot Face Templates PDFs from the Comelec website
  - **[My Election Ballot - v07.xlsx](./My%20Election%20Ballot%20-%20v07.xlsx)**  
    Main Excel workbook
  - **LICENSE.txt**  
    License information
  - **README.md**  
    Project documentation

## License

This Excel workbook is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

You are free to use, modify, and share this file, as long as proper attribution is provided.

**Copyright © 2025 Washington Alto**

### Disclaimer

This file is provided "as-is" without any warranties. I am not liable for any issues or damages resulting from its use. Users assume full responsibility.
