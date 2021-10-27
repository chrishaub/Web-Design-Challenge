# Web Design - HTML - CSS - Web Visualization Dashboard (Latitude)

## Background

Worked with HTML and CSS to create a dashboard showing off the analysis that was completed.

## Latitude - Latitude Analysis Dashboard with Attitude

Created a visualization dashboard website using visualizations created in a past projectg. Specifically, plotted [weather data](Resources/cities.csv).

In building this dashboard, created individual pages for each plot and a means by which can navigate between them. These pages contain the visualizations and their corresponding explanations. Created a landing page, page where can see a comparison of all of the plots, and another page where can view the data used to build them.

### Website Requirements

The website consists of 7 pages total, including:

* A [landing page](#landing-page) containing:
  * An explanation of the project.
  * Links to each visualizations page. A sidebar containing preview images of each plot, and clicking an image takes the user to that visualization.
* Four [visualization pages](#visualization-pages), each with:
  * A descriptive title and heading tag.
  * The plot/visualization itself for the selected comparison.
  * A paragraph describing the plot and its significance.
* A ["Comparisons" page](#comparisons-page) that:
  * Contains all of the visualizations on the same page so can easily visually compare them.
  * Uses a Bootstrap grid for the visualizations.
    * The grid is two visualizations across on screens medium and larger, and 1 across on extra-small and small screens.
* A ["Data" page](#data-page) that:
  * Displays a responsive table containing the data used in the visualizations.
    * The table is a bootstrap table component. [See](https://getbootstrap.com/docs/4.3/content/tables/#responsive-tables)
    * The data came from exporting the `.csv` file as HTML, or converting it to HTML. Used Pandas method called `to_html` that allows you to generate a HTML table from a pandas dataframe. See the documentation [here](https://pandas.pydata.org/pandas-docs/version/0.17.0/generated/pandas.DataFrame.to_html.html)

The website, at the top of every page, have a navigation menu that:

* Has the name of the site on the left of the nav which allows users to return to the landing page from any page.
* Contains a dropdown menu on the right of the navbar named "Plots" that provides a link to each individual visualization page.
* Provides two more text links on the right: "Comparisons," which links to the comparisons page, and "Data," which links to the data page.
* Is responsive (using media queries). The nav has similar behavior as the screenshots ["Navigation Menu" section](#navigation-menu) (notice the background color change).

