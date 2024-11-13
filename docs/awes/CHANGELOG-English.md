### MARKINGS
- [ NUMBER ] Initial public release of AWES
- [ + ] Add
- [ - ] Abstraction
- [ ^ ] Upgrade
- [ ! ] Fix
- [ ~ ] Not fixed or partially fixed and continues to have a problem
----------------------------------------------------------------------


# 24.1.2 [1421]

!!DATE 2024-11-13

#### WARNING!!!
      Once this version is downloaded, close AWES and replace the awes.exe file 
      with the awes-upd.exe by renaming it in awes.exe.

## AWES
- [ ^ ] Web application option enabled when creating a domain.
      Now, if you wish, you will be able to automatically download and install the necessary files 
      of popular web applications, such as Joomla, Drupal and Wordpress.

- [ ^ ] The upgrade window was fully activated.
      With this upgrade, you now have the option to download all upgrades through the dialog box. 
      AWES will prompt you to restart the application for the new features to take effect. 
      If it doesn't restart, the new features will only be available 
      after manually replacing the awes.exe file by renaming the awes-upd.exe to awes.exe.

- [ ! ] Fixed several minor bugs and conflicts in AWES and its application components.


## WEB SERVERS
- [ ^ ] `PHP 8.4` --> Upgraded to 8.4 RC4.

- [ ^ ] `Python 3.x` --> Upgraded to 3.13.150


## APPLICATIONS
- [ ^ ] `Firefox Developer Edition` -> Upgraded to version 133.0b7

- [ ^ ] `Visual Studio Code` -> Upgraded to 1.95.2


