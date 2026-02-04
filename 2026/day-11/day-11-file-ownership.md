# Understanding the file ownership in the linux
### What's the difference between owner and group?
  - Owner :- Owner is usually the user who created the file or directory.
    - The owner has the special permission to read, write or execute the file.
  - Group :- A group is a collection of users , it allows collaborating among different users.
    - Files can be assigned to a group so that all members of that group share certain permissions.
### Understanding ownership.
   - -rw-r--r-- 1 priyanshu_vishwakarma developer-team          57 Feb  4 06:44 linux-file.txt
   - here priyanshu_vishwkarama -- is the owner name,
   - developer-team -- is the group name.
###  Basic chgrp Operations.
   - step-1 : create a file
   - step-2 : check the current group of that file
   - step-3 : create new group :-- sudo groupadd group-name
   - step-4 : change the file group :-- sudo chgrp group-name file-name
   - verify the change :- ls -l file-name

