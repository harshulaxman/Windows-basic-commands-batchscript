# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

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

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-16 233222](https://github.com/user-attachments/assets/0b264cd7-d00a-414d-b37d-8f6bfd20b5e9)



## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-16 233235](https://github.com/user-attachments/assets/04e6c8f1-8551-412c-92f5-f4d93a88300b)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![Screenshot 2025-05-16 233247](https://github.com/user-attachments/assets/cc9d71ae-def8-4ef8-8cf9-ff74d2313eec)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
mkdir %userprofile%\Desktop\Backup

```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![Screenshot 2025-05-16 233300](https://github.com/user-attachments/assets/377e027a-e26d-4608-bee0-be6da8cbe595)



## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![Screenshot 2025-05-16 233311](https://github.com/user-attachments/assets/8f86d5b7-21db-4567-875e-f0f98231f9a9)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backupo.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```






## OUTPUT


![Screenshot 2025-05-16 232819](https://github.com/user-attachments/assets/03f27b52-b072-46cb-9a6f-f58943703c64)



# RESULT:
The commands/batch files are executed successfully.

