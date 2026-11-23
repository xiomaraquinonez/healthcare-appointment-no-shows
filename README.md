# Healthcare Appointment No-Show Analysis

An exploratory data analysis project investigating factors associated with medical appointment no-shows using Python, SQL, and Tableau.

## Project Overview

This project analyzes approximately 110,500 medical appointment records to identify patterns associated with missed appointments. The analysis explores how appointment lead time, patient age, SMS reminders, weekday, and neighborhood relate to appointment attendance.

The goal is to identify patterns that could help healthcare organizations better understand appointment attendance and inform future patient engagement strategies.

## Tools & Technologies

- **Python:** pandas, matplotlib
- **SQL:** SQLite
- **Data Visualization:** Tableau
- **Environment:** Jupyter Notebook

## Key Questions

- How does the time between scheduling and an appointment relate to no-show rates?
- Do no-show rates vary across patient age groups?
- How do no-show rates differ between patients who received SMS reminders and those who did not?
- Does the relationship between SMS reminders and no-show rates vary by appointment lead time?
- Are there differences in no-show rates across weekdays and neighborhoods?

## Key Findings

- **Appointment lead time:** No-show rates increased substantially with longer scheduling lead times, from 4.65% for same-day appointments to 33.00% for appointments scheduled 31–179 days in advance.
- **Age groups:** Young adults (18–34) had the highest no-show rate at 23.97%, while older adults (55–74) had the lowest at 15.70%.
- **SMS reminders:** Patients who received SMS reminders had a higher overall no-show rate. However, when comparing appointments within the same lead-time groups, SMS recipients had lower no-show rates for short-, medium-, and long-lead-time appointments.
- **Weekdays:** No-show rates varied relatively little across weekdays. Saturday had a higher rate, but the number of Saturday appointments was small.
- **Neighborhoods:** No-show rates varied across the ten neighborhoods with the highest appointment volumes.

## Project Files

| File | Description |
|---|---|
| `Healthcare_Appointment_No_Show_Analysis.ipynb` | Python data cleaning, exploratory analysis, visualizations, and SQL queries |
| `appointments.db` | SQLite database used for SQL analysis |
| `appointments_tableau.csv` | Cleaned dataset prepared for Tableau |
| `Medical_Appointment_No_Shows.twbx` | Packaged Tableau dashboard workbook |

## Dataset

The dataset is the Medical Appointment No Shows dataset from Kaggle:
[Medical Appointment No Shows – Kaggle](https://www.kaggle.com/datasets/joniarroba/noshowappointments)

The original dataset is not included in this repository. To run the notebook, download `KaggleV2-May-2016.csv` from Kaggle and place it in the same directory as the notebook.

## Methodology

1. Cleaned and prepared appointment records, including handling inconsistent dates and invalid age values.
2. Conducted exploratory data analysis using Python and pandas.
3. Used SQL queries and aggregations to investigate attendance patterns across different factors.
4. Created visualizations in Python and developed an interactive Tableau dashboard.
5. Summarized findings and developed recommendations for further investigation.

## Limitations

This analysis uses observational data and identifies associations rather than causal relationships. In particular, the SMS data does not indicate when reminders were sent, whether they were read, or why certain patients received reminders. Additional patient and appointment context would be needed to explain the observed patterns.

## Conclusion

Appointment lead time showed the largest differences in no-show rates among the factors examined. Age, SMS receipt, and neighborhood also revealed differences in attendance patterns, while weekday differences were relatively small. These findings highlight areas for further investigation
