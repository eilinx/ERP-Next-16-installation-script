# ERP-Next-16-installation-script

In order to use this you will need to have a clean install of Debian 13+ or Ubuntu 24.04+ server. You will a frappe-dedicated sudo-enabled account
(e.g. by performing):

```
sudo adduser [frappe-user]
usermod -aG sudo [frappe-user]
```

and then log in using the [frapp-user] above.
The rest is to execute:

```
wget https://raw.githubusercontent.com/abrefael/ERP-Next-16-installation-script/refs/heads/main/erp-next-installation-script.sh
sudo chmod +x erp-next-installation-script.sh
./erp-next-installation-script.sh
```

And follow the instructions on screen.
You will be prompted to:
1. Make sure your timezone is correct.
2. Supply passwords for your mariadb server root acount and for your site's admin account (select something complex enough, but a password you can remember...).
3. Your site name.
4. Your sudo password (the password that you gave your [frappe-user]).
Once you finish these steps, the script will perform it's magic and set you up.
You will have the options to:
- Install custom apps.
- Install ERPNext (experimental).
- Setup your server for production.
  
Caution! You will need to have your locale encoding set to UTF-8 in order to have you machine set for production.

Good luck! :-)
