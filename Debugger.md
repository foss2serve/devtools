This file contains some common issues that may arise when installing the Dev Tools Debugger:

### Node Error
**Conditions:** Trying the "yarn install" command.

**Error Message:** error devtools-launchpad@0.0.98: The engine "node" is incompatible > with this module. Expected version ">=7.0.0".

**Meaning:** You currently don’t have the most recent version of node installed

**Solution:** NVM is a great way to manage the build. Use the command: nvm use 8

This will download and install node >8 and npm >5.
You may need to remove old files that yarn installed with the older version of node.
Just a note: if you use the nvm use 8 command, it will only use that version of node for the current terminal session you are in. If you close out of the terminal and reopen it, you will need to re run the nvm use 8 command before doing anything.

### Yarn Lock
**Conditions:** Trying to change Yarn versions

**Error Message:** Debugger.html has a yarn.lock

**Meaning:** Yarn needs to store exactly which versions of each dependency were installed. If you try and change the versions, this will make the build error out. The yarn lock will force dependency versions.

**Solution:** Always commit yarn.lock from the beginning to ensure versions are kept the same for all branches of the project.
