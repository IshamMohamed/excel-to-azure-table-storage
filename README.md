# Excel to Azure Table Storage.
This is a console application to convert Microsoft Excel data to AzureTableStorage. Azure Table is a very exciting one and Excel worksheets suits them the most. But unfortunately a converter, that converts any existing Excel file to Azure Table is not detected (there might be, but my google didn't show that to me).

## How to
* Very simple, download the release from [here](https://github.com/IshamMohamed/excel-to-azure-table-storage/releases) and make it inside a folder. 
* Copy the Excel file you want to convert in the same folder
* Remember the worksheet number you need to convert
* Open cmd.exe, execute `ExcelToAzureTable.exe [excel_file_name] [worksheet_number]`
* eg : `ExcelToAzureTable.exe sample.xlsx 1`

After successfull exection, two new .cs files popup in the directory. To insert data into Table Storage, we need to classes, one is the helper class (that ends with Entity.cs here) and the next is execution class ([for further info](http://azure.microsoft.com/en-us/documentation/articles/storage-dotnet-how-to-use-tables/#add-entity)). You can copy the code in DataInsert.cs put it into the data insertion method.

## Tutorial
A detailed tutorial covering the need of this tool is available [here](http://social.technet.microsoft.com/wiki/contents/articles/29196.technet-guru-contributions-january-2015.aspx)
