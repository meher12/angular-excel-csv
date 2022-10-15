# Import Export Excel & CSV In Angular
## Install these packages
```
npm i xlsx
npm install --save @fortawesome/fontawesome-free
npm i bootstrap@4.6 --save
```

xlsx package provides a bunch of functions for reading and writing CSV/Excel files.

Parsing functions:-

      XLSX.read(data, read_opts) attempts to parse data

      XLSX.readFile(filename, read_opts) attempts to read filename and parse.

Note:- you can pass raw option to false if you want formatted data. (example - formatted date)

XLSX.read(data, { raw: false })
XLSX.readFile(filename, { raw: false })
JavaScript
Writing functions:-

      XLSX.write(wb, write_opts) attempts to write the workbook

      XLSX.writeFile(wb, filename, write_opts) attempts to write workbook

Utility Functions:-

      Constructing:-

            book_new creates an empty workbook

            book_append_sheet adds a worksheet to a workbook

       Importing:

           aoa_to_sheet converts an array of arrays of JS data to a worksheet

           json_to_sheet converts an array of JS objects to a worksheet

          sheet_add_aoa adds an array of arrays of JS data to an existing worksheet.

          sheet_add_json adds an array of JS objects to an existing worksheet.

    Exporting:

          sheet_to_json converts a worksheet object to an array of JSON objects.

          sheet_to_csv generates delimiter-separated-values output.

You can change the extension based on the file you want to import or export. (.xlsx, .xls, .csv)

For test you can use csv and xlsx files inside folder sample files 