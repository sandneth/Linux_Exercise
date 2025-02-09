Part 1
1. code : apt --version
2. code : sudo apt update
   - Fetches the latest package metadata.
   - Ensures you install the most recent versions.
3. code : sudo apt upgrade -y
   update- refreshes the package list without installing anything.
   upgrade- installs new versions of currently installed packages.
4. code : apt list --upgradable

Part 2 

5. code : apt search image editor
6. code : apt show gimp
    Depends: libc6, libgimp2.0, libgtk2.0
7. code : sudo apt install gimp -y
8. code : apt list --installed | grep gimp
   2.10.36-3ubuntu0.24.04.1 amd64 

Part 3

9. code : sudo apt remove gimp -y
    No, configuration files remain.
10. code : sudo apt purge gimp -y
     remove- uninstalls the package but keeps config files.
     purge- deletes both the package and its config files.
11. code : sudo apt autoremove -y
      Removes packages no longer needed by any installed application.
12. code : sudo apt clean
      Deletes cached '.deb' files to free up disk space.

Part 4

13. code : cat /etc/apt/sources.list
      Contains URLs for package sources.
14. code : sudo add-apt-repository universe
           sudo apt update
      Community-maintained packages not officially supported by Ubuntu.
15. code : sudo apt install fakepackage
      Eror : Unable to locate package fakepackage
      Verify package name.
      Run 'sudo apt update' and retry.
      Search for available packages using 'apt search'.

Bonus Challenge 

code : sudo apt-mark hold gimp
code : sudo apt-mark unhold gimp
  Prevents updates for system stability.
      
