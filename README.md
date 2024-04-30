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
![image](https://github.com/Lathika2006/Windows-basic-commands-batchscript/assets/148959215/8d1d35dd-a285-4d32-8085-7f1b7e1e6a8b)

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Lathika2006/Windows-basic-commands-batchscript/assets/148959215/a001440f-2028-4b29-a1cb-b7afed6e3de2)

![image](https://github.com/Lathika2006/Windows-basic-commands-batchscript/assets/148959215/75bc2e37-fc3a-48b1-8a16-7c6b8741dcb6)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Lathika2006/Windows-basic-commands-batchscript/assets/148959215/78147ed4-bbe6-48df-8524-52868404323a)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

```
![image](https://github.com/Lathika2006/Windows-basic-commands-batchscript/assets/148959215/33c8796d-1d41-4465-8a39-05c3a3ba14ca)


## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Lathika2006/Windows-basic-commands-batchscript/assets/148959215/e58b19a9-e3e5-4f4a-a9d7-5a68d5db234a)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![image](https://github.com/Lathika2006/Windows-basic-commands-batchscript/assets/148959215/9af7aa8f-66ad-4c49-9828-03b682ed8fc8)


# RESULT:
The commands/batch files are executed successfully.


