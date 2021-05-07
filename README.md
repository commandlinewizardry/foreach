# foreach
Bash script for executing commands using variable arguments and options

Usage: fe [OPTION(S)] [COMMANDSTATEMENT]

Reads in standard input line by line. Replaces '{}' in
COMMANDSTATEMENT with the line from standard input and then
executes the updated COMMANDSTATEMENT.

Fe is similar to the -exec option in the find command, or a
simplified version of the xargs command.

Options:

  -n       only print COMMANDSTATEMENT, do not execute it

Usage Example:
fe 'md5sum {}' < filenames.txt

Command Line Wizardry
https://www.commandlinewizardry.com
