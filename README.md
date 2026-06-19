# Hospital Dashboard

## Overview
This Power BI Hospital Dashboard provides insights into patient management, appointments, revenue performance, treatment costs, and departmental analysis. The dashboard helps healthcare administrators monitor key operational and financial metrics through interactive visualizations.

## KPIs (DAX Measures)

```DAX
Total Patients = COUNT(Patients[PatientID])

Total Appointments = COUNT(Appointments[AppointmentID])

Completed Revenue =
CALCULATE(
    SUM(Appointments[TreatmentCost]),
    Appointments[Status] = "Completed"
)

Average Treatment Cost =
AVERAGE(Appointments[TreatmentCost])
```

### KPI Results
- Total Patients: 192
- Total Appointments: 600
- Completed Revenue: 2M
- Average Treatment Cost: 10.17K

## Dashboard Visualizations
- Total Patients by Department
- Total Appointments by Department
- Completed Revenue by Month
- Completed Revenue by Doctor Name
- Total Patients by Gender
- Department Slicer for interactive filtering

## Tools & Technologies
- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
- Data Modeling

## Key Insights
- Cardiology has the highest number of patients and appointments.
- Monthly revenue trends help identify peak and low-performing periods.
- Doctor-wise revenue analysis highlights top contributors.
- Gender distribution of patients is nearly balanced.
- Department-level filtering enables focused analysis.

## Project Information
**Project Name:** Hospital Dashboard  
**Domain:** Healthcare Analytics  
**Tool:** Power BI Desktop
