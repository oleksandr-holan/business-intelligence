# Design a Report in Power BI Desktop

## Lab story

In this lab, you'll create a three-page report. You'll then publish it to Power BI, where you'll open and interact with the report.

In this lab you learn how to:

- Design a report
- Configure visual fields and format properties

**This lab should take approximately 45 minutes.**

## Get started

To complete this exercise, first open a web browser and enter the following URL to download the zip folder:

`https://github.com/MicrosoftLearning/PL-300-Microsoft-Power-BI-Data-Analyst/raw/Main/Allfiles/Labs/06-design-report-in-power-bi-desktop/06-design-report.zip`


Extract the folder to the **C:\Users\Student\Downloads\06-design-report** folder.

Open the **06-Starter-Sales Analysis.pbix** file.

> ***Note**: You can dismiss the sign-in by selecting **Cancel**. Close any other informational windows. Select **Apply Later**, if prompted to apply changes.*

## Design page 1

In this exercise, you'll design the first report page. When you’ve completed the design, the page will look like the following:

![Image of page 1, comprising a logo, two slicers, and three visuals.](Linked_image_Files/06-finished-report-page.png)

1. In Power BI Desktop, to rename the page, at the bottom-left, right-click **Page 1**, then **Rename** the page as **Overview**.

    > *Tip: You can also double-click the page name to rename it.*

1. To add an image, on the **Insert** ribbon tab, from inside the **Elements** group, select **Image**.

    ![Picture 1](Linked_image_Files/07-design-report-in-power-bi-desktop_image15.png)

1. In the **Open** window, navigate to the **C:\Users\Student\Downloads\06-design-report** folder.

1. Select the **AdventureWorksLogo.jpg** file, and then select **Open**.

1. Drag the image to position it at the top-left corner, and also drag the guide markers to resize it.

     ![Picture 12](Linked_image_Files/07-design-report-in-power-bi-desktop_image17.png)

1. To add a slicer, first de-select the image by clicking an empty area of the report page, then select the **Slicer** in the **Visualizations** pane.

     ![Picture 49](Linked_image_Files/07-design-report-in-power-bi-desktop_image18.png)

1. In the **Data** pane, drag the **Date \| Year** field (not the **Year** level of the hierarchy) into the slicer **Field** in Visualizations pane.

    > *The labs use a shorthand notation to reference a field. It will look like this: **Date \| Year**. In this example, **Date** is the table name and **Year** is the field name.*

1. To convert the slicer from a list to a dropdown, navigate to **Visualizations > Format visual > Visual > Slicer Settings > Style**, and then select **Dropdown** from the dropdown menu.

    ![Slicer style](Linked_image_Files/06_slicer_style.png)

1. Resize and position the slicer so it sits beneath the image and is the same width as the image.

     ![Picture 19](Linked_image_Files/07-design-report-in-power-bi-desktop_image20.png)

1. In the **Year** slicer, open the dropdown list, select **FY2020**, and then collapse the dropdown list.
    > *The report page is now filtered by year **FY2020**.*

     ![Picture 20](Linked_image_Files/07-design-report-in-power-bi-desktop_image21.png)

1. De-select the slicer by clicking an empty area of the report page.

1. Create a second slicer, based on the **Region \| Region** field (not the **Region** level of the hierarch).

1. Leave the slicer as a list, and then resize and position the slicer beneath the **Year** slicer.

     ![Picture 21](Linked_image_Files/07-design-report-in-power-bi-desktop_image22.png)

1. De-select the slicer by clicking an empty area of the report page.

1. To add a chart to the page, in the **Visualizations** pane, select the **Line and Stacked Column Chart** visual type.

     ![Picture 51](Linked_image_Files/07-design-report-in-power-bi-desktop_image26.png)

1. Resize and position the visual so it sits to the right of the logo, and so it fills the width of the report page.

     ![Picture 26](Linked_image_Files/07-design-report-in-power-bi-desktop_image27.png)

1. Drag and drop the following fields into the visual:

     - **Date \| Month**
     - **Sales \| Sales**

