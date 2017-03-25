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

