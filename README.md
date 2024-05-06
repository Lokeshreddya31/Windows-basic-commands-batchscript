# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

Developed by : Lokesh reddy A

Reg No : 212223040104

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab
![image](https://github.com/Lokeshreddya31/Windows-basic-commands-batchscript/assets/144870682/63dcf271-a6c5-4e6d-924d-8dfd7dc8c59b)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/Lokeshreddya31/Windows-basic-commands-batchscript/assets/144870682/ac0f5df9-acb7-4f29-a7e1-6b7d77574f60)
![image](https://github.com/Lokeshreddya31/Windows-basic-commands-batchscript/assets/144870682/46a1d50a-d1ff-4ac5-93b5-16f046b8dddb)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/Lokeshreddya31/Windows-basic-commands-batchscript/assets/144870682/ec26bb00-4f83-4a76-b70b-7c98c81c21ab)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/Lokeshreddya31/Windows-basic-commands-batchscript/assets/144870682/9195d646-3a9c-4b69-a731-1636b2fe4339)
![image](https://github.com/Lokeshreddya31/Windows-basic-commands-batchscript/assets/144870682/c73ed05f-85f1-45e4-ba8d-c3efa720b1f5)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![image](https://github.com/Lokeshreddya31/Windows-basic-commands-batchscript/assets/144870682/194dab8b-60a8-40c2-9436-058e7a9662a9)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```







## OUTPUT

![image](https://github.com/Lokeshreddya31/Windows-basic-commands-batchscript/assets/144870682/16bd279c-baa2-4f0d-94c4-6a5832769fa5)





# RESULT:
The commands/batch files are executed successfully.

