## User Creation  

useradd [options] username    
-c comment: Add a comment describing the user    
-d home_dir: Specify the home directory    
-s shell: Specify the user's login shell    
-g initial_group: Define the primary group    
-G groups: Add the user to supplementary groups    
-m: Create the home directory if it doesn't exist    
-u UID: Specify a user ID (UID)    

## User Modification  

usermod [options] username    
-c comment: Change the comment field  
-d home_dir: Change the user's home directory  
-l new_login: Change the username  
-s shell: Change the login shell  
-u UID: Change the user ID  
-aG groups: Append the user to supplementary groups  
-L: Lock the user account (disable login)  
-U: Unlock a locked user account 

## User Deletion  

userdel [options] username 
-r: Remove the user's home directory and mail spool  

## Password Management  

passwd username Changes a user's password  
chage [options] username  
-d last_day: Set the date since the password was last changed  
-E expire_date: Set account expiration date  
-I inactive: Set password inactive days after expiration  
-m mindays: Set minimum number of days between password changes  
-M maxdays: Set maximum number of days between password changes 

## Group Management  

groupadd [options] groupname  

-g GID: Specify the group ID (GID)  
-r: Create a system group  
groupmod [options] groupname  

-g GID: Change the group ID  
-n new_groupname: Rename the group  
groupdel groupname Deletes a group  

## Changing Ownership  

chown username file/directory : Changes the file or directory owner  
chown username:group file/directory: Changes both owner and group    
chgrp group file/directory: Changes the file or directory group  

## Important Notes:  

- Most of these commands require administrative privileges (sudo).  
- Always refer to the manual pages (man useradd, man usermod, etc.) for a full list of options and detailed explanations.  
