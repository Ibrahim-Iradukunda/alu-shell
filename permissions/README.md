su betty: a script that switches the current user to the user betty
whoami: a script that prints the effective username of the current user
groups: a script that prints all the groups the current user is part of
touch: a script that creates an empty file
chmod u+x: script that adds execute permission to the owner of the file
sudo chown: a script that changes the owner of the file hello to the user betty
chmod u+x,g+x,o+r hello: a script that adds execute permission to the owner and the group owner, and read permission to other users, to the file helle
chmod a+x hello: a script that adds execution permission to the owner, the group owner and the other users, to the file hello
chmod 007 hello: a script that sets the permission to the file hello but Owner: no permission at all, Group: no permission at all Other users: all the permissions
chmod 751 hello: a script that sets the mode of the file hello
chmod --reference=olleh hello:  a script that sets the mode of the file hello the same as olleh’s mode
find . -type d -exec chmod 755 {} \;: Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed
