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
![1 a](https://github.com/ramya23000505/Windows-basic-commands-batchscript/assets/149370791/7f214b6a-b62a-41f2-9852-cabfa0670c6b)

## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![1 b](https://github.com/ramya23000505/Windows-basic-commands-batchscript/assets/149370791/88382ef0-71b0-4658-9a40-22fe6e78ae57)

![2 b](https://github.com/ramya23000505/Windows-basic-commands-batchscript/assets/149370791/9ac64ec4-49b8-4468-bcc1-946a1b57cba0)

## COMMAND AND OUTPUT
Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![3a](https://github.com/ramya23000505/Windows-basic-commands-batchscript/assets/149370791/a9b5478d-d595-4127-bc98-e9635a0ceb9b)

## COMMAND AND OUTPUT
Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```
![4a](https://github.com/ramya23000505/Windows-basic-commands-batchscript/assets/149370791/cff2dbbb-5ae7-4043-829b-b0701d42881b)

![4b](https://github.com/ramya23000505/Windows-basic-commands-batchscript/assets/149370791/42e534ba-cc5b-4507-889f-9dc50449008b)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![5 aa](https://github.com/ramya23000505/Windows-basic-commands-batchscript/assets/149370791/e9ec16ea-ccc1-4e42-b818-d5750d97845c)

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
![output](https://github.com/ramya23000505/Windows-basic-commands-batchscript/assets/149370791/585b9169-0d26-44b7-9516-083917dacde3)
# RESULT:
The commands/batch files are executed successfully.
