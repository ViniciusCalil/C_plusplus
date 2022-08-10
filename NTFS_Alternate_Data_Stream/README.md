Alternate Data Stream - ADS
--------
The zip file "NTFS_ADS.zip" has the C++ project. This is a Code::Blocks IDE project. In the subdirectory ".\bin\debug\" there is the executable file.

---------------------------------------------
Description:
---------

This program allows simple tests intended to provide a little knowledge and experience with Microsoft NTFS ADS.

This program allows you: to create a file and any of its stream (the file's main stream or any ADS), to append data into any existing stream, and to read the contents of any existing stream.

---------------------------------------------
About ADS:
----------

The ADS - Alternate Data Stream is an exclusive resource of the Microsoft NTFS file system. It allows many data streams be saved into a single file.

If you open that file with normal methods (often used by most programs) only the file's main data stream is opened.

To access (create, read) an ADS, a special name format is required. But, even if you supply this special format name to common programs, they shall not access the ADS.

To access ADS you may use a special program or use Microsoft PowerShell.

For more technical information see: https://docs.microsoft.com/en-us/windows/win32/fileio/file-streams .

---------------------------------------------
Usage:
----------
  1) Type the full name (including path, name and extension) of the file that will be used in your tests. Don't use the special name format for ADS. This is the file in which you'll create new ADS's, append existing ADS and read the contents of existing ADS. 
    To exit the program, just type "0" (zero).
  2) Choose one of the following options according to your test:
       - if you want to create one new ADS, type a name that no other ADS (existent in the previous selected file) has;
       - or, type the name of an existing ADS if you want to append it with more data, or if you just want to read its content;
       - either, press only "ENTER" key to: create a new file, append the file's main stream or read the file's main stream contents.
    To exit the program, just type "0" (zero).    
 3) Select one of the following actions according to your test:
       - if you want to create one new stream (an ADS or even the file's main stream) or append an existing one, type "I";
       - if you want to read the contents of a existing stream, type "R";
       - if you just want to exit the program, type "0" (zero).
  4) If you selected "R" in the step "3)", the program will let you enter a text to be saved in the selected stream. To finish the input section, type a vertical bar character, "|" . Then, when you press "ENTER" key only the characters before the first vertical bar will be saved to the stream.
     If you selected "I", the program will show you the contents of that stream. 
     
Inside the zip file there is a "README.txt" file with more information about ADS.

---------------------------------------------
Search for files with ADS:
--------------------------

To check if there is any ADS in a specific file, use the command: 

    dir /R "specific_file_name"
    
To check if there is any file with ADS in a specific directory, use the command: 

    dir /R "directory_name" | find ":$DATA"
    
To check if there is any file with ADS in a specific directory subtree, use the command :

    dir /R /S "directory_name" | find ":$DATA" 

  Note that the subdirectory name is not displayed along the file names. If you need to find the subdirectory, you shall have to search one by one, using olny the "/R" command parameter.


Vinicius Calil, 2013/08/13.
