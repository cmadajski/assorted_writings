Things That Help with Linux Mastery

ls	list files in a directory
	use -a to show all files, including hidden files
	use -l to show the long version of the list, including file permissions and ownership
	use -t to sort the list from most recently edited to least recently edited

pwd	prints out the path of the current directory

cat	prints the contents of a file on the command line, useful for piping

	to print the contents of a text file:	cat example.txt

	to overwrite the contents of one file with another:	cat example1.txt > example2.txt

	to append the contents of one file to another:		cat example1.txt >> example3.txt

grep	searches for a given string in a file or directory
	use -i for case-insensitive
	use -R for recursive (if searching through a directory)

	to search for a string in a file:	grep stringValue example.txt

	to search for a string in all files of a directory	grep -R stringValue /path/to/directory

	to search for a string in all files of the current directory	grep -R stringValue .


** Making Aliases **

The bash config file can be found in ~/.bash_profile

If you open .bas_profile you can add a command alias using the syntax:	alias abc="original command"

You won't be able to use the new alias unless a new Bash session is started. You can do this
manually by using the command:	source ~/.bash_profile

** Environment Variables **

They are variables that can be used during any session (if saved in the current .bash_profile).

Proper syntax:	export VAR_NAME="put something here"

Some useful built-in environment variables:
	PS1 (defines the bash cursor used to illustrate new lines)
	HOME (defines the current user's home directory)
	PATH (holds a list of directories that contain bash scripts - common commands reside here)
	env (holds all the environment variables and their associated values)

	to see current user's home directory:	echo $HOME
	to change the bash cursor:	export PS1=">> "
	to see all environment variables:	env

