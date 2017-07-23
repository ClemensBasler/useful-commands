E: Could not get lock /var/lib/apt/lists/lock - open (11: Resource temporarily unavailable)

E: Unable to lock directory /var/lib/apt/lists/

=> sudo rm -rf /var/lib/apt/lists/* -vf 

The following packages have unmet dependencies:
 libreoffice-style-elementary : Depends: libreoffice-common (= 1:5.1.6~rc2-0ubuntu1~xenial2) but it is not installable

=> sudo dpkg -r --force-depends $pkg libreoffice-style-elementary
