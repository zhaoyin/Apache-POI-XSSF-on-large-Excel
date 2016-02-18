# Apache-POI-XSSF-on-large-Excel
* This repository includes resolving very large Excel read and write problems using Apache POI. It is a Maven Java Project 
* Essentially, the source code contains XSSF read and write independently and also readAndWrite which read in memory and write into another file. It simulates the process of downlaoding a large excel and editting certain cells and then writing/appending the resulting sheet to another excel file. As a result, XSSF is able to sort out reasonable sized Excel XLSX files for both reading and writing. I believe there are plenty of people done this part following the documentations from Apache POI. You can refer more on those tutorials: [https://poi.apache.org/spreadsheet/index.html].
* However, it cannot work with very large files such as over 15k rows sheets. 
* Therefore, I developed using XSSF to read and then handle writing work to SXSSF, which enables readAndWrite happens in 40k rows sheets for all Excel files including XLSX, XLS and XLSM.  
