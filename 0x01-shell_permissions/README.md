0x01. Shell, permissions
========================


About Bash projects
-------------------

Unless stated, all your projects will be auto-corrected with Ubuntu 20.04 LTS.

Resources
---------

**Read or watch**:

-   [Permissions](https://alx-intranet.hbtn.io/rltoken/aQmRB6ms-SDHUhqY0Rsa3g "Permissions")

**man or help**:

-   `chmod`
-   `sudo`
-   `su`
-   `chown`
-   `chgrp`
-   `id`
-   `groups`
-   `whoami`
-   `adduser`
-   `useradd`
-   `addgroup`



Create a script that switches the current user to the user `betty`.

-   You should use exactly 8 characters for your command (+1 character for the new line)
-   You can assume that the user `betty` will exist when we will run your script

```
julien@ubuntu:/tmp/h$ tail -1 0-iam_betty | wc -c
9
julien@ubuntu:/tmp/h$

```

**Repo:**

-   GitHub repository: `alx-system_engineering-devops`
-   Directory: `0x01-shell_permissions`
-   File: `0-iam_betty`

 Done! Help Check your code Get a sandbox QA Review

### 1\. Who am I


Write a script that prints the effective username of the current user.

```
julien@ubuntu:/tmp/h$ ./1-who_am_i
julien
julien@ubuntu:/tmp/h$

```

**Repo:**

-   GitHub repository: `alx-system_engineering-devops`
-   Directory: `0x01-shell_permissions`
-   File: `1-who_am_i`

 Done! Help Check your code Get a sandbox QA Review

### 2\. Groups



Write a script that prints all the groups the current user is part of.

```
julien@ubuntu:/tmp/h$ ./2-groups
julien adm cdrom sudo dip plugdev lpadmin sambashare
julien@ubuntu:/tmp/h$

```

Note: depending on the user, you will get a different output.

**Repo:**

-   GitHub repository: `alx-system_engineering-devops`
-   Directory: `0x01-shell_permissions`
-   File: `2-groups`

 Done! Help Check your code Get a sandbox QA Review

### 3\. New owner

Write a script that changes the owner of the file `hello` to the user `betty`.

```
julien@ubuntu:/tmp/h$ ls -l
total 4
-rwxrw-r-- 1 julien julien 30 Sep 20 14:23 3-new_owner
-rw-rw-r-- 1 julien julien  0 Sep 20 14:18 hello
julien@ubuntu:/tmp/h$ sudo ./3-new_owner
julien@ubuntu:/tmp/h$ ls -l
total 4
-rwxrw-r-- 1 julien julien 30 Sep 20 14:23 3-new_owner
-rw-rw-r-- 1 betty  julien  0 Sep 20 14:18 hello
julien@ubuntu:/tmp/h$

```

**Repo:**

-   GitHub repository: `alx-system_engineering-devops`
-   Directory: `0x01-shell_permissions`
-   File: `3-new_owner`
