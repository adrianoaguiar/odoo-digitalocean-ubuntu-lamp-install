# odoo-digitalocean-ubuntu-lamp-install
Automated Install Script For Odoo with SSH &amp; Reverse Proxy

## Basis
There are several odoo installation scripts out there, the two below was the basis for this one.
 * http://www.schenkels.nl/2015/01/install-odoo-v8-0-from-github-ubuntu-14-04-lts-formerly-openerp/
 * http://www.theopensourcerer.com/2014/09/how-to-install-openerp-odoo-8-on-ubuntu-server-14-04-lts/

This script is specific to the platform target described below. If the above scripts do not work for you, you can always try this one.

## Platform 
* Digital Ocean
 * Ubuntu 14.04 64-bit
 * LAMP Stack
 * Python (already preinstalled, but need to install modules required by Odoo)
* Odoo V8.0 (Github branch 8.0)
* Postgres 9.3

## Features
* Install & Setup server prerequisites (e.g. timezone, git, etc.)
* Securing The System
 * HTTPS & Reverse Proxy (optional)
 * Access to server via SSH key with passphrase (optional)
 * Disable Root on SSH (optional)
 * Create sudo user (for editing & running commands)
 * TBD - add fail2ban
* Create odoo system user
* Install postgres (no password, trust localhost), create an odoo postgres user and create the templatedb for the user
* Install Odoo via Github
* Install Odoo as a service
