# Shell basics command
## The following scripts include basic shell commands

`pwd` : this prints the absolute pathname of the current working directory.<br>
`cd` : it changes working directory to the user's home directory.
`ls -l` : displays current directory content in long format.
`ls -la` : display current directory content, including hidden files starting with ,
`ls -n -a` : displays current directory content in long format, hidden files and with user and group IDs displayed numerically
`mkdir /tmp/my_first_directory` : creates my_first_directory in /tmp/ directory.
`mv /tmp/betty /tmp/my_first_directory` : moves file 'betty' from /tmp/ directory to new directory /tmp/my_first_directory.
`rm /tmp/my_first_directory/betty` : deletes the file 'betty'.
`rmdir /tmp/my_first_directory` : deletes 'my_first_directory' directory.
`cd -` : It changes directory to previous one.
`ls -al . .. /boot` : list all files in working directory and in parent directory and the /boot directory in long format.
`file /tmp/iamafile` : prints type of file.
`ln -s /bin/ls __ls__` : creates symbolic link
`cp -nu *.html ..` : html files.
`mv [A-Z]* /tmp/u` : moves all files beginning with an uppercase letter to directory.
`rm *~` : delete all files that end with ~.
`mkdir {welcome/,welcome/to/,welcome/to/school`} : creates multiple directories in current working directory
`ls -pma` : lists all files and directories of current directory.
