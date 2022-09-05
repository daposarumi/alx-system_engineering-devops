# Shell basics command
## The following scripts include basic shell commands

### `pwd` : this prints the absolute pathname of the current working directory.<br>
`cd` : it changes working directory to the user's home directory.<br>
`ls -l` : displays current directory content in long format.<br>
`ls -la` : display current directory content, including hidden files starting with ','<br>
`ls -n -a` : displays current directory content in long format, hidden files and with user and group IDs displayed numerically<br>
`mkdir /tmp/my_first_directory` : creates my_first_directory in /tmp/ directory.<br>
`mv /tmp/betty /tmp/my_first_directory` : moves file 'betty' from /tmp/ directory to new directory /tmp/my_first_directory.<br>
`rm /tmp/my_first_directory/betty` : deletes the file 'betty'.<br>
`rmdir /tmp/my_first_directory` : deletes 'my_first_directory' directory.<br>
`cd -` : It changes directory to previous one.<br>
`ls -al . .. /boot` : list all files in working directory and in parent directory and the /boot directory in long format.<br>
`file /tmp/iamafile` : prints type of file.<br>
`ln -s /bin/ls __ls__` : creates symbolic link<br>
`cp -nu *.html ..` : html files.<br>
`mv [A-Z]* /tmp/u` : moves all files beginning with an uppercase letter to directory.<br>
`rm *~` : delete all files that end with ~.<br>
`mkdir {welcome/,welcome/to/,welcome/to/school`} : creates multiple directories in current working directory<br>
`ls -pma` : lists all files and directories of current directory.<br>
