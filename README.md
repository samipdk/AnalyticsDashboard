This dashboard helps Life Insurance Companies understand their business performance as well as provide insights into key metrics across various dimensions of the life insurance business. The dashboard covers four revenue sources, including overall FPI, micro-insurance business, foreign employment business and Endowment Business along with additional metrics such as TPI, Renewal, Monthly Trend Analysis and Surrender Analysis. In the dashboard the life insurance companies are also categorized into four generations based on their age.
This project aims to evaluate customer satisfaction by analyzing market share and identifying any weaknesses within various categories of the life insurance business.
Steps followed
-	Step 1: Monthly insurance statistics were downloaded from the central insurance authority's official website.
-	Step 2: Select the excel workbook from get data in the Home tab in power BI Desktop the excel file is imported into the PBIX file.
  

![Step 2](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/375e5f35-4521-4ea5-98b9-2b98baed0aba)

-	Step 3: The columns of the importable tables are double checked and incase there are any errors they are fixed through editing the query or updating the data in the SQL database.

![Step 3](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/8366de64-ae9b-4978-b57d-749038824dad)
-	Step 4: The homepage is designed using a combination of Shapes, texts and images.
-	Step 5: A bookmark navigator is added on the rectangular shape of the  homepage. The list is populated after the bookmarks are added.
  
![Step 5](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/17f370fb-7c4f-4196-9517-d552e0604898)  
-	Step 6: The plus sign Besides the home page is selected. This will add a new page.
-	Step 7: A square shape is inserted on the top of the page two slicers are placed for year and month. Also a bookmark navigator is inserted besides the slicers.
  
![Step 7](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/0529e186-9164-41c2-99cd-5d36e8fbb6fb)

-	Step 8: A matrix table is added and in the row pane of the matrix table the life insurance companies and generation is added.
  
![Step 8](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/eab93708-ffd4-45c4-aa25-f18ffde7155b)
-	Step 9: Dax measures were written for all the categories of life insurance i.e. Agency Business, Micro Insurance, Foreign Employment, Total Premium Income, Renewal, Surrender.
The Following Dax Measures were Used:

  For current year calculations: 

![Step 9-1](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/b6ac9a97-ce10-4ee2-92e6-1ff56463e01b)

For previous year calculations: 

![Step 9-2](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/ed6c65e7-aeca-47d4-9357-3e4dbfb2ddc0)

-	Step 10: Nine matrix tables are selected and all of the dax measures that are calculated and placed in the values section of the matrix table.

![Step 10](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/e6a6c416-ec97-42fd-99dd-088c5add20cf)

-	Step 11: Nine Bookmarks are added for all of the categories of the industry data and grouped together as the Industry Data.

![Step 11](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/6cb43523-2580-4c3f-9127-3158fd41e5fa)
  
-	Step 12: The Industry data bookmark is selected for the bookmark navigators. This will automatically populate the navigator list with the bookmarks.
-	Step 13: Another bookmark named home is added and after inserting an image in the Industry data page for the action of the image the Home bookmark is selected which when selected will    be directed to the home page

![Step 13](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/560930c4-ed0e-4d5a-b5e0-1444754457e9)
  
-	Step 14: The matrix tables are further designed using combinations of icons, background color based on different indicators such as growth, decline, etc.

![Step 14](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/548064a3-967d-4e6b-90ab-29bf8badad0c)

- Step 15: Save the file and publish the report to Power BI.

![Step 15](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/05bb19f9-6df1-42dc-a79e-87baf0112c50)
