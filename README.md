# PhpPsInfo

phppsinfo provides a way to reports PrestaShop Requirements information about the PHP/MySQL/Apache environment, and offers suggestions for improvement. 

This script allow you to quickly test your environement, where you want to install PrestaShop.
The default credentials for display the result are :

* Login : prestashop
* Password : prestashop

You can set server env vars to override informations:

* `PS_INFO_LOGIN`
* `PS_INFO_PASSWORD`


It tests:
	
* PHP & MySQL Version
* Apache modules
* PHP Extensions
* PHP Configuration
* MySQL Configuration
* Directories Configuration

