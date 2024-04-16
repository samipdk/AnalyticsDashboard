Insurance Analytics-Dashboard

## Problem Statement

This dashboard helps Life Insurance Companies understand their business performance as well as provide insights into key metrics accross various dimensions of the life insurance business. The dashboard covers four revenue sources, including overall FPI, micro-insurance business,forign employment business and Endowment Business along with additional metrics such as TPI, Renewal, Monthly Trend Analysis and Surrender Analysis. In the dashboard the life insurance companies are also categorized into four generations based on their age. 

This project aims to evaluate customer satisfaction by analyzing market share and identifying any weaknesses within various categories of the life insurance business.

### Steps followed 

- Step  1:  Monthly insurance statistics were downloaded from the central insurance authority's official website.

- Step  2:  From the Excel option in the Home tab in power BI Desktop the excel file is imported into the PBIX file.

  ![sql server select](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/9c2b0c3a-159f-4fc8-9050-952be6ed17a3)

- Step  3:  The columns of the importable tables are double checked and incase there are any errors they are fixed through editing the query or updating the data in the SQL database.

  ![Snap 2](https://github.com/samipdk/AnalyticsDashboard/assets/137905918/1ecea4b1-58ad-49d2-8e7d-ac0496c1697c)
- Step  4:  The homepage is designed using a combination of Shapes, texts and images.
- Step  5:  A bookmark navigator is added on the rectangular shape of the homepage. The list is populated after the bookmarks are addded
   ![image](https://github.com/samipdk/Analytics/assets/137905918/fbe1e6e5-c0f0-4236-a6ae-4e5d86b3e8ff)
  
- Step  6:  The plus sign Besides the home page is selected. This will add a new page.
- Step  7:  A square shape is inserted on the top of the page two slicers are placed for year and month. Also a bookmark navigator is inserted besides the slicers. 
- Step  8:  A matrix table is added and in the row pane of the matrix table the life insurance companies and generation is added.
- Step  9:  Dax measures were written for all the categories of life insurance i.e. Agency Business, Micro Insurance, Foreign Employement,Total Premium Income, Renewal, Surrender.
- Step 10:  Nine matrix tables are selected and all of the dax measures that are calculated and placed in the values section of the matrix table.
- Step 11:  Nine Bookmarks are added for all of the categories of the industry data and grouped together as the Industry Data.
- Step 12:  The Industry data bookmark is selected for the bookmark navigators. This will automatically populate the navigator list with the bookmarks.
- Step 13:  Another bookmark named home is added and after inserting an image in the Industry data page for the action of the image the Home bookmark is selected which when selected
            will be directed to the home page            
- Step 14:  The matrix tables are further designed using combinations of icons, background color based on different indicators such as growth, decline, etc.            

