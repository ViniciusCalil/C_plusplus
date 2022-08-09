# Directory Content Analyzer

The zip file "DirectoryContentAnalyzer.zip" has a C++ project which its objective is to collect information (name, size, modification date, etc) about all files and subdirectories in a file system subtree. The report generated can be copy-and-paste'd into any text editor.

The zip file also contains the executable file of the project, in the subdirectory ".\bin\Debug\".

This project was written in the "Code::Blocks" IDE and uses the UI toolkit "wxWidgets" version 3.1.2 with Code::Blocks' wxSmith resource. It was compiled by MinGW-W64 (version : MinGW-W64-builds-4.3.4) and gcc (version 7.3.0).


================================================================================
Additional information and development status:
----------------------------------------------

Inside the zip file there is another README.txt file with more detailed information.

================================================================================
Usage:
------

    1) Insert a directory path and name in the "Base Directoy" text box. You can use a browser to select it, by clicking in "Search" button.
    2) If you also want to know file size, modification time, etc, check the "Show Properties" check box inside the group box "Contents Option".
    3) If you want to search along all the subtree, check theh "Analyze Subdirectories" check box inside the group box "Contents Option".
    4) Click the "Start" button inside the group box "Analysis" so the program can start to generate the report.
    5) If you want to export the generated report, you can use de Windows copy and paste functionality ("Ctrl+C" and "Ctrl+V" hotkeys).

================================================================================

Vinicius Calil, 2019/02/27.
