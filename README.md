# Kickstarter Analysis Challenge

## Overview
 

Louise is an up-and-coming writer who is hoping to raise funds for her play "Fever." She came up with her own financial plan, but she needed help gathering, classifying, and analyzing the crowdsourced data to see if there were any unique elements that contributed to a successful campaign. She was able to get close to her fundraising target in a short length of time using this information. She now needs help determining how well these campaigns worked in relation to their debut dates and financing goals.

## Analysis and Challenges
 

You can make a pivot chart and a pivot table using the crowdsourced dataset in Excel. These tools are adaptable and effective because they allow you to select and choose the data you wish to evaluate using visual adjustments. Even after the data has been selected and the pivot table has been transformed to a graph, you can continue to alter the view with filters and customizations. The pivot charts use the data in the pivot table to build visuals, such as line graphs, to detect any trends, as we did for Louise's project analysis. We would utilize the subcategory theater to focus our analysis on a more relevant aspect of Louise's project because her campaign is for a play.

### Analysis of Outcomes Based on Launch Date
 

A column for years was added to the Kickstarter worksheet to get simply the years from the date launched column in order to present the outcomes based on launch date. It is divided by years since it contains a variety of dates that would be impossible to display on a graph. The results of theatrical productions were then filtered out of the parent category. You must select the correct field name for the filters, columns, rows, and values in the Pivot Table fields, or your pivot table will not display the correct data. The field years and parent category would be selected as filters because we are reporting outcomes based on the theater's launch date. The order in which you select the filters will determine how they appear on the table. You'd proceed in the same manner with the rest of the table. After the data has been displayed in the table, you can create a line graph using the same data. This creates a visual representation of the data, allowing us to see its relationship.




### Analysis of Outcomes Based on Goals
 

A column of ranges of the goal amount was inserted in the first column of a new page to represent the results depending on goals. In the "plays" subcategory, this range of values is used to compare the outcomes of successful, failed, and canceled plays. The formula COUNTIFS() is utilized in this study to calculate the result of each outcome based on the value range. Because you must adjust the formula in each cell so that the correct range is entered, this can be difficult. For example, in cell B2 you would enter the formula =COUNTIFS('Kickstarter '!$F:$F, "successful", 'Kickstarter '!$D:$D, "<1000", 'Kickstarter '!$R:$R, "plays") but in B3 you would have to edit this formula to then state =COUNTIFS('Kickstarter '!$D:$D, ">=1000",'Kickstarter '!$F:$F, "successful",  'Kickstarter '!$D:$D,"<=4999", 'Kickstarter '!$R:$R, "plays"). The formulas for the successful, failed, and canceled outcome data would need to be changed. The data is then broken down into percentages for each range depending on the overall number of projects. This aids visualization when creating a line graph using this data.

### Challenges and Difficulties Encountered
 

Entering the formulas for the target range numbers to extract the data from the Kickstarter worksheet was a difficulty for me. It took some time to enter the formulas in each cell as well. The correct usage of symbols has an impact on how effectively a formula works. Aside from that, it was a simple dataset to deal with in order to create an analysis.




## Results
 The results based on launch dates show that the months of May, June, and July have the largest number of successful outcomes, with May being the highest. Between those months, the difference between failed and successful outcomes is greater than the rest of the year, when the difference is consistently near. There is no discernible pattern among the canceled outcomes. Based on this data, it is recommended that you launch your financing campaign between May and July for the maximum chance of success.

Goal-based outcomes do not have a linear relationship because both successful and unsuccessful results are up and down. There may be some factor causing this association, but it appears that the higher the goal amount, the more probable it is to fail at some time. When you reach to $45,000.00 and up, you're almost certainly going to fail. Based on this line graph, a lesser goal amount of $10,000.00 or less would be preferable.

Although there is a lot of info to work with in this dataset, there are several other factors that could influence the results. The data is based on the goal amount; however, the pledged amount was not taken into consideration, which could lead to a different analytical result.

The line graph would be the ideal choice for outcomes depending on launch date because it shows how a value changes over time or over a time-series. A line graph was probably the best option for the goal-based outcomes, although I suppose a clustered bar chart might also be used. Bar charts are utilized when you’re measuring the values of discrete items such as the population by state. As you can see, the visual depiction makes it simple to compare findings.
