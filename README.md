# Elementor Addons & Templates - Sizzify Lite - v.1.2.7 / Nov 27, 2018 (installed)

## WordPress plugin

This is a copy of the code downloaded from the WordPress plugin repository and uploaded here for patching. This plugin is no longer available for download:

> This plugin has been closed as of August 31, 2020 and is not available for download. This closure is permanent. Reason: Author Request.
>
> https://wordpress.org/plugins/elementor-addon-widgets/

## Github repositories

The source code of this plugin is available at https://github.com/Codeinwp/elementor-addon-widgets (v1.3.2 / Apr 19, 2019 - no longer maintained - Public Archive).

This plugin also uses several dependencies from the original developer. These dependencies are still under active development.

Version 1.2.7 of this plugin required the following versions of these dependencies (source: composer/installed.json):

1. `"codeinwp/elementor-extra-widgets": "dev-master#a1fc5d0bff05594e717c72217b1b3444c7b1bae5",` (v1.0.3 / Jul 28, 2018) 
2. `"codeinwp/themeisle-content-forms": "dev-master#60f64fa4bb1d6941937bf45da2420d427cc6183f",` (v1.2.0 / Nov 12, 2018)
3. `"codeinwp/themeisle-sdk": "dev-master#951cde6e799e00d46a52416b62221fd771ddc326",` (Nov 27, 2018)
4. `"codeinwp/templates-directory": "dev-master#be218b189f9dc60e32463161567ca1b567f79019"`(Nov 12, 2018)

A simple update of `composer.json` as above is not possible as it results in changes in the versions of sub-dependencies. This could introduce side-effects which would be difficult to troubleshoot.

Therefore these dependencies have been baked into this repository at the listed versions.

## Patches

This plugin snapshot has been uploaded in order to patch incompatibilities with Elementor 3.4.7, arising from changes in the namespacing.

This affects the following files which have been patched here:

1. elementor-extra-widgets/widgets/elementor/posts-grid.php
1. elementor-extra-widgets/widgets/elementor/pricing-table.php
1. elementor-extra-widgets/widgets/elementor/services.php
1. themeisle-content-forms/class-themeisle-content-forms-elementor.php

---

# Elementor Addons & Templates - Sizzify Lite #
**Contributors:** [themeisle](https://profiles.wordpress.org/themeisle), [codeinwp](https://profiles.wordpress.org/codeinwp)  
**Tags:** elementor, elementor addons, page builder template, page builder templates, woocommerce, template builder, builder templates  
**Requires at least:** 4.4    
**Tested up to:** 4.9  
**License:** GPLv3  
**License URI:** https://www.gnu.org/licenses/gpl-3.0.html     

## Description ##
Adds new Addons & Widgets that are specifically designed to be used in conjunction with the [Elementor Page Builder](https://wordpress.org/plugins/elementor/).

Initial version contains 6(+2) widgets - more to come.
* 1: WooCommerce Product Categories
* 2: WooCommerce Recent Products   
* 3: WooCommerce Best Selling Products   
* 4: WooCommerce Featured Products   
* 5: WooCommerce On Sale Products   
* 6: WooCommerce Popular Products
* 7: New: EAW: Elementor Widget Recent Posts
* 8: New: EAW: Elementor Posts By Category

Elementor Native Widgets.
* 9:  New: EAW Posts Grid
* 10: New: EAW Pricing Table
* 11: New: EAW Services
	
## Themes ##
Minimal support is included for almost any theme therefore leaving most of the design to be carried out in the themes themselves.
Elementor Addons & Widgets does however inherit some design aspects of the current theme.

If you are a theme author you are encouraged to test the plugin making necessary adjustments and providing design options where necessary, there is a list of 20+ Best Elementor themes here: [here](https://www.codeinwp.com/blog/elementor-themes-templates/).

If you find any issues with your particular theme not playing nice with the templates please let us know so that we can do our best
to accommodate you.

## Installation ##
* These instructions assumes you already have a WordPress site and the Elementor plugin installed and activated.

1. Install using the WordPress built-in Plugin installer, or Extract the zip file and drop the contents in the `wp-content/plugins/` directory of your WordPress installation.
2. Activate the plugin through the 'Plugins' menu in WordPress.
3. Go to Pages > Add New
4. Select the desired template from the Page Attributes section
4. Press the 'Edit with Elementor' button.
5. Scroll down the left pane to the WordPress section and you should see the new widgets that you can drag and drop on to your page.

## Frequently Asked Questions ##

Why is it after dragging the required widget, making the necessary adjustments to settings and save the layout goes all wonky?

There is a known bug/conflict with WooCommerce assets not being loaded upon saving the edits, however refreshing the page puts things back to normal.
See this [issue #495](https://github.com/pojome/elementor/issues/495) for current status.

## Screenshots ##

1. Widgets Panel

2. Editor View

3. Frontend View Products And Posts

4. Frontend view posts with custom title.

## Changelog ##
### 1.2.7 - 2018-11-27  ###

* Update recommended theme link


### 1.2.6 - 2018-11-12  ###

* Fix issue with elementor content forms php notice
* Security fixes
* Performance enhancements
* Add notice to awesome Neve theme


### 1.2.5 - 2018-07-26  ###

* Development


### 1.2.4 - 2018-07-23  ###

* Add new controls for Elementor content forms.


### 1.2.3 - 2018-07-11  ###

* Version bump.


### 1.2.2 - 2018-07-11  ###

* Added styling options for elementor form widgets


### 1.2.1 - 2018-07-06  ###

* Fixes post grid pagination issue
* Fixes post grid colors not applying correctly
* Fixes Templates directory import issue
* Fixes content forms placeholder not used
* New templates in the templates directory


### 1.2.0 - 2018-03-29  ###

* Adds support for the premium version.
* Adds automatic page templates synchronization.
* Adds support for future extra-widgets and add-ons.


### 1.1.7 - 2018-03-29  ###

* Development


### 1.1.6 - 2018-03-29  ###

* Rebranded plugin to Sizzify


### 1.1.5 - 2018-02-08  ###

* Added Template Directory [under Pages > Template Directory]
* Added new Content Forms widgets
* A more modular structure


### 1.1.4 - 2017-12-18  ###

* Fixed Pricing Table Widget button link issue
* Fixed Post Grid Widget notice.
* Fixed Services Widget content align.


### 1.1.3 - 2017-11-17  ###

* Fixed javascript error on front end.


### 1.1.2 - 2017-11-16  ###

* Added three new Elementor native widgets.
* Tested up to 4.9


### 1.1.1 - 2017-10-11  ###

* Updated title and description
* Updated tested up to version 4.8


### 1.1.0 - 2017-09-29  ###

* Travis trigger.
* Added Themeisle SDK.
* Added Continuous Integration.
* Changed contributors.


### 1.0.4 ###
* Name change due to stipulation on Elementor's Terms and Conditions
* Adjustments made to plugin and author urls

### 1.0.3 ###
* FIXED: Fatal error clash with Storefront on checking if WooCommerce is active.

### 1.0.2 ###
* New: Recent Posts By Category
* Tweaks: CSS adjustments so that widget title when set does not break column layout

### 1.0.1 ###
* New: Recent Posts Widget

### 1.0.0 ###
* Initial release.

