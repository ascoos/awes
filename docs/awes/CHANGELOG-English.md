# 24.1.5 [1500]

⏰ 2024-12-20

### MARKINGS

- ➕ Add
- ⬆ Upgrade
- 🔧 Fix
- ⚠ Not fixed or partially fixed and continues to have a problem
- ◻ Abstraction

## ⚠️ WARNING
If you have AWES on a different drive than C: then you need to go to the configuration window and reconfigure the AWES and USERS folders to configure the configuration files contained in this upgrade.

## AWES

- ➕ Added 21 languages (Arabic, Bengali, Brazilian, Chinese, Croatian, Dutch, French, German, Hindi, Hungarian, Italian, Japanese, Korean, Polish, Portuguese, Russian, Spanish, Swedish, Thai, Turkish, Vietnamese).
- ➕ Added a 2nd user named `test`, which becomes the owner of two indexed domains:
    - `test.loc` : Here you will do checks on your various php or third-party codes.
    - `templates.loc`: Here you will test the tamplates and themes of your websites
- ➕ Added the `Codes` menu to support:
    - Implementation of the two new domains.
    - The examples of Ascoos Framework 24.
    - phpBCL8 library examples
- 🔧 Various problem fixes have been made.

## WEB SERVERS

- ➕ `Curl` : Curl 8.11.1 added
- ⬆ `PHP 8.x` : Upgraded to 8.4.2, 8.3.15, and 8.2.27
- ⬆ `PHP Modules` : Mongodb and MessagePack Modules have been upgraded.
- ⬆ `Python` : Upgraded to version 3.13.1150

## DATABASES

- ⬆ `mongoDB` : Upgraded to version 8.0.4

## ADDONS
- ◻  The web application `phpSysInfo` was removed due to the fact that some antiviruses show it to contain dangerous code. The removal was done as a precaution to secure your computer.
This plugin will be replaced in the future with my own application.

## APPLICATIONS

- ⬆ `Visual Studio Code` : Upgraded to version 1.96.2
- ⬆ `Notepad++` : Upgraded to version 8.7.4
- ⬆ `Firefox Developer Edition` : Upgraded to version 134 Beta-10

## WEB LIBRARIES

➕ Various libraries and php modules were added. Everything is located in the folder `AWES\codes`.

The following have been added to this release:
- `\AWES\codes\php\afw`  : Ascoos Framework 24'.
- `\AWES\local\srv\php\extras\PEAR` : It contains php libraries from PEAR.
- `\AWES\local\srv\php\extras\PECL` : It contains extra php modules that have been integrated into AWES.

#### 1. Ascoos Franework 24 (Free Edition)

Require PHP >= 8.2

An initial 24.0.7 Pre-Alpha version of Ascoos Framework 24 was added that includes table management classes, table data analysis methods as well as diagramming based on table data, also date management class, etc.

This framework is preconfigured to load before executing each script, so you won't have to call it every time.

Another useful element is that through the `libs` folder, it can load with it other libraries or frameworks, such as phpbcl8, Laravel etc, as long as it is inside a folder e.g. `afw/libs/[library folder]/autoload.php`. Ascoos Framework will automatically read the autoload.php of each library inside the `libs` folder and load them with it.

#### 2. phpbcl8
The PHP 8.x functionality support library on older 8 series versions (e.g. new PHP 8.4.1 functions not present in PHP 8.2 can be run through the phpbcl8 library). This library is built into the `Ascoos Framework 24`, so it is automatically read when the framework is loaded.

#### 3. PECL PHP Modules
- ➕ `XDebug` : Xdebug is an extension for PHP, and provides a range of features to improve the PHP development experience.
- ➕ `Memcached` : Memcached is an in-memory key-value store for small chunks of arbitrary data (strings, objects) from results of database calls, API calls, or page rendering.


 
