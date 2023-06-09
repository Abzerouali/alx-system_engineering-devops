__0x01. Shell, permissions__

0. My name is Betty:

      #!/bin/bash
      su betty

     *The Script switche the current user to the user betty.

1. Who am I:

      #!/bin/bash
      id -un

     *The Script print the effective username of the current user.

2. Groups:

      #!/bin/bash
      groups

     *The Script print all the groups the current user is part of.

3. New owner:

      #!/bin/bash
      chown betty hello

     *The Script change the owner of the file hello to the user betty.

4. Empty!:

      #!/bin/bash
      touch hello

     *The Script create an empty file called hello.

5. Execute:

      #!/bin/bash
      chmod u+x hello

     *The Script add execute permission to the owner of the file hello.

6. Multiple permissions:

      #!/bin/bash
      chmod u+x,g+x,o+r hello

     *The Script add execute permission to the owner and the group owner, and read permission to other users, to the file hello.

7. Everybody!:

      #!/bin/bash
      chmod ugo+x hello

     *The Script add execution permission to the owner, the group owner and the other users, to the file hello

8. James Bond:

      #!/bin/bash
      chmod 007 hello

     *The Script set the permission to the file hello as follows:

             -Owner: no permission at all
             -Group: no permission at all
             -Other users: all the permissions

9. John Doe:

      #!/bin/bash
      chmod 753 hello

     *The Script set the mode of the file hello to this:
                  -rwxr-x-wx

10. Look in the mirror:

      #!/bin/bash
      chmod --reference=olleh hello 

     *The Script set the mode of the file hello the same as olleh’s mode.

11. Directories:

      #!/bin/bash
      chmod -R ugo+X .

     *The Script add execute permission to all subdirectories of the current directory for the owner, the group owner and all other users.

12. More directories:

      #!/bin/bash
      mkdir -m 751 my_dir

     *The Script create a directory called my_dir with permissions 751 in the working directory.

13. Change group:

      #!/bin/bash
      chgrp school hello

     *The Script change the group owner to school for the file hello

14. Owner and group:

      #!/bin/bash
      chown -hR vincent:staff .

     *The Script change the owner to vincent and the group owner to staff for all the files and directories in the working directory.

15. Symbolic links:

      #!/bin/bash
      chown -h vincent:staff _hello

     *The Script change the owner and the group owner of _hello to vincent and staff respectively.

16. If only:

      #!/bin/bash
      chown --from=guillaume betty hello

     *The Script change the owner of the file hello to betty only if it is owned by the user guillaume.
17. Star Wars:

      #!/bin/bash
      telnet towel.blinkenlights.nl

     *The Script play the StarWars IV episode in the terminal.
