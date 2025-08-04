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
### Group Footer Design Overview
![Group Summary Design](images/GroupSummary_Design.png)<br><br>
### Under the menu Insert, select Summary to insert the total occupied beds per date to the Group Footer as follows
![Group Summary Bed Count](images/GroupSummary_Count.png)<br><br>
### Select Summary to insert the total bed fee per date to the Group Footer as follows
![Group Summary Bed Fee](images/GroupSummary_Sum.png)<br><br>
### Create a Formula Field OccupancyRateByDate, write code to calculate the bed occupancy rate per date, and insert it to the Group Footer
![Formula Field OccupancyRateByDate](images/FormulaField_OccupancyRateByDate.png)
## Report Summary
### Report Footer Design Overview
![Report Summary Design](images/ReportSummary_Design.png)<br>
### Create a Formula Field DateRange, write script to visualize the date range user selected and insert it to the Report Footer
![Formula Field DateRange](images/FormulaField_DateRange.png)<br><br>
### Under the menu Insert, Select Summary to insert the sum of bed fee for the date period user selected to the Report Footer as follows
![Group Summary Bed Fee](images/ReportSummary_Sum.png)<br><br>
### Create a RunningTotal Field RTotalOccupiedBedCount to calculate the sum of occupied bed for the period selected and to be referred in the Formula Field PeriodicOccupancyRate script
![Running Total Occupied Bed Count(images/RunningTotal_OccupiedBedCount.png)]<br><br>
### Create a Formula Field PeriodicOccupancyRate, write code to calculate the bed occupancy rate for the peirod user selected, and insert it to the Report Footer
![Formula Field Periodic Occupancy Rate](images/FormulaField_PeriodicOccupancyRate.png)
