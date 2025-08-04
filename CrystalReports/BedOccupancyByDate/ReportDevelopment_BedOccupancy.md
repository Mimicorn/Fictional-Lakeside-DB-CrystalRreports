# Inpatient Bed Occupancy Report Development
## Data Source
The data for this report is retrieved from the view <b>OccupancyDetailView</b> in the database <b>LakesideInpatient</b>. Please refer to <a href='../../'>database</a> directory for the detail of the view.
<br><br>
![Data Source](images/DatabaseExpert.png)
## Design Panel
![Design Panel](images/DesignPanel.png)
## Field Explorer
![Field Explorer](images/FieldExplorer.png)
## Formula Field BedFee
Create a Formula Field BedFee to calculate the cost of bed occupancy for the admission. 
<br><br>
![Formula Field BedFee](images/FormulaField_BedFee.png)
## Parameter Date
Create a parameter Date from the column OperationDate in the view for user to select the range of the date.
<br><br>
![Parameter Date](images/Parameter_ParaDate.png)
## Record Selection
Write script for the Record Selection Formula inside Selection Formulas in Formula Workshop with the parameter field, ParaDate, to display only the records based on the dates that user selects. 
<br><br>
![Record Selection Formula](images/RecordSelection.png)
## Group Expert
This report is grouped by the column OperationDate in the OccupancyDetailView view as shown in Group Expert.
<br><br>
![Group Expert](images/GroupExpert.png)<br><br>
![Group Expert Common](images/GroupExpert_Common.png)
<br>Check the box "Repeat Group Header On Each Page" in Group Expert Options to display group header on each page.
<br><br>![Group Expert Options](images/GroupExpert_Options.png)
## Group Summary
### Design Overview
![Group Summary Design](images/GroupSummary_Design.png)
Under the menu Insert, select Summary to insert the total occupied beds per date as follows
<br><br>
![Group Summary Bed Count](images/GroupSummary_Count.png)<br><br>
Select Summary to insert the total bed fee per date as follows
<br><br>
![Group Summary Bed Fee](images/GroupSummary_Sum.png)<br><br>
Create a Formula Field OccupancyRateByDate to calculate the bed occupancy rate per date and insert it to the Group Footer
<br><br>
![Formula Field OccupancyRateByDate](images/FormulaField_OccupancyRateByDate.png)
## Report Summary
