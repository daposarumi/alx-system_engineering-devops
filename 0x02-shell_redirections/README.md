# Shell, I/O Redirection

## The following scripts carry out different tasks under shell redirections and filters

`echo "Hello, World"` : script displays 'Hello, World" to standard output.<br/>
`echo "\"(Ôo)'"` : script displays confused smiley, the backslash is to say it is not a special character.<br/>
`cat /etc/passwd` : displays content of /etc/passwd.<br/>
`cat /etc/passwd /etc/hosts` : displays content of two files.<br/>
`tail -n 10 /etc/passwd` : displays the last ten lines of that file.<br/>
`head /etc/passwd` : displays first ten lines of file<br/>
`cat iacta |head -3 |tail -1` : script displays third line of file 'iacta'<br/>
`echo "Best School" > "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)"` : creates file that contains text "Best School"<br/>
`ls -la > ls_cwd_content` : overwrites the content of file "ls_cwd_content" with the output of 'ls -la'<br/>
`tail -1 < iacta >> iacta` : duplicates last line of file 'iacta'<br/>
`find -name "*.js" -type f -delete` : deletes all files with .js extension in current directory and sub-folders<br/>
`ls -A -lR | grep "^d" | wc -l` : counts the number of directories and subdirectories in current directory, including hidden directories and excluding the current and parent directory.<br/>
`ls -U -t | head -10` : display first ten files in directory, from newest to oldest and one file per line.<br/>
`sort | uniq -u` : displays unique words<br/>
`grep root /etc/passwd` : displays lines containing pattern "root" in file<br/>
`grep -c bin /etc/passwd` : displays number of lines that contain pattern "bin" in file<br/>
`grep -A 3 root /etc/passwd` : displays lines that contain pattern "root" and three lines after them<br/>
`grep -v bin /etc/passwd` : display all lines in files that do not contain pattern "bin"<br/>
`grep ^[[:alpha:]] /etc/ssh/sshd_config` : display all lines of files starting with a letter<br/>
`tr Ac Ze` : script replaces characters 'A' and 'c' with 'Z' and 'e' respectively<br/>
`tr -d 'cC'` : script removes all letters 'c' and 'C' from input<br/>
`rev` : script reverses input<br/>
`cut -d : -f 1,6 /etc/passwd | sort` : script displays all users and their home directory.<br/>
`find -empty | rev | cut -d'/' -f1 | rev` : script finds all empty files and directories in the current directory and all sub-directories.<br/>
`find -type f -name "*.gif" -printf "%f\n" | rev | cut -d'.' -f 2- | rev | LC_ALL=C sort -f` : lists all files with .gif extension in current directory and sub-directories.<br/>
`cut -c1 | paste -s | tr -d "[:blank:]"` : acrostic script<br/>
`tail -n +2 | cut -f1 | sort | uniq -c | sort -nr | head -11 | tr -s ' ' | cut -d' ' -f3` : script parses web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.<br/>
