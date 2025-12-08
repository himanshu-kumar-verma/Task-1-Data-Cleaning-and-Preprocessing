# 🧹 Task-1-Data-Cleaning-and-Preprocessing

## **Medical Appointment Dataset Cleaning Summary**

## Data Cleaning Steps I Performed

## Date Cleaning:

- Cleaned **ScheduledDay** and **AppointmentDay** using Text to Columns.

- Removed time components and converted them into valid Date format.

- Ensured both columns could be grouped properly in pivot tables.

## Age Column Fix:

- Removed rows with **Age = -1** (invalid data).

- Kept **Age = 0** because it represents newborn babies.

## Column Name Corrections:

- Renamed incorrect column headers to correct spellings:

  - Hipertension → Hypertension

  - Handcap → Handicap

## Identifier Cleanup:

- Converted **PatientId** and **AppointmentID** to Text format to prevent digit loss and exponential notation.

- Ensured IDs remain unchanged and consistent.

## Validation of Binary Columns:

- Verified that the following columns contain clean 0/1 values:

  • Scholarship

  • Hypertension

  • Diabetes

  • Alcoholism

  • Handicap

  • SMS_received

  • No-show

- Ensured they remain numeric for accurate counting and averaging.

## Duplicate Removal:

- Applied Remove Duplicates across the entire dataset.

- Ensured only unique appointment records remain.

## Text Cleaning:

- Used the **TRIM** function to remove extra spaces in Neighbourhood and other text based columns.

## Final Output:

- Created a final cleaned sheet.
