1. Start by copying Virtual Host File 1010.conf to:

sudo cp 1010.conf /etc/apache2/sites-available/1010.conf


2. Copying Folder 1010 to:

sudo cp /1010 /var/www/


3. Enable Virtual Host File:

sudo a2ensite 1010.conf

FYI - disable the default site defined


4. Restart Apache:

sudo systemctl restart apache2


5. (optional) Open Local Hosts File:

sudo nano /etc/hosts


6. Add new rows:

127.0.0.1   	localhost
111.111.111.111 1010.dev
111.111.111.111 tenten.dev

FYI - 111.111.111.111 change to your VPS IP