## UNCORRECTED
- [ ~ ] `PHP 5.6.40 and 8.4` --> Due to the upgrade of apache and openssl, it cannot load openssl and MongoDB drivers. 
      (#0000001 - https://issues.ascoos.com/view.php?id=1).

- [ ~ ] The SSL certificate generator sub-application was not enabled for the created domains because it still has some problems.


----------------------------------------------------------------------

# ASCOOS WEB EXTENDED STUDIO 24.1.1 [1409]

!!DATE 2024-10-31

### AWES
- [ + ] Added the automatic installation of the necessary SSL certificates in the Windows Root Store, so that do not hang the AWES pages running on localhost.
      The python.loc and node.loc pages require additional certificates that will be enabled to be created in subsequent versions.

- [ + ] Added option to create an Indexes view of domain contents.
      Its implementation is done during the creation of the domain through the corresponding dialog box.
      This is necessary when in a sector, we want to see in the browser the files contained in the folder and choose which one we want to execute.

- [ + ] User handling features have been added. 
      Right-clicking on the list on the selected user opens a pop-up menu, containing various functions for him:
    - Opening the user's data folder, either in Windows Explorer or in Visual Studio Code
    - Backup all its data and restore them.
    - Show the user's backup folder in Windows Explorer.

- [ + ] Domain handling capabilities have been added. 
      Right-clicking on the list on the selected sector opens a pop-up menu, containing various functions for it. 
      Indicatively, we mention:
    - Openning the domain folder either in Windows Explorer or in Visual Studio Code
    - create SSL certificate (Activation in the next version).
    - Create or delete repository (Activation in the next version)
    - The installation of a web application (Activation in the next version)
    - Backup and restore these.
    - Show the backup folder of the domain in Windows Explorer.

- [ + ] The dialog box for upgrading the AWES application was enabled. 
      Now, you don't have to download minor updates manually, although there's always the option for AWES to direct you to Sourceforge to download and install the upgrade package yourself.

- [ + ] Added the ability to notify the desktop if an upgrade is available. 
      This option is selected through the configuration dialog box on the "Upgrades" tab.

- [ ! ] Fixed bugs in the administration tab of users' domains.
    - Fixed the bug in deleting the apache configuration file when deleting a domain or subdomain.
    - Fixed bugs in automatically adding and refreshing the DNS list of the Windows Hosts file in the corresponding AWES tab, after adding or deleting domains.

- [ ! ] Fixed bugs in links to Ascoos websites.

- [ ! ] Fixed several minor bugs and conflicts in AWES and its application components.


## WEB SERVERS
- [ + ] `PHP` --> PHP version 8.4 RC3 has been added.

- [ ^ ] `PHP` --> upgraded versions 8.2.x and 8.3.x to 8.2.25, 8.3.13

- [ + ] `Memcached` --> Added the popular accelerator in version 1.6.8.

- [ + ] `MongoDB` --> Added the database in version 8.0.3, along with the compass manager. 
                  The database does not work on PHP versions 5.6 and 8.4 (See section 'UNCORRECTED').

- [ + ] `SubVersion` --> Added its function as a service in windows, but also as a component in apache. The first is temporarily disabled because it still has some bugs. As a component of apache it works and the appearance of a repository can be done either by calling it as https://localhost/svn/[RepositoryName], or more secure through the built-in WebSVN application present in the "plugins" tab.

- [ ^ ] `Apache` --> Updated apache to version 2.4.62 with openssl 3.1.7. This version works with VS17 but also runs applications built with VS16. 
                 Basically all PHP applications (5.6 - 8.4), Python and NodeJS run.

- [ - ] `MariaDB` --> 5 versions (11.0.x, 11.1.x, 11.2.x, 11.3.x, 11.5.x) were removed as it was deemed unnecessary to have so many versions of a database as their capabilities are fully covered by versions 11.4.x and 11.6.x that remained in AWES.

## ADDONS
- [ + ] `MemcacheInfo` --> Added the app to view information about memcached

- [ + ] `phpMemcachedAdmin` --> Version 1.3.0-dev of the web application has been added to provide information and manage memcached.

- [ ^ ] `phpMyAdmin` --> Upgraded to the latest version of the 6 Series that supports PHP 8.4

## APPLICATIONS
- [ ^ ] `Firefox Developer Edition` -> Upgraded to version 133.0b3

- [ ^ ] `Visual Studio Code` -> Upgraded to version 1.95.1

## UNCORRECTED
- [ ~ ] `PHP 5.6.40 and 8.4` --> Due to the upgrade of apache and openssl, it cannot load openssl and MongoDB drivers. 
      (#0000001 - https://issues.ascoos.com/view.php?id=1).

- [ ~ ] The SSL certificate generator sub-application was not enabled for the created domains because it still has some problems.

----------------------------------------------------------------------

# ASCOOS WEB EXTENDED STUDIO 24.1.0 [1332]

!!DATE 2024-10-17

### AWES
- [ ! ] Fixed critical bugs in the management tab of users and their domains.
- [ ! ] Fixed critical bugs in automatically adding or deleting domains' DNS in the Windows Hosts file.

## WEB SERVERS
- [ ^ ] IonCube PHP loaders -> Upgraded to version 14.0.0 (2024-10-14)

## DATABASES
- [ ^ ] MariaDB -> The 6 versions (11.0.x - 11.5.x) that were removed for compressed installation file size reasons were restored. So there are now 8 versions of the database available.

## APPLICATIONS
- [ ! ] Firefox Developer Edition -> Fixed bug in automatically changing user profile path when changing AWES installation folder from within the configuration window.
- [ ^ ] Firefox Developer Edition -> Upgraded to version 132.0b8


----------------------------------------------------------------------

# ASCOOS WEB EXTENDED STUDIO 24.1.0 [1263]

!!DATE 2024-10-13

## WEB SERVERS
- [ + ] SVN Subversion 1.14.4
- [ ^ ] PHP -> 8.1.30, 8.2.24, 8.3.12

## DATABASES
- [ + ] MariaDB -> 11.6.x

## APPLICATIONS
- [ ^ ] Firefox Developer Edition -> 132
- [ ^ ] Visual Studio Code -> 1.94.2
- [ ^ ] Notepad++ ->8.7.0
- [ ^ ] FileZilla FTP Client -> 3.67.1

## ADDONS
- [ ^ ] php browscap.ini -> 6001007 (2024-06-16)
- [ ! ] WebSVN (Web SVN Client)

----------------------------------------------------------------------


# ASCOOS WEB EXTENDED STUDIO 24.0.0 [1225]

### ALPHA VERSION 1

!!DATE `2024-05-30` Initial version (Read the `readme.txt` file first)

-------------------------------------------------- --------------------

## SERVERS

### WEB SERVERS
1. Apache 2.4.57
2. OpenSSL 1.1.1w
3. PHP -> 5.6.40, 7.4.33, 8.0.30, 8.1.28, 8.2.19 and 8.3.7
4. Node.js as CGI
5. Python as CGI

---

### DATABASES
1. MariaDB -> 10.x, 11.0.x, 11.1.x, 11.2.x, 11.3.x, and 11.4.x

---

### FTP SERVERS
1. FileZilla FTP Server

---

### EMAIL SERVERS
There is currently no email server.

## EXTRA
1. php browscap.ini to 6001006 (2023-12-04)
2. phpMyAdmin
3. phpFileManager (File Manager)
4. WebSVN (Web SVN Client)
5. MantisBT (Bug Manager)

---

## APPLICATIONS
1. Browser Firefox Developer Edition 126 (Portable)
2. Visual Studio Code (Portable) 1.89.1
3. Notepad++ 8.6.7
3. FileZilla FTP Client

---

## TOOLS

There is currently no tool

---

## WEB APPLICATIONS
Web applications are selected when creating a domain or subdomain through a related dropdown menu.

For starters, the following apps are supported:
1. Joomla 2.5.x - 3.x - 4.x - 5.x
2. Drupal
3. WordPress