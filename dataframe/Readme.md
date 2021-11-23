
Note about files in here...

Regarding the files, unfortunately they are ill formed. Both files, akk and top, have a column with values like 10.20% without the quotes. These values make parsing hard because they are neither a number nor a string. For the parser to work they should be between quote marks or without the %. The file worldcities works, but you need to add the infer-schema parameter (I used a value of 1000). The problem with this file is that the format for some values change. By default the command infers the data type using the first 5 rows and then continues parsing with the specified schema. By changing the value to 1000 now it uses 1000 rows to infer the schema

So I need to write a script so that when these files are generated the M's and B's are removed and the adjusted number is calculated.

ref: core-team note from nov 23, 2021
