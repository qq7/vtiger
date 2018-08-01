vTiger CRM - Customer Relationship Management
=============================================

`vTiger`_ is a open source Customer Relationship Management application
with comparable functionality to SugarCRM and Salesforce.com, but with
more free features. It includes phone and e-mail integration, analysis
and reporting, customer support with self-service portal, and marketing
& sales automation for campaigns, lead generation, billing and inventory
management.

This appliance includes all the standard features in `TurnKey Core`_,
and on top of that:

- Vtiger configurations:
   
   - Installed from upstream source code to /var/www/vtigercrm
   - Deny access to Installation/migration interfaces by default
     (security).
   - Accept any hostname as the site URL.

   **Security note**: Updates to vTiger may require supervision so
   they **ARE NOT** configured to install automatically. See `vTiger
   documentation`_ for upgrading.

- SSL support out of the box.
- `Adminer`_ administration frontend for MySQL (listening on port
   12322 - uses SSL).
- Postfix MTA (bound to localhost) to allow sending of email from web
  applications (e.g., password recovery).
- Webmin modules for configuring Apache2, PHP, MySQL and Postfix.

Credentials *(passwords set at first boot)*
-------------------------------------------

-  Webmin, SSH, MySQL: username **root**
-  Adminer: username **adminer**
-  vTiger: username **admin**


.. _vTiger: https://www.vtiger.com/
.. _TurnKey Core: https://www.turnkeylinux.org/core
.. _Adminer: https://www.adminer.org/
.. _vTiger documentation: http://community.vtiger.com/help/vtigercrm/administrators/migration.html
