Turmerik Project

Overview:
Turmerik is a project designed to manage patient data and assess eligibility for clinical trials based on patient characteristics such as age and medical conditions.

Requirements:
- Python 3.x
- Pandas library
- Jupyter Notebook (optional, for interactive use)

Setup Instructions:

1. Clone the Repository:
   Open your terminal or command prompt and run:
   git clone <repository-url>
   cd <repository-folder>

2. Prepare Data Files:
   Place the following CSV files in the project directory:
   - patients.csv: Patient details including ID, birthdate, and gender.
   - conditions.csv: Conditions associated with each patient.
   - medications.csv: Medications prescribed to patients.
   - observations.csv: Lab results for each patient.
   - trials.csv: Information about clinical trials.

   Example Structure:
   - patients.csv:
     Id,BIRTHDATE,GENDER
     1,1990-01-01,M
     2,1985-05-05,F

   - conditions.csv:
     PATIENT,DESCRIPTION
     1,Diabetes
     2,Hypertension

3. Run the Jupyter Notebook:
   Launch Jupyter Notebook:
   jupyter notebook
   Open the `Turmerik.ipynb` file from the Jupyter interface.

Usage Instructions:

1. Load Data: The notebook will load the CSV files for processing.
2. Calculate Ages: Ages will be calculated based on birthdates.
3. Check Eligibility: The notebook checks which patients are eligible for trials based on age and conditions.
4. Save Results: Outputs are saved as:
   - eligible_trials.json: A JSON file listing eligible trials for each patient.
   - eligible_trials.xlsx: An Excel file with the same data.
