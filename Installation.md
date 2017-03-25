You can view a live copy of the latest version used for testing by visiting **www.mistvale.com**.

# 1 Full Install
### A) Requirements:
Apache with Mysql & PhP support
- Apache v2.2 or higher
- MySQL 5 or higher
- Php version 5.2.0 or higher
- GD compiled into Php (In windows, enable GD exetension in php.ini file).

### B) Installing The Site
 1. Create a new database for MaNGOS Web to use. Example:

```
mysql -u root -p -e "CREATE DATABASE mangosweb"
```

 2. Create a user and assign privileges to the MaNGOS Web database.

```
mysql -u root -p -e "GRANT ALL PRIVILEGES ON mangosweb.* to mangos_username@localhost IDENTIFIED BY 'mangos_password'"
```

 3. Edit the PHP file: config/config-protected.php with the correct database information.


```
$dbconf = array(
'db_host'         => 'localhost',
'db_port'         => '3306',
'db_username'     => 'mangosweb_username',
'db_password'     => 'mangosweb_password',
'db_name'         => 'mangosweb',
'db_encoding'     => 'utf8',
);
```

 4. Upload the MaNGOS Web files to your webserver.
 5. Enter your site URL in your browser (e.g. http://www.mistvale.com)
 6. You will be automatically redirected to the installer.
 7. Just follow the on screen instructions.
 8. On step 2, if you are not able to use MaNGOS Web, you will see the reason why.
 9. Once completed, you need to delete the install/ directory from your web server.
 10. Go straight to the admin panel, navigate to site config. Configure the site.
 11. Go to Realms next, and for each realm you want users to use, you need to edit that realms DB information and turn "Site Enabled" from "Disabled" to "Enabled"

