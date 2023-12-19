Requirements
------------

System requirements for AsonetCMS are modest, so every modern server should suffice.

+ Apache 2.2+ with `mod_rewrite`
+ PHP version 7.4+
+ MySQL 5.6+

PHP configuration must have the following extensions:

+ git
+ gd
+ mbstring
+ zip
+ cURL
+ simplexml
+ json


Installation
------------

Extract all files from the compressed package and then transfer them to the local directory or remote server. In the case of a remote server, connect to it via a (S)FTP client, such as the free [FileZilla](https://filezilla-project.org) program. Usually, files should be uploaded to `www`, `htdocs` or `public_html` - if you are not sure about it ask your hosting provider please.

**Warning!** Make sure the `.htaccess` file is also on the server. Without it the CMS will not work.

Some servers may require additional permissions `chmod 777` for the following directories and files:

+ uploads/

Go to _(Your domain)/install_
1. Fill out the database credentals.
2. Fill out authorization credentals.
3. After that you maybe **required** to login after installation.

Configuration
-------------

CMS can be configured by editing the settings in the dashboard panel.

### Administration panel
To change the basic configuration in the admin panel, select the `Admin > Config` tab. From here You can enter and save all needed settings.

If you want to change templates, which should only be done by experienced admins, you can use the integrated _File Manager_.


Update
------

If you want to keep up to date with all the latest news, bug fixes and security issues, you should regularly check ASONET-CMS homepage. System updates can be done automatically via the admin backend. Your hosting should support Git because our updates come from our GitHub repository.

In case of complications you can always ask us about it at our support forums or via our ticket system.

Before each update, you should always do a file and database backup. If an update has failed, you can restore it at any time.


More to come soon.
