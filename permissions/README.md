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
find . -type d -exec chmod a+x {} +: Create a script that adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed
mkdir -m 751 my_dir: a script that creates a directory called my_dir with permissions 751 in the working directory
chgrp school hello: script that changes the group owner of the file hello to school
chown vincent:staff *: a script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory
chown --no-dereference vincent:staff _hello: a script that  change the owner and the group owner of a symbolic link _hello to vincent and staff, respectively, you can use the following script
sudo chown vincent hello: a script that changes the owner of the file hello to vincent only if it is owned by the user guillaume
