#Homework: 4 The Linux Filesystem

Watch the video “Linux Filesystem Explained” and read the presentation “How to navigate the filesystem” then answer the questions below.

#####1.Explain the difference between absolute path and relative path:
Absolute path is the full pathname starting from root (/). Relative path is the partial pathname starting from a directory inside your present working directory.

#####2.Why Linux uses / instead of \ for its directory paths?
Linux follows the UNIX traditions of / instead of \

#####3.In Windows, these files are all the same: File FILE file and FiLE. But in Linux this is not the case, Why?
Linux cares about capitalization, so you can have different files with the same name but but with a capital letter or lowercase letter.

#####4.What is the Filesystem Hierarchy Standard (FHS) and who maintains it?
The FHS defines the structure and layout and is maintained by the Linux Foundation.

#####5.Explain what type of files are stored in the following directories:
|Directory|What is it used for|
|-----|-----|
|/bin|Contains binary commands that can be used by system administrators, users, and scripts|
|/dev|Contains device files, such as CD/DVD-ROM drive|
|/etc|Contains static configuration files, which are also unshareable files, meaning they are local to the machine|
|/home|An optional directory that might not be included in all linux distributions: in openSUSE, it's the user's home directory|
|/lib|Contains shared libraries that are loaded when a program starts|
|/opt|Contains static shareable add-on software packages|
|/tmp|Contains temporary files that system administrators should delete whenever the system is booted|
|/var|Contains variable data files, such as log files|
|/proc|sudo files and information about system processes and resources
|/usr|Contains shareable, read-only applications and files|



#####6.How does a period at the beginning of a file name means (example .bashrc)?
it means the file is a hidden file

#####7.Which command would you use to list all the files inside the /usr/share/ directory? 
ls -a /usr/share/

#####8.If you are working in the /usr/share/icons directory and want to move to your home directory, which command would you use?
cd command

#####9.Explain what these commands do:

cd .config/.htop; - Changes the current working directory
cd ../; -  Goes back 1 or more directories
ls -lX - Lists all files in a single command then sorts by file extension

#####10.John has a lot of files in the directory /var/www/html/webapp. He wants to long list all the files, including hidden files, by modification time (newest first), and with human-readable file sizes. Which command should he use conjuring that his current working directory is:

/home/john/.git/
ls -alhts 