Hospital Dashboard

Overview
This Power BI Hospital Dashboard provides insights into patient management, appointments, revenue, treatment costs, and departmental performance. It helps hospital management monitor operational and financial metrics through interactive visualizations.

Key KPIs
The dashboard uses DAX measures to calculate the following KPIs:
1.Total Patients = COUNT(Patients[PatientID])
2.Total Appointments = COUNT(Appointments[AppointmentID])
3.Completed Revenue =
CALCULATE(
    SUM(Appointments[TreatmentCost]),
    Appointments[Status] = "Completed"
)
4.Average Treatment Cost =
AVERAGE(Appointments[TreatmentCost])
KPI Results
Total Patients: 192
Total Appointments: 600
Completed Revenue: 2M
Average Treatment Cost: 10.17K

Visualizations
Total Patients by Department – Department-wise patient distribution.
Total Appointments by Department – Appointment analysis across departments.
Completed Revenue by Month – Monthly revenue trend.
Completed Revenue by Doctor – Doctor-wise revenue contribution.
Total Patients by Gender – Gender distribution of patients.
Department Slicer – Interactive filtering for detailed analysis.

Tools Used
Power BI Desktop
Power Query
DAX
Data Modeling

Insights
Cardiology has the highest patient volume and appointments.
Revenue trends vary across months.
Doctor-wise revenue analysis highlights top contributors.
Patient gender distribution is nearly balanced.

Project: Healthcare Analytics Dashboard
Tool: Power BI Desktop
Domain: Healthcare Analytics
