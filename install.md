# installation with composer

Minimal composer.json:

```
{
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/jgreidy/SmartyPaginate"
        }
    ],
    "require": {
        "smartypaginate/smartypaginate": "^1.7"
    }
}
```

SmartyPaginate contains plugins for Smarty. You can copy the plugins from
```
vendor/smartypaginate/smartypaginate/plugins 
```
into
```
vendor/smarty/smarty/libs/plugins
```
or you can do something like this:
```
$smarty->plugins_dir[] = 'vendor/smartypaginate/smartypaginate/plugins';
```