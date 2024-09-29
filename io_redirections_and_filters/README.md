echo "Hello, World": script that prints "Hello, World" followed by a new line to the standard output
echo "\"(Ôo)'": script that displays a confused smiley face 
cat /etc/passwd: display the content of the /etc/passwd file
cat /etc/passwd /etc/hosts: To display the contents of both the /etc/passwd and /etc/hosts files
tail -n 10 /etc/passwd: To display the last 10 lines of the /etc/passwd file
head -n 10 /etc/passwd: To display the first 10 lines of the /etc/passwd file
head -n 3 iacta | tail -n 1: a script that displays the third line of the file iacta
echo 'Best School' > \\\*\\\\"'\"Best School\"\\'"\\\\\*\$\\\?\\\*\\\*\\\*\\\*\\\*:\) : a shell script that creates a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line
ls -la > ls_cwd_content: script that writes the output of the ls -la command into a file named ls_cwd_content
tail -n 1 iacta >> iacta: a script that duplicates the last line of the file iacta
find . -type f -name "*.js" -delete: script that deletes all regular files with a .js extension
find . -type d ! -path . ! -print  | wc -l: a script that counts the number of directories and sub-directories in the current directory
ls -t | head: a script that displays the 10 newest files in the current directory
sort | uniq -u: a script that takes a list of words as input and prints only words that appear exactly once
grep "root" /etc/passwd: Display lines containing the pattern “root” from the file /etc/passwd
