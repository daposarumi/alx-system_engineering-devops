# Shell, I/O Redirection

script that parses web sever logs
echo "Hello, World": script displays 'Hello, World" to standard output
echo "\"(Ôo)'": script displays confused smiley, the backslash is to say it is not a special character.
cat /etc/passwd: displays content of /etc/passwd.
cat /etc/passwd /etc/hosts: displays content of two files.
tail -n 10 /etc/passwd: displays the last ten lines of that file.
head /etc/passwd: displays first ten lines of file
cat iacta |head -3 |tail -1: script displays third line of file 'iacta'
echo "Best School" > "\*\\\'\"Best School\"\'\\\*$\?\*\*\*\*\*:)": creates file that contains text "Best School"
ls -la > ls_cwd_content: overwrites the content of file "ls_cwd_content" with the output of 'ls -la'
tail -1 < iacta >> iacta: duplicates last line of file 'iacta'
find -name "*.js" -type f -delete : deletes all files with .js extension in current directory and sub-folders
ls -A -lR | grep "^d" | wc -l : counts the number of directories and subdirectories in current directory, including hidden directories and excluding the current and parent directory.
ls -U -t | head -10 : display first ten files in directory, from newest to oldest and one file per line.
sort | uniq -u : displays unique words
grep root /etc/passwd : displays lines containing pattern "root" in file
grep -c bin /etc/passwd : displays number of lines that contain pattern "bin" in file
grep -A 3 root /etc/passwd : displays lines that contain pattern "root" and three lines after them
grep -v bin /etc/passwd : display all lines in files that do not contain pattern "bin"
grep ^[[:alpha:]] /etc/ssh/sshd_config : display all lines of files starting with a letter
tr Ac Ze : script replaces characters 'A' and 'c' with 'Z' and 'e' respectively
tr -d 'cC' : script removes all letters 'c' and 'C' from input
