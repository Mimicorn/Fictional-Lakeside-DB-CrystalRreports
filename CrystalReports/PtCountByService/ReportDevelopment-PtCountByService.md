# Encounter Information By Patient Service Report Development
## Data Source 
### Diagnosis_Intervention_View
The data source for this report is from <b>Diagnosis_Intervention_View</b> view in the Database <b>LakesideInpatient</b>. Please refer to <a href='../../'>database</a> directory for the detail of the view.
<br><br>![Data Source](images/DatabaseExpert.png)
## Report Design Panel
![Report Design Panel](images/DesignPanel.png)
## Field Explorer
![Field Explorer](images/FieldExplorer.png)
## Patient Name Formula Field
Create a formula field PtName combining the first name and the last name of the patient. Add PtName to the report body as Patient Name field.
<br><br>![Formula Field Patient Name](images/FormulaField_PatientName.png)
## Diagnosis Formula Field
Create a formula field Diagnosis combining the diagnosis code and its corresponding description. Add Diagnosis to the report body as Diagnosis field.
<br><br>![Formula Field Diagnosis](images/FormulaField_Diagnosis.png)
## Procedure Formula Field
Create a formula field Procedure combining the procedure code and its corresponding description. Add Procedure to the report body as Procedure field.
<br><br>![Formula Field Procedure](images/FormulaField_Procedure.png)
## Patient Service Parameter
Create a patient service parameter ParaService for user to filter specific services 
<br><br>![Parameter Patient Service](images/Parameter_Service.png)
## Discharge Date Parameter
Create a discharge date parameter ParaDcDate for user to choose discharge dates
<br><br>![Parameter Discharge Date](images/Parameter_DischargeDate.png)
## Record Selection Formula
Write script for the Record Selection Formula inside Selection Formulas in Formula Workshop with the parameter fields, ParaService and ParaDcDate, to display only the records based on the patient services and the discharge dates that user selects. 
<br><br>![Record Selection Formula](images/RecordSelection.png)
## Discharge Date Start Formula Field
Create a formula field DdateFromSelected to get the value of discharge start date selected by user and insert it to the report page header and report footer
<br><br>![Discharge Start Date](images/FormulaField_DischargeDateFrom.png)
## Discharge Date End Formula Field
Create a formula field DdateToSelected to get the value of discharge end date selected by user and insert it to the report page header amd report footer.
<br><br>![Discharge End Date](images/FormulaField_DischargeDateTo.png)
## Suppress Duplicate Field Value
Under Format menu, choose Format Field to hide the duplicate field values for the same patient encounter in Format Editor by checking on Suppress If Duplicated option in Common tab. 
<br><br>![Suppress Duplicate Field Value](images/FieldFormatEditor.png)
## Suppress Line in Detail
Choose the line in Detail section, right click on Format Line. Check on Suppress box In Format Line Editor and click on the square icon beside it to open the Formula Workshop for the current formula.
<br><br>![Line Detail Form Editor](images/LineDetails_FormatEditor.png)<br>
Write code to hide the line in Detail section in between records for the same encounter.
<br><br>![Line Detail Form Editor Suppress](images/LineDetails_FormatEditor_Suppress.png)
## Suppress Line in Group Footer
Check on Suppress box in Format Line Editor for the line in Group Footer section, click on the square icon beside it to open the Formula Workshop, and write code to hide the line in Group Footer section if the current group is not the last group in the report. 
<br><br>![Line Group Footer Form Editor Suppress](images/LineGroupFooter_FormatEditor_Suppress.png)
## Next Group Formula Field
Create a formula field NextGroup to get the value of the next printing group in the report. It is referrenced in the above suppress the line in Group Footer formula.   
<br>![Next Group Formula Field](images/FormulaField_NextGroup.png)
## Group Expert
This report is grouped by the column Serv_name (patient service name) in the view as shown in Group Expert.
<br><br>![Group Expert](images/GroupExpert.png)
![Group Expert Common](images/GroupExpertCommon.png)
<br>Check the box "Repeat Group Header On Each Page" in Group Expert Options to display group header on each page.
<br><br>![Group Expert Options](images/GroupExpertOptions.png)
## Group Summary
Under the menu Insert select Summary to insert the count of encounters for each group as shown below to the Group Footer section.
<br><br>![Group Summary](images/GroupSummary.png)
## Report Summary
Under the menu Insert select Summary to insert the count of encounters for all groups as shown below to the Report Footer section.
<br><br>![Report Summary](images/ReportSummaryInsert.png)
