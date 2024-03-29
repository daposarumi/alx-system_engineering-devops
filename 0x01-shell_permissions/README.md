# Shell permissions
## This contains commands and script as regards changing file permissions in the shell etc

* `su betty` : script switches current user to betty<br>
* `whoami` : script prints effective username of current user<br> 
* `groups` : script prints all the group current user is part of<br>
* `chown betty hello` : script changes owner of file <br>
* `touch hello` : script creates empty file 'hello'<br>
* `chmod u+x hello` : adds execute permission to owner of file 'hello'<br>
* `chmod ug+x,o+r hello` : adds multiple permissions to file <br>
* `chmod ugo+x hello` : script adds execution permission to users and group owner and owner<br>
* `chmod 007 hello` : script adds all permissions to only users, and adds no permissions to owner and group owner<br>
* `chmod 753 hello` : script sets the mode of file 'hello' to this `-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello`<br>
* `chmod --reference=olleh hello` : script mirrors permission of file 'olleh'<br>
* `chmod a+x */` : script adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.<br>
* `mkdir -m 751 my_dir` : script creates directory with permission '751'<br>
* `chgrp school hello` : script changes group owner to `school` in file `hello`<br>
* `chown vincent:staff *` : script changes owner to `vincent` and gorup owner to `staff` for all the files and directories<br>
* `chown -h vincent:staff _hello` : script changes owner and group owner of file `hello`<br>
* `chown --from=guillaume betty hello` :  changes the owner of the file `hello` to `betty` only if it is owned by the user `guillaume`.<br>
* `telnet towel.blinkenlights.nl` : script plays Star Wars VI in terminal.
