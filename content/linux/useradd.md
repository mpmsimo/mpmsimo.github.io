#Adding a user

As root create the user, then add the user to the sudoers group.

`useradd user` Creates a user on the system.

-c Adds a user with a comment associateed with the user account.

-d Specify a value to for the users home directory, it is usually the path to the home directory and the users login.

-g Add a user to a group.

-z Specifies the users shell.

#Changing a password
`passwd user` Used to reset a users password, you will be prompted to enter the password twice.

#Modifying /etc/sudoers
`visudo` On most systems you can use this command to add a user to the sudoers file to grant them access to groups, sudo access among other things.
