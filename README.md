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

mkdir %userprofile%\Desktop\MyLab

![Screenshot 2024-05-11 222652](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/f8688554-1c88-4dde-b8ea-e5380703b8ee)





Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT:

cd %userprofile%\Desktop\MyLab


![Screenshot 2024-05-11 222731](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/e829b91f-d97c-4669-83c4-70e938cc587d)




type nul > MyFile.txt


![Screenshot 2024-05-11 222758](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/50660cbc-0bc2-4c21-a9f3-daf2944be938)





List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT:

dir %userprofile%\Desktop\MyLab

![Screenshot 2024-05-11 222821](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/fd1099d7-35c2-4db5-82d0-401206e8f10c)



Copy "MyFile.txt" to a new folder named "Backup" on the desktop.



## COMMAND AND OUTPUT:

mkdir %userprofile%\Desktop\Backup

![Screenshot 2024-05-11 222837](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/c3c58a4a-baeb-4e61-992f-0deafba0eb39)



copy MyFile.txt %userprofile%\Desktop\Backup

![Screenshot 2024-05-11 222854](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/7f29aa5d-ea72-4a91-aa41-8f9a6365414c)



Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT:

mkdir %userprofile%\Desktop\Documents

move MyLab Documents


![Screenshot 2024-05-11 222922](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/31bf1ed1-6191-4ee7-823e-25ff70fff8a1)



## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.




## COMMAND:

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!



## OUTPUT:

![Screenshot 2024-05-11 222937](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/7ef006ac-25af-4ae7-bf2f-c08f11ec0c2e)



## COMMAND:

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!


## OUTPUT:

![Screenshot 2024-05-11 223010](https://github.com/KAVIYASHANMUGAM19/Windows-basic-commands-batchscript/assets/155141139/cbe3f2df-1cc9-42f9-b145-73509cdeb205)


# RESULT:
The commands/batch files are executed successfully.
