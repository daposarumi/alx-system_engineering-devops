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
