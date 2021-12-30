# ExportToExcel
A simple C# library to export data to an Excel file

Ever wanted to easily create a real Excel file in C#, from your DataSet, DataTable or List data ?
Now you can.

Simply add this GitHub library to your C# library, and call the `CreateExcelDocument()` function, telling it the name of your Excel file, and where your data is stored.

```
// Step 1: Create a DataSet, and put some sample data in it
DataSet ds = CreateSampleData();

// Step 2: Create the Excel .xlsx file
try
{
    string excelFilename = "C:\\Sample.xlsx";
    CreateExcelFile.CreateExcelDocument(ds, excelFilename);
}
catch (Exception ex)
{ 
    MessageBox.Show("Couldn't create Excel file.\r\nException: " + ex.Message);
    return;
}
```


You can read more about this project on my [CodeProject](https://www.codeproject.com/Articles/692121/Csharp-Export-data-to-Excel-using-OpenXML-librarie) article.

And you can follow my other work on my [Mikes Knowledge Base](http://mikesknowledgebase.com/) website.


Mike Gledhill


