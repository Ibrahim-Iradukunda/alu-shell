#!/bin/bash: act as shell
pwd: display current directory
ls: act as listing files
cd ~: changes the working directory to the user’s home directory
ls -l: Display current directory contents in a long format
ls -la: Display current directory contents, including hidden files, starting with dot (.) long format
ls -lna: Display current directory content, Long format, with user and group IDs displayed numerically, And hidden files (starting with .)
mkdir /tmp/my_first_directory: To create a script that creates a directory named my_first_directory in the /tmp/ directory
mv /tmp/betty /tmp/my_first_directory/: to move a file from one director to another
rm /tmp/my_first_directory/betty: to delete a file
rmdir /tmp/my_first_directory: to delete a directory
cd -: Changes the current directory to the previous working directory
ls -la . .. /boot: a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory
file /tmp/iamafile: write a script that prints the type of the file named iamafile
ln -s /bin/ls __ls__: Create a symbolic link
cp -u *.html ../: a script that copies all HTML files from the current working directory to the parent directory
mv [A-Z]* /tmp/u/: a script that moves all files beginning with an uppercase letter to the directory
