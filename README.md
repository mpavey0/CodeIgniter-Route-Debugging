CodeIgniter-Route-Debugging
===========================

###Installation
####Copy file
Clone file to application/core/MY_Router.php

If you have [customized your application prefix](https://ellislab.com/codeigniter/user-guide/general/core_classes.html), edit:

1. the file name, replacing `MY` with your prefix
2. the class name inside the file, replacing `MY` with your prefix.

####Set logging threshold to debug
Open application/config/config.php and change the log threshold:

`$config['log_threshold'] = 2;`

###Log

All routes will be logged inside application/logs and will look like:

```
DEBUG --> Client sent : product/laptop
DEBUG --> Route found : product/(:any)  --> shop/view_product/$1
DEBUG --> Redirecting to : product/laptop  --> shop/view_product/laptop
```
