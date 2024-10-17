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
~~~
mkdir %userprofile%\Desktop\MyLab
~~~
![Screenshot 2024-10-17 202609](https://github.com/user-attachments/assets/ae314d3d-d247-4d8f-9d47-3364dfdda9e0)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
~~~
cd %userprofile%\Desktop\MyLab
~~~
![Screenshot 2024-10-17 202632](https://github.com/user-attachments/assets/01b8bafd-b330-4107-8d5f-a06d92654a1b)

~~~
type nul > MyFile.txt
~~~
![Screenshot 2024-10-17 202655](https://github.com/user-attachments/assets/f0b89d05-f0c0-463e-8553-cf766e27806e)


List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
~~~
dir %userprofile%\Desktop\MyLab
~~~
![Screenshot 2024-10-17 202741](https://github.com/user-attachments/assets/8ba743a9-3405-4b7e-a4cc-e6409da695b2)


Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Backup
~~~
![Screenshot 2024-10-17 202800](https://github.com/user-attachments/assets/86b190f2-74c8-4630-a08d-701480069b1c)

~~~
copy MyFile.txt %userprofile%\Desktop\Backup
~~~
![Screenshot 2024-10-17 202818](https://github.com/user-attachments/assets/7d055e42-190f-4230-9ea4-a762d15b19dc)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
~~~
![Screenshot 2024-10-17 202900](https://github.com/user-attachments/assets/86f64669-7595-4bde-8be2-6c4e59cce412)




## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~
![Screenshot 2024-10-17 202922](https://github.com/user-attachments/assets/bc4a211f-c0b1-4b0c-88c6-832e45681010)

## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~
## OUTPUT
![Screenshot 2024-10-17 202935](https://github.com/user-attachments/assets/65ec7a8d-27da-409c-a8d9-611e1663c74e)


## RESULT:
The commands/batch files are executed successfully.






# RESULT:
The commands/batch files are executed successfully.


