# NAME: S.KAVIYA
# RESIGTER NO: 212223040090
# EX08 Windows-basic-commands-batchscript

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


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\MyLab
``


![image](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/21364bec-83bf-4747-8d00-71a202228b2a)



Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT:
```
cd %userprofile%\Desktop\MyLab
```




```
type nul > MyFile.txt
```

![image](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/77d18816-b629-4760-8c58-da3cb17f6820)




List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT:
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/55bae660-1ec7-4ddc-95a6-a402253bfae8)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Backup
```
![image](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/704da7ae-50e5-4b87-ad2a-a0e7734175e1)


```
copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/21ed75c8-9868-4fff-8c9b-f32875975c49)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT:
```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![image](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/9704dd14-bd81-46c0-b84d-e80b1e8f4fdf)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.




## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```


## OUTPUT:

![image](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/21f352a7-45a8-45a6-aad8-cbf124e4ec89)



## COMMAND:
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT:

![image](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/0b5f14ef-efba-489b-bcfe-5ca5fbc3c8cb)

# RESULT:
The commands/batch files are executed successfully.
