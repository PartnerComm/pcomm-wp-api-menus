# PartnerComm WordPress Menu API

This WordPress plugin in creates an API to access menus within the WordPress JSON API.

## Installation

##### Composer Install
Add the plugin to the list of repositories.
```    
{
    "type": "vcs",
    "url": "https://github.com/PartnerComm/pcomm-wp-api-menus.git"
}
```
Add the plugin to the list of required packages.
```
    "pcomm/pcomm-wp-api-menus": "1.0.*"
```

##### Traditional Install
Upload this `pcomm-wp-api-menus` folder and it's contents to your Wordpress plugins directory.

##### Activate the Plugin
Activate the plugin through the 'Plugins' menu in WordPress.

## Using the Menu API

This menu API allows you to make GET requests to the following endpoints:

##### All menus
`wp-json/wp/v2/menus`
___
##### A specific menu
`wp-json/wp/v2/menus/{menu}` 
___
##### All theme locations and their menus
`wp-json/wp/v2/menus/theme-locations`
___
##### A specific theme location's menu
`wp-json/wp/v2/menus/theme-locations/{location}` 
___

## Release Notes
* 1.0.0 : initial commit and release
