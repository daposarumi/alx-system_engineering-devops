# Shell permissions
## This contains commands and script as regards changing file permissions in the shell etc

`su betty` : script switches current user to betty
`whoami` : script prints effective username of current user
`groups` : script prints all the group current user is part of
`chown betty hello` : script changes owner of file 
`touch hello` : script creates empty file 'hello'
`chmod u+x hello` : adds execute permission to owner of file 'hello'
`chmod ug+x,o+r hello` : adds multiple permissions to file 
`chmod ugo+x hello` : script adds execution permission to users and group owner and owner
`chmod 007 hello` : script adds all permissions to only users, and adds no permissions to owner and group owner
`chmod 753 hello` : script sets the mode of file 'hello' to this `-rwxr-x-wx 1 julien julien 23 Sep 20 14:25 hello`
