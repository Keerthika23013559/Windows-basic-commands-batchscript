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
mkdir %userprofile%\Desktop\MyLab
![327055741-36936d11-8c99-4a06-86bd-371f77970536](https://github.com/Keerthika23013559/Windows-basic-commands-batchscript/assets/162658262/98670dca-5890-4460-afc4-e448993c25ea)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![327055789-8781dff8-8728-4e41-8a57-a93ab34f1897](https://github.com/Keerthika23013559/Windows-basic-commands-batchscript/assets/162658262/7902f444-340f-4ab2-aaf6-1b2bd72ad513)

![327055801-099dfe54-7391-40e7-bd86-8803550fdb23](https://github.com/Keerthika23013559/Windows-basic-commands-batchscript/assets/162658262/5e9378a8-a2d9-410f-b774-d9be58ffe6d4)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![327056060-f052d54b-31de-4d1e-a370-f41b99ea3076](https://github.com/Keerthika23013559/Windows-basic-commands-batchscript/assets/162658262/fa51a3ef-ccdf-4f93-af6b-d3fa04e1fec8)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
![327056109-ebce6ac2-931c-4bdb-bfd6-de038a3de91f](https://github.com/Keerthika23013559/Windows-basic-commands-batchscript/assets/162658262/533a8a16-b30f-4691-aeb1-3ffd5904c3ea)

![327056129-ce5af7b3-b94c-4b25-963e-dda2fb46b423](https://github.com/Keerthika23013559/Windows-basic-commands-batchscript/assets/162658262/f615a15a-0abf-433d-9a46-3c12c3a08de4)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![327056288-edcc3337-11c3-4b63-9ec3-f002ca7baa58](https://github.com/Keerthika23013559/Windows-basic-commands-batchscript/assets/162658262/23b7c105-a6e7-455d-838e-d3b14a1d1d5e)

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
![327056392-6258a13c-9ddd-4789-a9b0-d9c25d79fc3f](https://github.com/Keerthika23013559/Windows-basic-commands-batchscript/assets/162658262/6c1d82b7-16c9-443d-9f8c-08d2b11b36fa)





# RESULT:
The commands/batch files are executed successfully.

