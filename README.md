xps
===

eXquisite Ports Seeker - An beautiful and easy way to search the FreeBSD ports tree.

xps is a tool that searches the ports INDEX file and prints all ports whose metadata contain the given terms and match the specified criterias.

The default mode prints a line for each port found. The brackets in the beginning of each line show the port's status. For the time being, this may only contain 'i' if the port is installed.

Examples:
---------

Show all ports whose names contain 'firefox' and print verbose descriptions:
xps -v firefox

Show all ports in category 'devel' with exact name 'python'.
xps -e -c devel python

Show all ports whose names contain 'glib' and are installed:
xps -i yes glib

Show all ports maintained by <author> in category <category>:
xps -m <author> -c <category>

Show all ports that contain 'pdf' in thier short description:
xps -D pdf

Show ports whose name starts with 'gnome':
xps -E '^gnome'

Show ports that can be updated to newer version:
xps -u yes
