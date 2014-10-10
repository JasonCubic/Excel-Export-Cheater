# Excel Export Cheater

## How it works

This technique cheats by relying on Excel to take HTML labeled as a xls file and convert it into a spreadsheet.  It is a quick and easy hack that mostly works.  But this technique is not a perfect or even good solution because excel does throw up a warning that something is wrong with the data file.


## The breakdown of the steps are as follows

1. Wrap your table in a div
2. Create a form that submits to the PHP file SaveToExcel.php
3. Add an onsumbit that calls the javascript function saveToExcel
4. The saveToExcel javascript function sets a value in the form to the contents of the table
5. The form submits to the SaveToExcel.php script
6. The SaveToExcel.php script does some encoding before downloading the html file disguised as an xls file
7. Excel does the work to convert the html table to an excel spreadsheet