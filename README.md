This is the COLORS lab application for COP4331. Once logged in, it allows users to 
maintain a database of colors that they can add to, and search from. These functions 
are handled through API endpoints.

It uses the LAMP stack. A combination of Linux (ubuntu 24), Apache, MySQL, and PHP.

Want to run this?

DigitalOcean: Create a LAMP stack droplet, it is pre-configured exactly as needed 
with exact firewall settings, apache, and mySQL installations. Place this folder into 
the web root (typically ../var/www/html/). Otherwise you can clone this repository
directly into your root (check github instructions). Next run mySql in the terminal and 
set up database as COP4331. Create tables for Users and Colors, with appropriate 
fields and keys. Save and exit.

After this, it should be running. Domains can be used by adding the Droplet's IPv4
address as a DNS record in your domain manager (GoDaddy, PorkBun, etc). If not, check 
firewall rules and make sure Apache is listed.

Limitations:
This service is not secure. It unfortunately uses http, not https. It's also susceptible 
to client data manipulation (for example, setting UserID from F12 inspector).

Changes:
Frontend is now styled, with nice colors.
MySQL database present and tables created appropriately.
API endpoints present and working.
Frontend javascript correctly calls these endpoints.

Created by Nathan Melloul. No AI usage in this project.