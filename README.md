## Elementor Addons & Templates - Sizzify Lite - v.1.2.7 / Nov 27, 2018 (installed)

## WordPress plugin

This is a copy of the code downloaded from the WordPress plugin repository and uploaded herr for patching. This plugin is no longer available for download:

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

## Patches

This plugin snapshot has been uploaded in order to patch incompatibilities with Elementor 3.4.7, arising from changes in the namespacing.

This affects the following files:

1. elementor-extra-widgets/widgets/elementor/posts-grid.php
1. elementor-extra-widgets/widgets/elementor/pricing-table.php
1. elementor-extra-widgets/widgets/elementor/services.php
1. themeisle-content-forms/class-themeisle-content-forms-elementor.php
