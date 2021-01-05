# PhpPsInfo - PrestaShop system requirements checker

![Screenshot](https://devdocs.prestashop.com/1.7/basics/installation/img/phppsinfo.jpg)

PhpPsInfo is a PHP script that allows you to test if your current environment fullfills PrestaShop's requirements, and offers suggestions for improvements.

This script allows you to quickly test the environement where you want to install PrestaShop.

The default credentials for displaying the results are:

* Login: prestashop
* Password: prestashop

You can set server env vars to override them:

* `PS_INFO_LOGIN`
* `PS_INFO_PASSWORD`


Tests include the following:
	
* PHP & MySQL Version
* Apache modules
* PHP Extensions
* PHP Configuration
* MySQL Configuration
* Directories Configuration

##  Usage

1. Download the [latest release](https://github.com/PrestaShop/php-ps-info/releases).
2. Extract the zip file.
3. Upload the `phppsinfo.php` file to your server and put it inside your current shop’s directory or the one where you intend to install it.
4. Open it up on your browser (`http://your-domain.com/path-to-your-prestashop/phppsinfo.php`).
5. Type in the login and password if prompted (use `prestashop` for both).
6. Enjoy!

## License

This tool is released under the MIT License.

## Troubleshooting

Working with a CGI environment such as Apache + FPM, you have to add a custom Apache RewriteCond.

```
RewriteCond %{HTTP:Authorization} .
RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]
```
