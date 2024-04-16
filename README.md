This dashboard helps Life Insurance Companies understand their business performance as well as provide insights into key metrics across various dimensions of the life insurance business. The dashboard covers four revenue sources, including overall FPI, micro-insurance business, foreign employment business and Endowment Business along with additional metrics such as TPI, Renewal, Monthly Trend Analysis and Surrender Analysis. In the dashboard the life insurance companies are also categorized into four generations based on their age.
This project aims to evaluate customer satisfaction by analyzing market share and identifying any weaknesses within various categories of the life insurance business.
Steps followed
-	Step 1: Monthly insurance statistics were downloaded from the central insurance authority's official website.
-	Step 2: Select the excel workbook from get data in the Home tab in power BI Desktop the excel file is imported into the PBIX file.
  

![Step 2](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/e3e8b51b-a330-45d9-b486-9e01e91d349a)

-	Step 3: The columns of the importable tables are double checked and incase there are any errors they are fixed through editing the query or updating the data in the SQL database.

![Step 3](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/8366de64-ae9b-4978-b57d-749038824dad)
•	Step 4: The homepage is designed using a combination of Shapes, texts and images.
•	Step 5: A bookmark navigator is added on the rectangular shape of the  homepage. The list is populated after the bookmarks are added.
![Step 5](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/17f370fb-7c4f-4196-9517-d552e0604898)  
•	Step 6: The plus sign Besides the home page is selected. This will add a new page.
•	Step 7: A square shape is inserted on the top of the page two slicers are placed for year and month. Also a bookmark navigator is inserted besides the slicers.
![Step 7](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/0529e186-9164-41c2-99cd-5d36e8fbb6fb)
•	Step 8: A matrix table is added and in the row pane of the matrix table the life insurance companies and generation is added.
![Step 8](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/eab93708-ffd4-45c4-aa25-f18ffde7155b)
•	Step 9: Dax measures were written for all the categories of life insurance i.e. Agency Business, Micro Insurance, Foreign Employment, Total Premium Income, Renewal, Surrender.
The Following Dax Measures were Used:

For current year calculations: 
sum (MKT_Data_Tot [FPI])
For previous year calculations: 
var Last_Date= LASTDATE (DimDate [DateValue])
var prev_fiscal_mon=calculate (max (DimDate [PreviousYearMonthNo]), FILTER (all(DimDate),DimDate[DateValue]=Last_Date))
var py_st_date=CALCULATE (MIN (DimDate [DateValue]), FILTER (all (DimDate),DimDate[Nepali Year Month Number]=prev_fiscal_mon))
var py_end_date=CALCULATE (Max (DimDate [DateValue]), FILTER (all (DimDate),DimDate[Nepali Year Month Number]=prev_fiscal_mon))
var result=CALCULATE ([Industry FPI], DATESBETWEEN(DimDate[DateValue],py_st_date,py_end_date))
return 
IF(
    NOT (ISBLANK (SELECTEDVALUE(DimDate[Nepali Year Month])))
    , result, [YTD Industry FPI Last Year]

)


•	Step 10: Nine matrix tables are selected and all of the dax measures that are calculated and placed in the values section of the matrix table.
•	Step 11: Nine Bookmarks are added for all of the categories of the industry data and grouped together as the Industry Data.
•	Step 12: The Industry data bookmark is selected for the bookmark navigators. This will automatically populate the navigator list with the bookmarks.
•	Step 13: Another bookmark named home is added and after inserting an image in the Industry data page for the action of the image the Home bookmark is selected which when selected will be directed to the home page
•	Step 14: The matrix tables are further designed using combinations of icons, background color based on different indicators such as growth, decline, etc.

