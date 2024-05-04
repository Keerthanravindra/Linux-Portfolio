Linux File Permissions Project [Portfolio]
Google Cybersecurity Professional Certification



                                   
Project Portfolio

Title	Using Linux-commands-to-manage-file-permissions
Version	2.3
Date Issued	03/03/2024
Status	Finished
Document owner	Keerthan R
Creator name	Keerthan R
Creator organisation name	Google [Coursera]
Subject category	Cybersecurity – Linux - Permissions
 
Contents
1.	Project   Description..........................................................................................................................................................................................
2.	Check file and directory details .......................................................................................................................................................................
3.	Describe the permissions string ......................................................................................................................................................................
4.	Change  file  permissions..................................................................................................................................................................................
5.	Change file permissions on a hidden file .........................................................................................................................................................
6.	Change  directory  permissions.........................................................................................................................................................................
7.	Summary   ........................................................................................................................................................................................................
 
1.	Project Description
Authorization is the concept of granting access to specific resources in a system. It's important because without authorization any user could access and modify all files belonging to other users or system files.
This would certainly be a security risk. In Linux, file and directory permissions are used to specify who has access to specific files and directories.
The permissions do not currently reflect the level of authorization that should be given. Checking and updating these permissions will help keep their system secure.

To complete this task, I performed the following tasks:
 
2.	Check File and directory details.
This document displays the file structure of the /home/researcher2/projects directory and the permissions of the files and subdirectory it contains.
In the /home/researcher2/projects directory, there are five files with the following names and permissions. To check this, I run the ls -la command in the Shell terminal:


I use the First, ls -la displays permissions to files and directories. This shows the files and directories, including the hidden ones.
 
3.	Describe the permissions string.
The 10-character string begins each entry and indicates how the permissions on the file are set.
•	The 1st character indicates the file type. The d indicates it’s a directory. When this character is a hyphen (-
), it's a regular file.
•	The 2nd-4th characters indicate the read (r), write (w), and execute (x) permissions for the user. When one of these characters is a hyphen (-) instead, it indicates that this permission is not granted to the user.
•	The 5th-7th characters indicate the read (r), write (w), and execute (x) permissions for the group. When one of these characters is a hyphen (-) instead, it indicates that this permission is not granted for the group.
•	The 8th-10th characters indicate the read (r), write (w), and execute (x) permissions for the owner type of other. This owner type consists of all other users on the system apart from the user and the group. When one of these characters is a hyphen (-) instead, that indicates that this permission is not granted for other.
 
4.	Change file permissions.
The organization does not allow other to have write access to any files. Based on the permissions established in Step 3, identify which file needs to have its permissions modified. Use a Linux command to modify these permission.
The file project_m.txt is a restricted file and should not be readable or writable, even by the group. List the contents and permissions of the current directory and check if the group has read or write permissions.
Then, I used the chmod command to change permissions of the project_m.txt file so that the group doesn’t have read or write permissions.

 
5.	Change file permissions on a hidden file.
The research team has archived .project_x.txt, which is why it’s a hidden file. This file should not have write permissions for anyone, but the user and group should be able to read the file. Used a Linux command to assign
.project_x.txt the appropriate authorization.

By using this command and setting the correct permissions, I’ve changed the permissions of the file .project_x.txt
so that both the user and the group can read, but not write to, the file.
 
6.	Change directory permissions.
The files and directories in the project’s directory belong to the researcher2 user. Only researcher2 should be allowed to access the drafts directory and its contents. Used a Linux command to modify the permissions accordingly.

With this command, I’ve removed the execute permission for the group from the drafts directory.
 
7.	Summary
I examined various permissions to align them with my organization's desired level of authorization for files and directories in the project’s directory. To begin, I utilized the ls -la command to assess the existing permissions of the directory. This provided valuable insights that guided my subsequent actions. Afterwards, I employed the chmod command multiple times to modify the permissions of both files and directories.

