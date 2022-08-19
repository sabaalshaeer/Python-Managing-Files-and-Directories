# Python-Managing-Files-and-Directories
Check to see if the output directory already exists.

Position the insertion point at the end of line 112, and press Enter twice.

Type the following code:


Line 115 checks to see if the output folder already exists on the user's computer.
If it doesn't, line 116 will create the folder.
Line 117 sets the current working directory to the output folder. This will assume that all files used in file operations such as writing, copying, and moving will be located in the output folder, unless a complete path is provided when referring to the file.
Delete lines 131 through 133.

These lines contain a placeholder comment, print statement, and trailing blank. You just completed the task identified by this placeholder.

Examine the one remaining TO-DO placeholder in line 132.


You've already written the code to save the results to a log file. Now you will copy the log file to a dated archive file.

Write code to copy the output log to a dated archive file.

Position the insertion point at the end of line 6, and press Enter.

Type the code as shown.


Line 7 imports the copyfile method from the shutil module.
In line 8, an import statement for the strftime method has already been added in preparation for generating a file name that contains the date and time.
In lines 120 through 123, examine the code that produces the log file name.


This is the code you added to get the base name of the input file, to which you append "_results.txt" to produce a name for the log file.
You will build upon this code to produce a dated name you will use for the archive copy of the log file.
Position the insertion point at the end of line 123, and press Enter.

Enter two more lines of code as shown.


Line 124 uses the strftime method to create a formatted text string containing the date and time. This is used to create a time stamp in the file name of the copied file.
Line 125 creates a name for the archive file using the base file name, the text "results_backup", the time stamp, and the file extension for text files.
Position the insertion point at the end of line 132, and press Enter.

Enter the code as shown.


Line 133 displays a message to show that the log file has been saved.
Line 136 copies the log file to create an archive file.
Line 137 displays a message to show that the archive file has been saved.
Test the archive copy functionality.

In the Project pane, right-click wordcount.py and select Run 'wordcount'.

At the three prompts, enter open-boat.txt, y, and y.


The manuscript is analyzed, and the output files are generated and listed. Files from previous runs are listed along with the dated archive file.

Re-run wordcount.py.

At the three prompts, enter open-boat.txt, y, and y.

Examine the new directory listing.


A new log file has been created, overwriting the old open-boat_results.txt file. However there are two open-boat_results_backup files because the file name includes a time stamp that means a unique file will be created each time. These backup files will continue to accrue each time the program runs.

Delete the TO-DO placeholder statements in lines 139 through 141.

Test the program's ability to create a new output folder.

On the Windows desktop, delete the Wordcount Output folder along with the files it contains.

In PyCharm, in the Project pane, right-click wordcount.py and select Run 'wordcount'.

At the three prompts, enter open-boat.txt, y, and y.

The missing output folder is created automatically, and the new log and archive file are saved to it.

