# Built-in server debugging with PhpStorm on Ubuntu
The deffinitive guide for say goodbay to var_dump(), dump(), echo, dd(), etc...
### Install and configure Xdebug
- Installing
```sh
$ sudo apt-get install php-xdebug
```
- In order to check if has been installed run:
```sh
$ php -v
```
You should see your Php Version and: <br />
'with Xdebug v2.5.5, Copyright (c) 2002-2017, by Derick Rethans'

- Locate xdebug.ini configuration file:
```sh
$ php --ini | grep xdebug
```
- Edit the file and add these lines:
> xdebug.remote_enable=on <br />
> xdebug.remote_connect_back=on

Php settings ready!

### Set Up your browser
- Add this extension [Xdebug Helper](https://chrome.google.com/webstore/detail/xdebug-helper/eadndfjplgieldjbigjakmdgkmoaaaoc?utm_source=chrome-app-launcher-info-dialog) to enable/disable debugging on your browser.
- Right click on the bug icon and set PhpStorm IDE key
- Click on the bug to enable

### Debugging With PhpStorm
- Enable/disable debug:
![N|Solid](https://raw.githubusercontent.com/mjgr0013/built-in-server-xdebug-with-phpstorm/master/Phone.png)

Now add a breakpoint at any file and reload the browser, PhpStorm should ask you for start debugging and may stop at the breakpoint.
