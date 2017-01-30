You can view a live copy of the latest version used for testing by visiting **www.mistvale.com**.

# Setting the Donation System
1. If you dont already, create a premier paypal account. (It's free http://www.paypal.com)
2. From the PayPal menu, go to Profile > More Options > Under selling Preferences > Instant Payment Notification Preferences.
3. Select Instant notification
4. Enter the full path including your domain name to ipn.php in the root of your
MaNGOS directory.
Example: http://you-domain-or-ip/ipn.php
5. In the MaNGOSWeb Admin Control Panel -> Site Config. Make sure you have the paypal email address set!
6. To test using sandbox: 
A) open 'ipn.php' and edit line 21: "$Paypal->testMode(FALSE);" set the FALSE to TRUE.
B) Go to https://developer.paypal.com and create a developer account
C) click "Simulate Instant Payment Notification"
D) Click "eCheck Complete" and then Enter some random information and hit send
E) You should get confirmation that the data was sent
F) Check you DB "mw_donate_transactions" and you should see your test IPN there. If not then check the IPN Log "core/logs/ipn.txt" 
NOTE: Paypal sandbox has been really buggy lately. But i have tested the donation system myself over and over since re-writting it with no errors at all ;)