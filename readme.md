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

## Theme Use
To output a menu in the theme, for PHP rendering in a component, we've created the following helper functions.

#### Get menu by name
```
if (function_exists('pcomm_wp_api_menu_by_name')): 
    echo pcomm_wp_api_menu_by_name('primary-navigation'); 
endif;
```

#### Get menu by location
```
if (function_exists('pcomm_wp_api_menu_by_location')): 
    echo pcomm_wp_api_menu_by_location('primary'); 
endif;
```

## Release Notes
* 1.0.1 : adds theme helper functions for outputting specific menus
* 1.0.0 : initial commit and release
