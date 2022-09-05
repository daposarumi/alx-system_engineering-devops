# Shell permissions
## This contains commands and script as regards changing file permissions in the shell etc

* `su betty` : script switches current user to betty<br>
* `whoami` : script prints effective username of current user<br>
`groups` : script prints all the group current user is part of<br>
`chown betty hello` : script changes owner of file <br>
`touch hello` : script creates empty file 'hello'<br>
`chmod u+x hello` : adds execute permission to owner of file 'hello'<br>
`chmod ug+x,o+r hello` : adds multiple permissions to file <br>
`chmod ugo+x hello` : script adds execution permission to users and group owner and owner<br>
`chmod 007 hello` : script adds all permissions to only users, and adds no permissions to owner and group owner<br>
`chmod 753 hello` : script sets the mode of file 'hello' to this `-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello`<br>
`chmod --reference=olleh hello` : script mirrors permission of file 'olleh'<br>
`chmod a+x */` : script adds execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. Regular files should not be changed.<br>
