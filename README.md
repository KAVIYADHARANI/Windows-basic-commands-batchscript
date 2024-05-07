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

![image](https://github.com/KAVIYADHARANI/Windows-basic-commands-batchscript/assets/144870680/d5e435e6-f45d-4f8e-80a7-96cf60b1fd08)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```

![image](https://github.com/KAVIYADHARANI/Windows-basic-commands-batchscript/assets/144870680/8194d413-1beb-4bae-b876-9e46b961ff40)


![image](https://github.com/KAVIYADHARANI/Windows-basic-commands-batchscript/assets/144870680/7bf349a2-8a93-47c4-b9f9-b2067ccda8c8)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
dir %userprofile%\Desktop\MyLab
```

![image](https://github.com/KAVIYADHARANI/Windows-basic-commands-batchscript/assets/144870680/b82b1863-0114-4a02-a5b6-23d39e55c7cb)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/KAVIYADHARANI/Windows-basic-commands-batchscript/assets/144870680/36ed9dcb-a3d3-4f6e-892f-d5abf4ea8bc9)

## COMMAND AND OUTPUT
```
mv Myfile.txt %userprofile%\Documents
```

![image](https://github.com/KAVIYADHARANI/Windows-basic-commands-batchscript/assets/144870680/5a9357dd-cc5e-44ea-bc0a-26f73700986f)


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

![image](https://github.com/KAVIYADHARANI/Windows-basic-commands-batchscript/assets/144870680/be79e789-98fb-4490-a732-8798e584c434)





# RESULT:
The commands/batch files are executed successfully.

