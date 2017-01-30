#Changelog

##4.0.4 - RSS / Login & Top Kills Cleanup
 - RSS function was broken.  Cleaned it up to get it passing RSS validation.
 - Fixed Top Kills page - background was solid black for somea reason.
 - Updated it to be more clean using the standard table design and background.
 - Moved main content down to prevent login button from being covered up.

##4.0.3 - In Game Mail
 - Added ability to send in game mail to characters.
 - Fixed bug in remote access send() function.
 - Moved Tiny MCE initalization to email page so it is not available for in game mail (plain text only allowed).

##4.0.2 - Account cleanup
 - A lot of general code / user experience cleanup.
 - Admin->Ban account for period of time.
 - Admin->Add ban IP option.
 - Admin->Account list page -> clean up active (aka suspend) / banned status.
 - Admin->Created Ban List page showing all current account and IP bans in the database.

##4.0.1 - reCAPTCHA
 - Updated user registration page to utilize Google's reCAPTCHA 2.0 
 - Check out and register for free @ https://www.google.com/recaptcha/

***

##4.0.0 - Initial Re-release
 - Updating to support new MySQLi commands
 - Fixed bug preventing donate page from loading (still need to test a full transaction)
 - Fixed image reference in Cataclysm_1 template which pointed to WotLK
 - Added character delete functionality <admin page>
 - Added account delete functionality <admin page>
 - Now able to use topKills for older style character_honor_cp style database
 - Edit realm: Fixed cosmetic issue where old settings were still shown in the form fields after saving changes.
