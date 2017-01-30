You can view a live copy of the latest version used for testing by visiting **www.mistvale.com**.

# 1 Full Install
### A) Requirements:
Apache with Mysql & PhP support
- Apache v2.2 or higher
- MySQL 5 or higher
- Php version 5.2.0 or higher
- GD compiled into Php (In windows, enable GD exetension in php.ini file).

### B) Installing The Site
 1. Make sure all files are in the same folder under you "htdocs" or "www" folder
 2. Enter your site url in your Internet Browswer (Ex: http://yourdomain.com)
 3. You will be automatically redirected to the installer.
 4. Just follow the on screen instructions.
 5. On step 2, if you arent able to use mangosweb, you will see the reason why.
 6. Once completed, you need to edit line 3 of the installer. change "$disabled = FALSE;" to "$disabled = TRUE;"
 7. Go straight to the admin panel! and go to site config. Configure the site :P
 8. Go to Realms next, and for each realm you want users to use, you need to edit that realms DB information and turn "Site Enabled" from "Disabled" to "Enabled"

### C) How To Update
 1. Go to your Admin Control Panel and click "Check For Updates" on the last row.
 2. If there are any updates, it will show you a list of files that will be updated. Click "Update MangosWeb" to begin the update process.
 3. The update process is automatic and will end in just a few seconds. Once done click "Return"
 4. Continue the process untill there are no more updates. Its that easy.

# 2 Upgrading From older versions of MangosWeb
Note: Upgrading is only supported from V3.X.  Anything prior (e.g. <= V2.X) is not supported due to unknown database modifications.
 1. Delete the two php files under the config/ directory in the V4 folder.  No modifications were performed to these files and if you upload them you will lose your site/database/realm settings.
 2. Upload all of the new directories and files to the existing MaNGOSWeb folder on your webserver.
 3. No database modification is required.
 4. Use!  MaNGOSWebV4 is now ready to use.
