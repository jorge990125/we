You can view a live copy of the latest version used for testing by visiting **www.mistvale.com**.

# Changelog

## 4.0.8 - XSS Exploit Fix
 - Fixed XSS exploit issue in install script

## 4.0.7 - Added New Templates
 - Added Mists of Pandaria template
 - Added Burning Crusade template
 - Fixed a few broken images

## 4.0.6 - SQL script updates, Added Server Statistics page
 - Added Server Statistics page
 - Reordered entries
 - Removed hard set item ID from insert statements, used NULL instead so DB will auto_increment
 - Removed unused lines of code
 - Cleaned up top menu breadcrumb links in server statistics page
 - Cleaned up top menu breadcrumb links in players online page
 - Cleaned up the way the realm names were listed in game mail & char tools page
 - Identified several broken class references between Config & Core.  This update fixes that and cleans up the variables and functions.

## 4.0.5 - Updates & Bug Fixes for Database, Account Creation, SSOTD, Server Statistics Page
 - Optimized DB install .sql file adding unsigned to most ID's and other INT columns.
 - Also modified inc\account\account.login.php to check mw_account_extend to make sure account exists in this table at time of login.  If you create an account in the game's console they weren't replicated to this table which caused login issues.
 - SSOTD random screenshot on the home page did not show an image due to some outdated or incorrect code.  Fixed null issues and changed date to use unix timestamp.
 - Removed old DB scripts.
 - Removed server info pages since backend functions did not exist.
 - Added a 4.X to 4.0.5 migration SQL script.
 - Modified full_install.sql to reflect the DB optimizations.
 - Fixed server -> statistic page to properly pull and show images andcharacter stats.
 - Converted old style commands to new mysqli.  Added appropriate links and variables to support new structure.

## 4.0.4 - RSS, Login & Top Kills Cleanup
 - RSS function was broken.  Cleaned it up to get it passing RSS validation.
 - Fixed Top Kills page - background was solid black for somea reason.  Updated it to be more clean using the standard table design and background.
 - Moved main content down to prevent login button from being covered up.

## 4.0.3 - In Game Mail
 - Added ability to send in game mail to characters.
 - Fixed bug in remote access send() function.
 - Moved Tiny MCE initalization to email page so it is not available for in game mail (plain text only allowed).

## 4.0.2 - Account cleanup
 - A lot of general code / user experience cleanup.
 - Admin->Ban account for period of time.
 - Admin->Add ban IP option.
 - Admin->Account list page -> clean up active (aka suspend) / banned status.
 - Admin->Created Ban List page showing all current account and IP bans in the database.

## 4.0.1 - reCAPTCHA
 - Updated user registration page to utilize Google's reCAPTCHA 2.0 
 - Check out and register for free @ https://www.google.com/recaptcha/

***

## 4.0.0 - Initial Re-release
 - Updating to support new MySQLi commands
 - Fixed bug preventing donate page from loading (still need to test a full transaction)
 - Fixed image reference in Cataclysm_1 template which pointed to WotLK
 - Added character delete functionality <admin page>
 - Added account delete functionality <admin page>
 - Now able to use topKills for older style character_honor_cp style database
 - Edit realm: Fixed cosmetic issue where old settings were still shown in the form fields after saving changes.
