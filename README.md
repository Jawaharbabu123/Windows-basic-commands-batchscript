# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware.

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
~~~
mkdir %userprofile%\Desktop\MyLab
~~~
![image](https://github.com/user-attachments/assets/d11e2311-8133-4d7c-9e10-d398ed57159d)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
~~~
cd %userprofile%\Desktop\MyLab
~~~
![image](https://github.com/user-attachments/assets/364ed0e7-4635-4534-ab77-e81b31c62cf3)

~~~
type nul > MyFile.txt
~~~
![image](https://github.com/user-attachments/assets/7daf850a-c4bf-4bc7-875f-419b59436df9)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
~~~
dir %userprofile%\Desktop\MyLab
~~~
![image](https://github.com/user-attachments/assets/59f3ec04-3022-42d4-a710-7870dd0c5c23)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Backup
~~~
![image](https://github.com/user-attachments/assets/20696441-da77-4b0f-bf3a-06f29ed716e9)

~~~
copy MyFile.txt %userprofile%\Desktop\Backup
~~~
![image](https://github.com/user-attachments/assets/4728c442-4e62-4ea7-9638-ae6d9b721673)


Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
~~~
![image](https://github.com/user-attachments/assets/0e80d2b2-da5e-44de-b6b7-0c3e4f1db1a0)




## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~
![Uploading image.png…]()


## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~
## OUTPUT

![alt text](<Screenshot 2025-05-15 152510.png>)

# RESULT:
The commands/batch files are executed successfully.

