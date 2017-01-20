# Forum Integration
1. In v3, I have included some PHP classes (Not written by me, credits are in the php class files themselves), that will create forum accounts when a user logs into the site. If the account exists it will log the user in the forums as well. Please note that i was only able to test the phpBB3 bridge as I do not have vBulletin. But the vBulletin one should work just fine.
2. Go to your MaNGOSWeb Admin Control Panel -> Site Config. In the sub nav click "Forum Integration Settings"
3. You can only have ONE bridge enabled at a time!
4. For the forum path, you must enter the the PATH, not the URL! If the forum is NOT in the same htdocs or www folder as MangosWeb, then the bridge will not work!
5. To test if the bridge works, logout and try to log back in the site. If a white screen displays, or there is an error, then chances are your path is wrong. Don;t worry, you will still be logged in the site, but not in the forums.
6. I Cant guarantee results on the vBulletin bridge until users like yourself test it out. The phpBB3 bridge has been tested and works.