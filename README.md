squidaccess.log
===============

Show's on browser squid proxy logs as and when they are logged.

Step1:
Get HTML.py-0.04.zip from http://www.decalage.info/python/html and unzip it, copy HTML.py inside /usr/lib/pythonx.x/

Step2:
Put both the html1.py and squidaccess.sh scripts inside /var/scripts/ folder.

Step3: Create a cronjob entry.
/home/bala# crontab -l
*/1 * * * * /var/scripts/squidaccess.sh > /home/bala/html1error.txt 2>&1

Step4: Open a browser and hit on http://localhost/access.html
