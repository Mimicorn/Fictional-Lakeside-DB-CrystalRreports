# Length of Stay By Patient Service Report Development
## Data Source
The data of this report is derived from the view <b>EncounterView</b> in the database <b>LakesideInpatient</b>.
<br><br>![Data Source](images/DatabaseExpert.png)
## Report Design Panel 
![Report Design Panel](images/DesignPanel.png)
## Field Explorer
![Field Explorer](images/FieldExplorer.png)
## Formula Field Name
Create a formula field Name combining the first name and the last name of the patient. Add Name to the report body as Patient Name field.
<br><br>![Formula Field Name](images/FormulaField_Name.png)
## Patient Service Parameter
Create a patient service parameter ParaService for user to filter specific services 
<br><br>![Parameter Patient Service](images/Parameter_ParaService.png)
## Record Selection Formula
Write script for the Record Selection Formula inside Selection Formulas in Formula Workshop with the parameter field, ParaService, to display only the records based on the patient services that user selects. 
<br><br>![Record Selection Formula](images/RecordSelection.png)
## Group Expert
This report is grouped by the column Serv_name (patient service name) in the EncounterView view as shown in Group Expert.
<br><br>![Group Expert](images/GroupExpert.png)
## Group Summary
Under the menu Insert select Summary to insert the average and the sum of LOS for each patient service as shown below to the Group Footer section.
<br><br>![Group Summary](images/GroupSummary_Avg.png)
<br><br>![Group Summary](images/GroupSummary_Sum.png)
## Report Summary
Under the menu Insert select Summary to insert the average and the sum of LOS for all patient services as shown below to the Report Footer section.
<br><br>![Report Summary](images/ReportSummary_Avg.png)
<br><br>![Report Summary](images/ReportSummary_Sum.png)
