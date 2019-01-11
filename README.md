# PhpPsInfo

phppsinfo is a PHP script that allows you to test if your current environment fullfills PrestaShop's requirements, and offers suggestions for improvements.

This script allows you to quickly test the environement where you want to install PrestaShop.

The default credentials for displaying the results are:

* Login: prestashop
* Password: prestashop

You can set server env vars to override them:

* `PS_INFO_LOGIN`
* `PS_INFO_PASSWORD`


It tests:
	
* PHP & MySQL Version
* Apache modules
* PHP Extensions
* PHP Configuration
* MySQL Configuration
* Directories Configuration

