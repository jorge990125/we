# Setting up Remote Access

 1. To setup remote access to your server, you must have it enabled in your server config. Its best to have it look like this

```
  Console.Enable = 1
  Ra.Enable = 1
  Ra.IP = 0.0.0.0
  Ra.Port = 3443
  Ra.MinLevel = 3
  Ra.Secure = 1
  Ra.Stricted = 0
  SOAP.Enabled = 1
  SOAP.IP = 0.0.0.0
  SOAP.Port = 7878
```
 2. Next you need to create an account to be the remote access "bot" account. I found that with mangos especially, you need to create this account either A) Through the server console B) Through the site, then going into the DB and uppercasing the whole username... EX: test -> TEST.
 3. Go into the ACP -> Realms -> your realm name. Scroll down to the bottom where it says "Remote Access"
 4. Enter your information. the account name DOES NOT need to be in caps :)