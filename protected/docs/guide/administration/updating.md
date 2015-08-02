Updating
=========

If you are using custom themes or modules, please check the guides before updating.

## The Git Way

* First, backup ALL your files & database
* Pull latest Git files `git pull`
* Run `php /path/to/youbook/protected/yiic update`

## The Source/Download Way

* First, backup ALL your files & database
* Download the zip
* Delete current installation files (Backup? :-))
* Extract download package
* Restore from backup:
    - /path/to/youbook/uploads/file
    - /path/to/youbook/uploads/profile_image
    - /path/to/youbook/protected/runtime
    - /path/to/youbook/protected/config/local/_settings.php
    - /path/to/youbook/protected/modules
    - /path/to/youbook/themes (if any)
 Check file permissions (see [Installation](installation.md))
* Run `php /path/to/youbook/protected/yiic update`

## From 0.10.1 to 0.11.0
You may also need to run these commands to rebuild space, and user lists for the Directory
* Run `php /path/to/youbook/protected/yiic search_rebuild`
* Run `php /path/to/youbook/protected/yiic search_optimize`