1. In the visual fields pane (located beneath the **Visualizations** pane), notice that the fields are assigned to the **X-axis** and **Column y-axis** wells/areas.

    > *By dragging fields into a visual, they'll be added to default wells/areas. For precision, you can drag fields directly into the wells/areas, as you'll do next.*

     ![Picture 27](Linked_image_Files/07-design-report-in-power-bi-desktop_image28_N.png)

1. From the **Data** pane, drag the **Sales \| Profit Margin** field into the **Line y-axis** well/area.

     ![Picture 28](Linked_image_Files/07-design-report-in-power-bi-desktop_image29.png)

1. Notice that the visual only has 11 months.

    > *The last month of the year, 2020 June, doesn't have any sales (yet). By default, the visual has eliminated months with BLANK sales. You'll now configure the visual to show all months.*

1. In the visual fields pane, in the **X-axis** well/area, for the **Month** field, select the down-arrow, and then select **Show Items With No Data**.

    > *Notice that the month **2020 June** now appears.*

     ![Picture 52](Linked_image_Files/07-design-report-in-power-bi-desktop_image30.png)

1. De-select the chart by clicking an empty area of the report page.

1. To add a chart to the page, in the **Visualizations** pane, select the **Stacked Column Chart** visual type.

     ![Picture 53](Linked_image_Files/07-stacked-column-chart.png)

1. Resize and position the visual so it sits beneath the column/line chart, and so it fills half the width of the chart above.

     ![Picture 33](Linked_image_Files/07-design-report-in-power-bi-desktop_image32.png)

1. Add the following fields to the visual wells/areas:

     - X-axis: **Region \| Country**
     - Y-axis: **Sales \| Sales**
     - Legend: **Product \| Category**

1. De-select the chart by clicking an empty area of the report page.

1. To add a chart to the page, in the **Visualizations** pane, click the **Stacked Bar Chart** visual type.

     ![Picture 54](Linked_image_Files/07-design-report-in-power-bi-desktop_image33.png)

1. Resize and position the visual so it fills the remaining report page space.

     ![Picture 35](Linked_image_Files/07-design-report-in-power-bi-desktop_image34.png)

1. Add the following fields to the visual wells/areas:

     - Y-axis: **Product \| Category**
     - X-axis: **Sales \| Quantity**

1. To format the visual, open the **Format** pane.

     ![Picture 3](Linked_image_Files/07-design-report-in-power-bi-desktop_image35.png)

1. Expand the **Bars** and then the **Colors** group, and then set the **Default Color** property to a suitable color (to complement the column/line chart).

1. Set the **Data Labels** property to **On**.

     ![Picture 2](Linked_image_Files/07-design-report-in-power-bi-desktop_image36.png)

1. Save the Power BI Desktop file.

*The design of the first page is now complete.*

## Design page 2

In this exercise, you'll design the second report page. When you’ve completed the design, the page will look like the following:

 ![Image of page 2, comprising a slicer and matrix.](Linked_image_Files/07-design-report-in-power-bi-desktop_image37.png)

> ***Important**: When detailed instructions have already been provided in the labs, the lab steps will provide more concise instructions. If you need the detailed instructions, you can refer back to other tasks in this lab.*

1. To create a new page, at the bottom-left, select the plus icon, and rename new page to **Profit**.

1. Add a slicer based on the **Region \| Region** field.

1. Use the **Format** pane to enable the “Select All” option (in the **Slicer settings > Selection** group).

1. Resize and position the slicer so it sits at the left side of the report page, and so it is about half the page height.

     ![Picture 44](Linked_image_Files/07-design-report-in-power-bi-desktop_image40.png)

1. Add a matrix visual, and resize and position it so it fills the remaining space of the report page

     ![Picture 45](Linked_image_Files/07-design-report-in-power-bi-desktop_image41.png)

1. Add the **Date \| Fiscal** hierarchy to the matrix **Rows** well/area.

     ![Picture 46](Linked_image_Files/07-design-report-in-power-bi-desktop_image42.png)

1. Add the following five **Sales** table fields to the **Values** well/area:

     - **Orders** (from the **Counts** folder)
     - **Sales**
     - **Cost**
     - **Profit** (from the **Pricing** folder)
     - **Profit Margin** (from the **Pricing** folder)


     ![Picture 55](Linked_image_Files/07-design-report-in-power-bi-desktop_image43.png)

