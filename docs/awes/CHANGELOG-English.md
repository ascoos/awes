### MARKINGS
- [ NUMBER ] Initial public release of AWES
- [ + ] Add
- [ - ] Subtraction
- [ ^ ] Upgrade
- [ ! ] Correction

----------------------------------------------------------------------

# ASCOOS WEB EXTENDED STUDIO 24.1.0 [1359]

!!DATE 2024-10-21

### AWES
- [ + ] Added option to create an Indexes view of domain contents. This is necessary when in a sector, we want to see in the browser the files contained in the folder and choose which one we want to execute. This requires caution, because if the installation is for public use and not for local use, the contents of the domain will be visible globally on the Internet or internal network.

- [ ! ] Fixed bugs in the management tab of users domains. Specifically, the error in deleting the apache configuration file when deleting a domain or subdomain has been fixed.

- [ ! ] Fixed bugs in the automatic refresh of the DNS list of the Windows Hosts file in the corresponding AWES tab, after adding or deleting domains.

## ADDONS
- [ + ] mySQLiteAdmin -> Added the SQLite web database management application

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