MSSQL Stored Procedure to extract ORACLE inserts.
---------------------------------------------------

This code has been used in production env with the following limitations:

1. Big rows can cause errors.
2. 16-bit Encoding is write like I/x0N/x0... null character after each letter. You will need remove it.
   sed -i 's/\x0//g' file.sql
3. It does not work with CLOB.


By the way It could reduce your work. 