1. In the **Filters** pane (located at the left of the **Visualizations** pane), notice the **Filter On This Page** well/area (you may need to scroll down).

     ![Picture 57](Linked_image_Files/07-design-report-in-power-bi-desktop_image44.png)

1. From the **Data** pane, drag the **Product \| Category** field into the **Filter On This Page** well/area.

    > *Fields added to the **Filters** pane can achieve the same result as a slicer. One difference is they don’t take up space on the report page. Another difference is that they can be configured to achieve more sophisticated filtering requirements.*

1. Inside the filter card, at the top-right, select the arrow to collapse the card.

1. Add each of the following **Product** table fields to the **Filter On This Page** well/area, collapsing each, directly beneath the **Category** card:

     - **Subcategory**
     - **Product**
     - **Color**

     ![Picture 60](Linked_image_Files/07-design-report-in-power-bi-desktop_image46.png)

1. Save the Power BI Desktop file.

*The design of the second page is now complete.*

## Design page 3

In this exercise, you'll design the third—and final—report page. When you’ve completed the design, the page will look like the following:

 ![Image of page 3, comprising a slicer and three visuals.](Linked_image_Files/07-design-report-in-power-bi-desktop_image47.png)

1. Create a new page, and then rename it as **My Performance**.

1. To simulate the performance of row-level security filters, drag the **Salesperson (Performance) \| Salesperson** field to the page level filters in the filter pane.

     ![Image of Salesperson field in filter pane.](Linked_image_Files/07-design-report-in-power-bi-desktop_image999.png)

1. Select **Michael Blythe**. Data on the **My Performance** report page will now be filtered to display data for Michael Blythe only.

1. Add a dropdown slicer based on the **Date \| Year** field, and then resize and position it so it sits at the top-left corner of the page.

     ![Picture 70](Linked_image_Files/07-design-report-in-power-bi-desktop_image49.png)

1. In the slicer, set the page to filter by **FY2019**.

     ![Picture 71](Linked_image_Files/07-design-report-in-power-bi-desktop_image50.png)

1. Add a **Multi-row Card** visual, and then resize and reposition it so it sits to the right of the slicer and fills the remaining width of the page.

     ![Picture 56](Linked_image_Files/07-design-report-in-power-bi-desktop_image51.png)

     ![Picture 74](Linked_image_Files/07-design-report-in-power-bi-desktop_image52.png)

1. Add the following four fields to the visual:

     - **Sales \| Sales**
     - **Targets \| Target**
     - **Targets \| Variance**
     - **Targets \| Variance Margin**

