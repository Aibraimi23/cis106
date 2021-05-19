#Notes

##Table of Contents
- [Notes Lecture 1](#notes-lecture-1)
    - [What is Linux?](#what-is-linux)
    - [What is a Linux Distribution?](#what-is-a-linux-distribution)
        - [Two of the major Linux Distributions](#two-of-the-major-linux-distributions)
        - [Two independent Distributions](#two-independent-distributions)
    - [The GNU Public License](#the-gnu-public-license)
    - [Open source vs Closed source vs Free software](#open-source-vs-closed-source-vs-free-software)
    - [What is Ubuntu](#what-is-ubuntu)
- [Notes Lecture 02 | Installing Ubuntu](#notes-lecture-02--installing-ubuntu)
    - [What is Virtualization?](#what-is-virtualization)
    - [Server-side virtualization](#server-side-virtualization)
        - [Virtual Desktop Infrastructure(VDI)](#virtual-desktop-infrastructurevdi)
    - [Client-side virtualization](#client-side-virtualization)
    - [Benefits of Virtualization](#benefits-of-virtualization)
    - [Installing Ubuntu in a virtual machine](#installing-ubuntu-in-a-virtual-machine)
    - [Desktop Environments](#desktop-environments)
        - [GUI](#gui)
        - [DE](#de)
    - [GNOME DE](#gnome-de)
    - [KDE DE](#kde-de)
    - [XFCE DE](#xfce-de)
    - [Mate DE](#mate-de)
    - [Cinnamon DE](#cinnamon-de)
    - [What is a Shell](#what-is-a-shell)
    - [The Bash Shell](#the-bash-shell)
    - [Managing Software](#managing-software)
        - [Debian Package Management System](#debian-package-management-system)
    - [The Linux Filesystem](#the-linux-filesystem)
- [Notes Lecture 04 | Manipulating files and directories](#notes-lecture-04--manipulating-files-and-directories)
    - [Creating directories](#creating-directories)
    - [Creating files](#creating-files)
    - [Deleting files and directories](#deleting-files-and-directories)
        - [rm command](#rm-command)
    - [Moving files and directories](#moving-files-and-directories)
        - [The mv command](#the-mv-command)
    - [Copying files and directories](#copying-files-and-directories)
        - [The cp command](#the-cp-command)
    - [Getting Help](#getting-help)
    - [Working with Wildcards](#working-with-wildcards)
        - [The * Wildcard](#the--wildcard)
        - [The ? Wildcard](#the--wildcard)
        - [The [ ] Wildcard](#the---wildcard)
        - [Brace Expansion](#brace-expansion)
- [Notes Lecture 05 | Command Line Text Editors](#notes-lecture-05--command-line-text-editors)
    - [The basics of Nano](#the-basics-of-nano)
        - [Opening and Creating files](#opening-and-creating-files)
        - [Saving and exiting](#saving-and-exiting)
        - [Cutting and pasting](#cutting-and-pasting)
        - [Searching for text](#searching-for-text)
    - [The basics of VIM](#the-basics-of-vim)
        - [How to start and quit vim](#how-to-start-and-quit-vim)
        - [Vim modes](#vim-modes)
        - [Editing a file with vim](#editing-a-file-with-vim)
        - [Searching words in vim](#searching-words-in-vim)
        - [Moving to Lines](#moving-to-lines)
- [Notes Lecture 06 | Managing Data and File permissions](#notes-lecture-06--managing-data-and-file-permissions)
    - [Managing Data](#managing-data)
        - [Archiving utilities](#archiving-utilities)
        - [File Compression](#file-compression)
        - [Useful commands](#useful-commands)
        - [Zip, 7Zip, and rar](#zip-7zip-and-rar)
    - [File Permissions](#file-permissions)
        - [Files vs Directories](#files-vs-directories)
        - [Files](#files)
        - [chmod command](#chmod-command)

#Notes Lecture 1
##What is Linux?
* Linux is a kernel.
* A kernel is the core of an operating system.
* Linux is a multitasking, multi user, multipurpose operating system
* Linux is an open-source operating system that is accessible to anyone who chooses to use it.
##What is a Linux Distribution?
* A linux distribution is any operating system that uses the Linux Kernel.
###Two of the major Linux Distributions
* Debian
* Redhat
###Two independent Distributions
* Slackware
* Arch
* Gentoo
##The GNU Public License
* The GPL is a free, copyleft license software and other kinds of works that guarantees end users th freedom to run, study, share, and modify the software.
* There are 3 version GPL v1, V2, and V3.
* Linux kernel is released under the GNU General Public License version 2.
##Open source vs Closed source vs Free software
| Open Source | Closed Source | Free Software |
|-----|------|-----|
|The source code is distributed with the software|The user is restricted from modifying the code|The software can be free of charge or obtained by a fee|
|The software may be distributed for a fee or free|The software is not distributed with the source code| The software is distributed with the source code
##What is Ubuntu
* Ubuntu  is a Linux distribution, freely available with both community and professional support.
* The software should be available free of charge
* The software tools should be usable by people in their local language and despite any disabilities.
* Ubuntu is suitable for both desktop and server use.
  * Intel x86 (IBM-compatible PC)
  * AMD 64 (x86-64)
  * ARMv7
  * ARMv8 (ARM64)
  * IBM POWER8/POWER9 (ppc64el)
  * IBM Z zEC12/zEC13/z14
  * IBM LinuxOne Rockhopper l+ll/Emporer l+ll (s390x)

#Notes Lecture 02 | Installing Ubuntu
##What is Virtualization?
* Replication of hardware to simulate a virtual machine inside a physical machine.
* Two general types of virtualization:
  * server-side virtualization
  * client-side virtualization
* The difference between the two is where the virtualizing takes place

##Server-side virtualization 
###Virtual Desktop Infrastructure(VDI)
* Thick client or fat client
* Think client 
* Zero client 
##Client-side virtualization
* Software installed on a computer to manage virtual machines
* Each VM has its own operating system installed
* For client-side virtualization, the computer needs:
  * A hypervisor (software that allows the management of virtual machines)
  * Hardware support
* Capable CPU
* Enough RAM
* Enough Storage
##Benefits of Virtualization
* Allows running multiple OSs on one machine 
* Allows applications to be tested before installing them on a host machine
* Reduces cost by decreasing the physical hardware that must be purchased for a network
* Offers the chance to experiment with untested programs without infecting host machines with viruses or other malware
##Installing Ubuntu in a virtual machine
* Download the iso file
* Click on new and enter a name for the virtual machine
* Select an OS type
* Select the desired memory size
* Select storage type
* Select file location and size 
* Start!
  
  #Notes Lecture 03 | Learning the Bash Shell
##Desktop Environments
###GUI
* A graphical user interface is a set of programs that allows a user to interact with the computer system vias icons, windows, and various other visual elements.
###DE
* A desktop environment is an implementation of the desktop of the desktop metaphor made of a bundle of programs running on top of a computer operating system, which shares a common GUI, sometimes described as a graphical shell.
##GNOME DE
* Default desktop in Ubuntu is GNOME 3. It is used not only by Ubuntu but also several other linux distributions such as, Debian, Fedora, Red Hat, Enterprise Linux, and Oracle Linux. The official GUI for GNOME 3 is called GNOME Shell.
* GNOME was an acronym for HNU Network Object Model Environment, but the acronym was dropped because it no longer reflected the vision of the GNOME project.
* GNOME was started August 15,1997, by Miguel de lcaza and Federico Mena as a free software project to develop a desktop environment and applications for it.
##KDE DE
* The Kool Desktop environment got its start in 1996, with its first version released in 1998
* Through time the name KDE was no longer just referring to a desktop environment, but insread, it specified the project's organization and the strong community that supported it.
##XFCE DE
* XFCE is a lightweight DE that aims to be fast and low on system resources, while still being visually appealing and user friendly
* The XFCE project was started by Oliver Fourdan in 1996.
##Mate DE
* The Mate DE is the continuation of GNOME 2.
* Mate has forked applications from GNOME core
* Mate Applications include:
  * File manager
  * Text editor
  * Document viewer
  * Archive manager 
  * Terminal emulator 
  * Window manager
##Cinnamon DE
* Cinnamon is a free and open-source DE for the X Windows System that drives from GNOME 3 but follows traditional desktop metaphor conventions.
* Cinnamon is the principal DE of the Linux Mint distribution
* The development of Cinnamon started as a response to the release GNOME 3 and the GNOME Foundation decision of dropping support for GNOME 2
##What is a Shell
Shells make large-scale IT possible. They're a necessary component to modern computing. But it might not have turned out that way without a lot of hard work from a developer at the Free Software foundation named Brian Fox. The Bash shell is shipped with almost every computer in the world.
##The Bash Shell
* The GNU bash shell is a program that provides interactive access to the Linux system.
* It runs as a regular program and is normally started whenever a user logs in into a terminal.
* Most Linux distributions use the bash shell as the default shell. however, other shells exist like
  * Tcsh Shell
  * Csh Shell
  * Ksh Shell
  * Zsh Shell
  * Fish Shell
##Managing Software
###Debian Package Management System
* The DPMS is the foundation for managing software on all Debian distributions
* Debian package names end with .deb extension and are called ".deb files"
* At the core of the DPMS is the dpkg (Debian Package) application
* Dpkg works in the back-end of the system. dpkg can directly manipulate .deb files.
##The Linux Filesystem
* Linux organizes its files in what is called a hierarchical directory structure (tree like pattern of folders).
* Directory and folder mean the same thing
* the first directory in the file system is called the root directory. the root directory contains files and subdirectories.
* Filesystem Hierarchy Standard (FHS) Specifies requirements and guidelines for file and directory placement in UNIX-like operating systems.

#Notes Lecture 04 | Manipulating files and directories
##Creating directories 
* mkdir is used for creating a single directory or multiple directories
* to create multiple directories, separate each directory name with a space
* You can create directories in the present working directory or in a different directory by using an absolute path or relative path
##Creating files
* touch command is used for creating files
* Create a file called list - touch list
##Deleting files and directories
###rm command
* rm removes files
* rm by default does not remove directories. To remove a directory use rm with -r option
* In linux and other Nix systems you cannot remove non empty directories 
* To remove empty directories use the rmdir command 
* To remove non-empty directories use rm -r + directory name or directory absolute path
##Moving files and directories
###The mv command
* mv moves and renames directories
* The basic formula of the mv command is:
  * mv + source + destination
* Where source is the file or directory that you want to move and destination is where the directory or file is going
* Both source and destination can be an absolute path or relative path 
##Copying files and directories
###The cp command
* cp copies files/directories from source to a destination 
* The cp command uses the same structure as the mv command
  * cp + files to copy + destination 
* To copy directories you must use the -r option
  * cp -r + directory to copy + destination
##Getting Help
* Man pages are documentation files that describe Linux shell commands, executable programs, system calls, special files, and so forth
* Man Pages are quick references 
* To view a man page type: man + command
* To exit the man page press letter "q"
* Most commands have a help a help option built in. Normally that option is -h or --h or --help
* Some commands my not have a man page but an info page
* You can use the whatis command to display a simple description of what a command does
##Working with Wildcards
* Wildcard represent letters and characters used to specify a filename for searches
* File globbing is the processing of pattern matching using wildcards
* The wildcards are officially called metacharater wildcards
###The * Wildcard
* The main wildcard is a star, or asterisk (*) character
* A start alone matches anything and nothing and matches any number of charaters
###The ? Wildcard
* The ? wildcard metacharacter matches precisely one character
* In addition, the question mark proves very useful when working with hidden files
* If you want to list all hidden files you can use: ls ..??* which will match all files that start with a . or .. abd have any character after it.
###The [ ] Wildcard 
* The brackets wildcard match a single character in a range
* The brackets wildcard wildcard use the exclamation mark to reverse the match.For example, match everything except the vowels [!aeiou] or any other character except numbers [!0-9]
###Brace Expansion
* Brace expansion {} is not a wildcard but another feature of bash that allows you to generate arbitrary strings to use with commands

#Notes Lecture 05 | Command Line Text Editors
##The basics of Nano
###Opening and Creating files
* For opening and creating files
  * nano + filename
###Saving and exiting 
* If you want to save the changes you've made ctrl + 0
* To exit nano, type ctrl + X
* If you ask nano to exit from a modified file, it will ask you if you want to save it, just press N for no and Y for yes. It will then ask for a filename and press enter
###Cutting and pasting
* To cut a single line, you can use ctrl +k the line disappears
* To paste it, use ctrl + U
###Searching for text
* Searching for string is east as long as you think "Whereis" instead of "Search" Simply hit ctrl + W type in you string and press enter
##The basics of VIM
* The vi command is now linked to the vim command, so even when you issue the vi command, you're actually starting the vim editor
* To install vim 
  * sudo apt install vim
###How to start and quit vim
* To start vim typ vim
* To quit vim press esc and type :qa!
  * : prefix for entering command line mode
  * q short for quit 
  * a short for all buffers
  * ! force
  * :qa! quit all now
* To set line numbers :set number
###Vim modes
* Insert mode: used for writing texts
* Normal mode: used for manipulating text
* Command mode: used for entering vim commands
* Visual mode: used for navigation and manipulation of text selections
* Select mode: similar to visual mode
* Ex-mode: Similar to the command-line mode but optimized for batch processing
###Editing a file with vim
* You can tell vim that you want to edit another file by using the e command
* :e new,txt will now open new.txt and allow you to edit
* ctrl + g will show the file that you are currently editing in the status line
* You can also use :f in command mode to see the file that you are currently working on
###Searching words in vim
* Use / and the word you are looking for to search forward
* Letter n will repeat the search for the next word
* ? To search backward 
* *will search for the next occurrence of the word under the cursor
* #will search backward for the previous occurrence of the word under the cursor
###Moving to Lines
* To move to a specific line use : plus the line number
  * :8 will move you to line 8
  * Additionally use 8G
* $ will move to the end of the line
* 0 will move to the beginning of the line
* + executes any vim command from the shell prompt 

#Notes Lecture 06 | Managing Data and File permissions
##Managing Data
* Backup- Copies files and directories to an archive 
* System backup- Use to restore data in case of a system failure or data loss and corruption
* Archive- File containing many other files, each of which is still identified by its filename, owner, permissions, and timestamp 
###Archiving utilities
* Tar(Tape archive)- creates archives by combining files and directories into a single file
* CPIO- Creates an archive, restores files from an archive, or copies a directory hierarchy. The CPIO utility has three modes of operation:
  * Create mode places multiple files into a single archive file
  * Extract mode restores files from an archive
  * Pass-through mode copies a directory hierarchy 
* Ar- Creates, modifies, and extracts from archives
###File Compression
* Gzip, Bzip2, and xz commands are used for compression
* Gzip, Bzip2, and xz compress files in place meaning the original file is deleted after compression
* bzip offers better compression ratios in comparision to gzip
* xz produces better compression ratios than gzip and bzip2
###Useful commands
* gunzip= gzip -d
* bunzip= bzip -d
* unxz= xz -d
###Zip, 7Zip, and rar
* Zip is an archiving and compression utility
* 7zip is an open source, cross-platform and fully-featured file archiver with a high compression ratio
* To use 7zip on linux you need the package: p7zip-full
* RAR is a proprietary archive file format developed by Eugene Roshal. The command unrar allows Linux users to extract rar archives.
##File Permissions
* A file can be owned only by one user and one group
* ls -l shows you the file user owner and group owner
* The /etc/passwd file contains a list of all the users in Linux
* The /etc/group file contains a list of all the groups in Linux
* The chown command is used for changing group owner
###Files vs Directories
###Files
* R(read)
  * Gives users permission to open and view a files contents
* W(write)
  * Gives users permission to open a file and edit it contents
* X(execute)
  * Allows users to run the file
* Directories
  * R(read)
    * Allows users to list a directory's contents with commands such as ls
  * W(write)
    * Allows users to add or remove files and subdirectories
  * X(execute)
    * Allows users to switch to the directory with the cd command
###chmod command
* The chmod command is used to change permissions on files and directories 
* The permissions argument is the information used to change permissions
* The file/directory argument specifies the file or directory you want to change
* You can use the chmod command in two ways to change file permissions:
  * Symbolic Notation 
  * Numeric Notation