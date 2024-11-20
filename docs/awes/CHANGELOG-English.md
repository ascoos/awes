# 24.1.3 [1457]

!!DATE 2024-11-20

### MARKINGS
- [ NUMBER ] Initial public release of AWES
- [ + ] Add
- [ - ] Abstraction
- [ ^ ] Upgrade
- [ ! ] Fix
- [ ~ ] Not fixed or partially fixed and continues to have a problem

----------------------------------------------------------------------

# ABOUT THIS RELEASE
As of this version and later, this changelog will include only changes made to the version that you are running. This was considered necessary in order to have a greater analysis of the changes without burdening the system resources.

In aggregate, you will be able to see all changes soon through https://awes.ascoos.com/whatsnews/changes.php website (It is currently under construction).
For easy access to it, the `Help` -> `All Changes` menu has been added, just below the present menu.


## AWES
- [ + ] `Tools` : The `Tools` menu -> `Security Files [BKP] Manager` has been added, through its submenu you can get zip copies of the security files [.bkp] that AWES creates in every critical change you make through the configuration window. You can also delete these files from AWES and restore a zip copy, which you choose through a special dialog box.

- [ + ] `Logs` : Added the `Logs` -> `PHP Logs` menu with the ability to view and clear the contents of the log files of all active versions of PHP in AWES.

- [ + ] `Logs` : The `Logs` -> `Databases Logs` -> `MariaDB Logs` menu has been added with the ability to view and clear the contents of the log files of all active versions of the MariaDB database in AWES.

- [ + ] `Logs` : Added the `Logs` -> `Databases Logs` -> `MongoDB Logs` menu with the ability to view and clear the log contents of all active versions of the MongoDB database in AWES. 

- [ + ] `Windows DNS Hosts` : Added to the menu `Servers` -> `DNS` -> `DNS Hosts File` option to open in Windows Explorer, the folder where the hosts file is located. The ability to delete security files created after each change was also added to the same menu.

- [ + ] `Configuration` : Added options to delete or clean temporary and log files when AWES is terminated.

- [ ! ] `Configuration` : Fixed in the tab `Users and Domains Settings` -> `Domains Settings` -> `Will domains have a password protection option?` the `Do you want to confirm access to this domain?` command in the create a domain dialog box. 
Now when we have `Will domains have a password protection option?` selected in the AWES configuration box, then `Do you want to confirm access to this domain?` can also work, otherwise it will also be inactive.

- [ ! ] `Configuration` : Fixed in the tab `DNS Settings` -> `Windows DNS Hosts` -> `Enable Windows Hosts` the activation - disabling of the remaining options in the tab, depending on whether or not this option is selected.
Once the changes are saved in Configuration, it automatically creates the activation - deactivation of the corresponding tab and the `DNS` button in the action bar.

- [ ! ] `Configuration` : `Users and Domains Settings` -> `Users Settings` -> `Force create a primary domain for a new user` has been moved to the `Users and Domains Settings` -> `Domain Settings`.
This option will always be checked so that each new user can create his main domain.

- [ ! ] Fixed several minor bugs and conflicts in AWES and its application components.


## WEB SERVERS
- [ ^ ] `Filezilla` : FTP Server was upgraded to version 1.9.4. 
It should be remembered that the free version used in Ascoos Web Extended Studio does not support SFTP.
The initial Password to login to Filezilla management is `root`.
I have left the configuration to be done by each user, because everyone has different approaches. 


## ADDONS
- [ ^ ] `Mantis` : Upgraded to versions 2.25.8 for PHP 5.6 and version 2.27.0 for PHP >= 7.4
The previous folders 20 and 26 are not tampered with so that in case you have made some changes to the Mantis configuration, you will be able to copy it to the new folders.
You can delete the old folders 20 and 26 without fear (as long as you have backed up and recovered any uploads).


## APPLICATIONS
- [ + ] `Spintool` : Added the free spintool app to make the necessary screenshots. This application was also placed by default on the toolbar, so that it is immediately used.

- [ ^ ] `Firefox Developer Edition` -> Upgraded to version 133.0b9

- [ ^ ] `Visual Studio Code` -> Upgraded to 1.95.3


## UNCORRECTED
- [ ~ ] `PHP 5.6.40 and 8.4` --> Due to the upgrade of apache and openssl, it cannot load openssl and MongoDB drivers. 
      (#0000001 - https://issues.ascoos.com/view.php?id=1).

- [ ~ ] The SSL certificate generator sub-application was not enabled for the created domains because it still has some problems.


`THANK YOU FOR CHOOSING AWES`.