1. Format the visual:

     - In the **Callout values** group, increase the **Text Size** property to **28pt**

     - In the **General > Effects > Background** group, set the **Color** to a light gray color (such as "White, 20% Darker) to give contrast

         ![Picture 79](Linked_image_Files/07-design-report-in-power-bi-desktop_image53.png)

1. Add a **Clustered Bar Chart** visual, and then resize and position it so it sits beneath the multi-row card visual and fills the remaining height of the page, and half the width of the multi-row card visual.

     ![Picture 59](Linked_image_Files/07-design-report-in-power-bi-desktop_image54.png)

     ![Picture 78](Linked_image_Files/07-design-report-in-power-bi-desktop_image55.png)

1. Add the following fields to the visual wells/areas:

     - Y-axis: **Date \| Month**
     - X-axis: **Sales \| Sales** and **Targets \| Target**

         ![Picture 80](Linked_image_Files/07-design-report-in-power-bi-desktop_image56.png)

1. To create a copy of the visual, press **Ctrl+C**, and then press **Ctrl+V**.

1. Position the new visual to the right of the original visual.

     ![Picture 82](Linked_image_Files/07-design-report-in-power-bi-desktop_image57.png)

1. To modify the visualization type, in the **Visualizations** pane, select **Clustered Column Chart**.

     > *It’s now possible to see the same data expressed by two different visualization types.*

     ![Picture 61](Linked_image_Files/07-design-report-in-power-bi-desktop_image58.png)

 *The design of the final page is complete.*

## Publish and explore the report

In this exercise, you'll publish the report to the Power BI service and explore the published report behavior.

> **Note**: You can review the remainder of the exercise, even if you don't have access to the online Power BI service to perform the tasks directly.

1. Select the **Overview** page, then save the Power BI Desktop file.

1. On the **Home** ribbon tab, from inside the **Share** group, select **Publish**.

    > *If you're not signed into Power BI Desktop already, you'll need to sign-in to publish.*

     ![Picture 67](Linked_image_Files/07-design-report-in-power-bi-desktop_image59.png)

1. In the **Publish to Power** BI window, notice that **My Workspace** is selected.

    > *We won't go into detail about the different items within the Power BI service in this lab.*

1. To publish the report, select **Select**. This may take a few moments.

1. When the publication has succeeded, select **Got It**.

1. Open a Microsoft Edge browser, then sign-in at `https://app.powerbi.com`.

1. In the Microsoft Edge browser window, in the Power BI service, in the **Navigation** pane (located at the left, and it could be collapsed), expand **My Workspace**.

    ![Screenshot 2024-04-18 101424](https://github.com/afelix-95/PL-300-Microsoft-Power-BI-Data-Analyst/assets/148110824/346415bc-e559-4559-84b5-ef3a1f808461)

1. Review the contents of the workspace.

    - There are four types of items that can exist in a workspace, and we talk about **reports** and **semantic models**.

    - You may need to refresh your Microsoft Edge browser if the semantic model is not visible.

    - When you published the Power BI Desktop file, the data model was published as a semantic model.

1. To explore the report, select the **Sales Analysis** report.

1. At the left, in the **Pages** pane, select the **Overview** page.

1. In the **Regions** slicer, while pressing the **Ctrl** key, select multiple regions.

1. In the column/line chart, select any month column to cross filter the page.

1. While pressing the **Ctrl** key, select another month.

     > *Note: By default, cross filtering filters all other visuals on the page.*

1. Notice that the bar chart is filtered and highlighted, with the bold portion of the bars representing the filtered months.

1. Hover the cursor over the bar chart visual, and then at the top-right, hover the cursor over the filter icon.

    > *The filter icon allows you to understand all filters that are applied to the visual, including slicers and cross filters from other visual.*

1. Hover the cursor over a bar, and then notice the tooltip information.

1. To undo the cross filter, in the column/line chart, select an empty area of the visual.

1. Hover the cursor over the stacked column chart visual, and then at the top-right, select the **Focus mode** icon.

    > *Focus mode zooms the visual to full page size.*

     ![Picture 96](Linked_image_Files/07-published-report-visual-filter.png)

1. Hover the cursor over different segments of the bar charts to reveal tooltips.

1. To return to the report page, at the top-left, select **Back to Report**.

     ![Picture 86](Linked_image_Files/07-design-report-in-power-bi-desktop_image66.png)

1. Hover the cursor over one of the visuals again, then at the top-right, select the ellipsis (…), and then notice the menu options. Try out each of the options, except the ones within **Share**.

     ![Picture 97](Linked_image_Files/07-design-report-in-power-bi-desktop_image67.png)

1. At the left, in the **Pages** pane, select the **Profit** page.

     ![Picture 84](Linked_image_Files/07-design-report-in-power-bi-desktop_image68.png)

1. Notice that the **Region** slicer has a different selection to the **Region** slicer on the **Overview** page.

    > *The slicers aren't synchronized. You’ll modify the report design to ensure they sync between pages in the **Enhance a Report in Power BI Desktop** lab.*

1. In the **Filters** pane (located at the right), expand a filter card, and apply some filters.

    > *The **Filters** pane allows you to define more filters than could possibly fit on a page as slicers.*

1. In the matrix visual, use the plus (+) button to drill into the **Fiscal** hierarchy.

1. Select the **My Performance** page.

     ![Picture 89](Linked_image_Files/07-design-report-in-power-bi-desktop_image69.png)

1. At the top-right on the menu bar, select **View**, and then select **Full Screen**.

     ![Picture 98](Linked_image_Files/07-design-report-in-power-bi-desktop_image70.png)

1. Interact with the page by modifying the slicer, and cross filtering the page.

1. At the bottom of the window, notice the commands to change page, navigate backwards or forwards between pages, or to exit full screen mode.

1. Select the right icon to exit full screen mode.

     ![Picture 91](Linked_image_Files/07-design-report-in-power-bi-desktop_image71.png)

## Lab complete
