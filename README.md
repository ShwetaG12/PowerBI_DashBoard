# Amazon_Dashboard
Problem statement

This dashboard helps Amazon understand the Sales. It is Amazon Sales Analytics Dashboard where carefully analyzing the data and identifying key trends and patterns, can uncover valuable insights and address specific challenges to improve business performance.

Steps: 
1.Create an Excel formula to give values "Delay" if the difference of dates in cell C2 and B2 in days is greater than 4, otherwise the value should be "On time".

Solution:

Excel =IF(DAYS(C2,B2) > 4, "Delay", "On time") Use code with caution.

2.Extracting Name from Email ID
Prompt: Write an Excel formula to extract the name from an email ID in F2, with @ as a separator.

Solution:

Excel =IF(C2-B2 > 4, "Delay", "On time") Use code with caution.

3.Extracting Values from Comma-Separated String
Prompt: I have comma-separated values in G2. Write three Excel formulas to extract the values as comma separators in H2, I2, and J2.

Solutions:

Excel H2: ==LEFT(G2,FIND(",",G2)-1) I2: =MID(G2,FIND(",",G2)+1,FIND(",",G2,FIND(",",G2)+1)-FIND(",",G2)-1) J2: RIGHT(G2,LEN(G2)-FIND(",",G2,FIND(",",G2)+1))

These formulas use the LEFT, MID, and RIGHT functions to extract the first, second, and third values from the comma-separated string in G2, respectively.

Steps for Power BI Dashboard Using Above Data

1.Connect to Your Data Source:
Import your Excel data into Power BI using the "Get Data" option. Choose the appropriate data source (e.g., Excel workbook). Navigate to your Excel file and select the sheet containing the relevant data. Click "Load" to import the data into Power BI.

2.Create Calculated Columns:
In the Power BI Data View, create calculated columns using the formulas from Step 1 and Step 3.

3.Build Visualizations:
Drag and drop fields from your data model onto the canvas to create visualizations.

4.Customize and Format:
Customize the appearance of your visualizations by changing colors, labels, and formatting options. Add titles, legends, and tooltips to make your dashboard more informative and user-friendly.

5.Publish and Share:
Once satisfied with dashboard, publish it to the Power BI service or share it as a report.
