DoulCi-server2
==============

The new leak from w0rm
Cross-platform compatible: Works on Windows, Linux, and Android.

What is: Apple Albert alternative, useful for making your own activation server (for Activation Lock Bypass, for example).  

## Installation Instructions

### Windows (XAMPP)
1. Put files to htdocs folder in XAMPP
2. Edit hosts file (C:\Windows\System32\drivers\etc\hosts) and add line: `127.0.0.1 albert.apple.com`
3. Start Apache from XAMPP control panel

### Linux
1. Install Apache and PHP with OpenSSL support:
   ```bash
   sudo apt-get update
   sudo apt-get install apache2 php php-openssl
   ```
2. Copy files to web root (typically /var/www/html/)
3. Edit /etc/hosts and add line: `127.0.0.1 albert.apple.com`
4. Restart Apache: `sudo service apache2 restart`

### Android (Termux)
1. Install Termux from F-Droid or Play Store
2. Install required packages:
   ```bash
   pkg update
   pkg install php apache2 openssl
   ```
3. Copy files to Apache document root
4. Edit hosts file (requires root): `su -c "echo '127.0.0.1 albert.apple.com' >> /etc/hosts"`
5. Start Apache server

## Additional Notes
If you want to fix iTunes error (0x8XXXX) - install fiddler2 with fake RootCA.
Only for advanced users who know about RSA.
Fixed all errors. DO NOT WORK WITHOUT TRUE CERTS.
For entertainment purposes only.


