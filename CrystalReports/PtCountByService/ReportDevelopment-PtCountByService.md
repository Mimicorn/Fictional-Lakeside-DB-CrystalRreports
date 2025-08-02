# Encounter Information By Patient Service Report Development
## Data Source 
### Diagnosis_Intervention_View
The data source for this report is from <b>Diagnosis_Intervention_View</b> view in the Database <b>LakesideInpatient</b>. 
![Data Source](images/DatabaseExpert.png)
## Report Design Panel
![Report Design Panel](images/DesignPanel.png)
## Field Explorer
![Field Explorer](images/FieldExplorer.png)
## Patient Name Formula Field
Create a formula field PtName combining the first name and the last name of the patient. Add PtName to the report body as Patient Name field.
![Formula Field Patient Name](images/FormulaField_PatientName.png)
## Diagnosis Formula Field
Create a formula field Diagnosis combining the diagnosis code and its corresponding description. Add Diagnosis to the report body as Diagnosis field.
![Formula Field Diagnosis](images/FormulaField_Diagnosis.png)
## Procedure Formula Field
Create a formula field Procedure combining the procedure code and its corresponding description. Add Procedure to the report body as Procedure field.
![Formula Field Procedure](images/FormulaField_Procedure.png)
## Patient Service Parameter
Create a patient service parameter ParaService for user to filter specific services 

## Discharge Date Parameter
