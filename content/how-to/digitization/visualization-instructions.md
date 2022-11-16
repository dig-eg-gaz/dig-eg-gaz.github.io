---
title: Data Visualization Tutorial
linktitle: Data visualization
author: zach
toc: true
type: book
date: "2017-03-28"
draft: false
menu:
  digitization:
    parent: Digitization
    weight: 130

weight: 130
---

Tableau is a powerful tool that can be used to view, manipulate, explore, and analyze data. For the purposes of this course, Tableau is useful to engage with the results from our Xpath queries.

## Installation
1. Your FSU email allow you free access to Tableau’s full Desktop suite. Navigate to [this page](https://www.tableau.com/academic/students) and its instructions to download your copy of Tableau. **Be sure to use your FSU email address**.

2. You will receive a download link via email. Download Tableau and follow installation instructions.

3. After downloading and installing the software, you can follow [video tutorials](https://onlinehelp.tableau.com/current/guides/get-started-tutorial/en-us/get-started-tutorial-home.html) to get up to speed with more advanced functions. But for now, let's look at some simple examples using data from the digital Egyptian Gazette.

## Walkthrough
1. First, let's gather data to explore in Tableau. This data comes from the [Coton](/issues/templates/#coton) table, which appears regularly in the financial news section of the Egyptian Gazette.

2. Using this query: `//table[@xml:id="deg-ta-cotn01"]//cell[contains(.,'balles')]/following-sibling::cell[1]`, returns the number of bales of cotton exported. Right click on the results and save to a temporary file.

3. We will want to do more than just explore total cotton exports so let's also run this query:`//table[@xml:id="deg-ta-cotn01"]//cell[contains(.,'Angleterre')]/following-sibling::cell[1]`, along with France, Russie, Autriche, Italie, Allemagne, Espagne, and other countries to acquire the cotton export numbers to each respective destination.

4. The resulting data from each of these queries will be quite raw. We can use [Regular Expressions](/how-to/digitization/regular-expression-instructions/) to clean up our data before putting it into Tableau.

5. The spreadsheet we create from these results should contain the following variables: Month, Country, and Total Cotton Export (Bales). You can download a sample [spreadsheet](https://raw.githubusercontent.com/dig-eg-gaz/samples/master/tableau-cotton-exports.xlsx) containing these data.

6. Now that we have data representing monthly total cotton exports and where they are being shipped we want to visualize this data.

7. Open Tableau, and click "Connect to a File" in the upper left corner, and select the spreadsheet from your hard drive.

8. Make sure that Tableau is recognizing the data types in your spreadsheet (dates, country names, numbers, etc). While in the Data Source interface, change the “Month” column from string to date value by Clicking on the “Abc” icon and selecting “Date” from the drop down menu. Set the “Country” column's geographic role to "Country/Region".

9. At the bottom, click Sheet 1. After dragging and dropping the “Total Cotton Export (Bales)” cell in the row slot, place the “Month” cell in the column slot, under Marks select “Bar”.

![Cotton Exports](tableau-1905-cotton-export-total.png)

The resulting visual gives us an annual total of exports, but we can go deeper.

10. In the column slot, click the “Date” cell and select “Month”. This provides a clearer representation of fluctuations in the cotton export value during the year. <!-- If we select the second “Month” in the drop down menu it provides a visualization that includes zero value months. -->
![Cotton Exports](tableau-1905-monthly-cotton-exports.png)

11. In the "Marks" box select "Label", and click the box next to "Show Mark Labels". Now our data is effectively communicating the monthly totals of cotton exports. Now let's incorporate each destination to further increase the accuracy of the data.

12. Drag and drop the "Country" cell into the Color box. Now we can see that a majority of the cotton exported every month was shipped to England.

![Cotton Exports](tableau-cotton-exports-by-country.png)

13. For a simpler comparative drag and drop the "Country" cell into the Filters box, click none, then select which countries you want to compare. For now let's look at the difference between cotton exports to England and France.

![Cotton Exports to England and France](tableau-cotton-exports-england-france.png).

14. To create a different kind of visualization clear the Columns and Rows then drag and drop the "Country" cell into the Columns slot and "Total Cotton Export" into the Rows slot. (You may need to remove the filter to display all countries). On the right hand side of the interface click "Show Me", and select the Symbol Map option. The resulting image depicts the amount of comparative cotton exported to each location.

![Global Cotton Exports](tableau-global-cotton-exports.png)

15. To save our visualizations, click “Story”, “New Story”. Drag the desired sheet to the designated location. Click “Story”, “Export Image”.

## Conclusion
Tableau is great for creating visualisations from your data, but it also is useful for data exploration. When we create data visualisations it is important to remember to keep graphics simple and self-explanatory. For independent data exploration, however, we can try simple as well as complex approaches. Experiment with your data in the software to not only create graphics, but to see how different visualisations help you think about your research.
