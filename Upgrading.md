# Upgrading your MaNGOS Web
Note: Upgrading is only supported using version 4.1.0 and higher.  Anything prior is not supported due to unknown database modifications and non-existent functionality.
 1. Download the latest release from https://github.com/paintballrefjosh/MaNGOSWebV4/releases.
 2. Upload all of the directories and files to the existing MaNGOS Web folder on your webserver **EXCEPT** the "install/"  and "config/" directories.
 3. If you are upgrading from any version prior to 4.1.0 then you'll need to upload the "config/" directory as well and re-enter your database login information in config/config-protected.php 
 4. Open a browser to your site and you will be redirected to the automatic database updater script.
 5. Use!  MaNGOS Web is now ready to use.