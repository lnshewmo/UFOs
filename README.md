# UFO Sightings with JavaScript

## Purpose 

Using JavaScript and HTML with Bootstrap and D3, an interactive webpage was developed to allow users to view data on UFO sightings recorded during January of 2010.  The data is presented in a table and can be filtered based on 5 input fields.

### Overview

A snip of the rendered page:

![overview.png](/static/images/overview.png)

## Results

To filter the table, the user must input something in one of the input fields and then hit enter.  The table will return rows which meet this criteria.  The table can then be further filtered down by selecting another criteria to enter in one of the other fields.  In this image, the table was first filtered on Date = "1/9/2010" and then further narrowed with the addition of "light" in the Shape field.  This stepwise filtering approach will maximize the return of data in the table.

![filtering.png](/static/images/filtering.png)

## Summary

**Drawback of the Redesign:**

-  If the user enters too many criteria in the filtering fields all at once, the table is likely not to return any data.
-  The original design of the webpage allowed users to filter by date only and contained a button to initalize the filter.  The new design removed the button.  

**Further Development:**

1. Add a button to clear the fields after completing a search.  To clear the fields currently, the user must empty them manually or reload the page.
2. The alignment of the search fields with its corresponding label could be fixed with the label above the field or a fixed distance from the field to improve the aesthetic.  Also the placeholder text could be greyed out to make that distinction more obvious.
3. This small dataset contains some typographical errors and lacks consistency in units, punctuation and capitialization.  Some cleaning may be in order.

### Resources

`app.js` - defines the functions which filter and build the table from the `data.js` array

`index.html` - renders and formats the webpage, connecting all the elements: bootstrap, css, d3 library, dataset and javascript functions
