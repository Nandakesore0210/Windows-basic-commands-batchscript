# EX 08: Windows-basic-commands-batchscript

## DATE:

## AIM:
To execute Windows basic commands and batch scripting

## DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 




## WINDOWS COMMANDS:

## Exercise 1: Basic Directory and File Operations

Create a directory named "MyLab" on the desktop.

## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

```
mkdir %userprofile%\Desktop\MyLab

```
![Screenshot 2024-05-07 192819](https://github.com/user-attachments/assets/9a88b327-a3c4-4d64-b52d-3825d45904c7)

```
cd %userprofile%\Desktop\MyLab
```

![Screenshot 2024-05-07 192917](https://github.com/user-attachments/assets/33f04d41-e989-4cd6-9744-cbf054f30071)

```
type nul > MyFile.txt

```

![myfile](https://github.com/user-attachments/assets/4b437b4e-c26a-4e33-a7ac-c1dda46df3f8)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```

![Screenshot 2024-05-07 193029](https://github.com/user-attachments/assets/2d8e8f85-eed3-4762-b9cc-7b138b94baa9)


## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
mkdir %userprofile%\Desktop\Backup

```

![backup](https://github.com/user-attachments/assets/4a3bfc5d-c1fc-46b2-93b1-57f5797ccedc)


```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![Screenshot 2024-05-07 193122](https://github.com/user-attachments/assets/8a7e6423-e74d-40a2-be66-4230b1f524cc)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Documents
```

```
move MyLab Documents
```

![Screenshot 2024-05-07 193431](https://github.com/user-attachments/assets/8c5b4295-d7c5-4d66-8874-937aaf94d40b)

## COMMAND AND OUTPUT


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!

```

## OUTPUT

![Screenshot 2024-05-07 203226](https://github.com/user-attachments/assets/57312ae1-05be-4505-a5c3-46e6a3a4a017)

# RESULT:
The commands/batch files are executed successfully.

