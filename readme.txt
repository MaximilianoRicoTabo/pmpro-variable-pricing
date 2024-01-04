=== Paid Memberships Pro - Variable Pricing Add On ===
Contributors: strangerstudios
Tags: paid memberships pro, pmpro, membership, donate, donations, charity, charities
Requires at least: 5.2
Tested up to: 6.4
Stable tag: 0.4.6

Allow customers to set their own price when checking out for your membership levels.

== Description ==
This plugin requires Paid Memberships Pro.

== Installation ==

1. Upload the `pmpro-variable-pricing` directory to the `/wp-content/plugins/` directory of your site.
1. Activate the plugin through the 'Plugins' menu in WordPress.
1. Edit the levels you want to add variable pricing to and set the "Variable Pricing" settings.

== Frequently Asked Questions ==

= I found a bug in the plugin. =

Please post it in the issues section of GitHub and we'll fix it as soon as we can. Thanks for helping. https://github.com/strangerstudios/pmpro-variable-pricing/issues

== Changelog ==
= 0.4.6 - 2024-01-04 =
* ENHANCEMENT: Updating `<h3>` tags to `<h2>` tags for better accessibility. #44 (@ipokkel)
* BUG FIX: Fixed PHP warning if an empty level ID is passed to `pmprovp_get_settings()`. #43 (@dparker1005)
* REFACTOR: No longer pulling the checkout level from the `$_REQUEST` variable. #43 (@dparker1005)
* REFACTOR: Now using `get_option()` instead of `pmpro_getOption()`. #42 (@JarrydLong)

= 0.4.5 - 2023-01-30 =
* ENHANCEMENT: Improved translation logic within the plugin and translated some missing strings.
* ENHANCEMENT: Updated French translation (@paullaffitte).
* BUG FIX: Fixed an issue where PHP sessions were interfering with the REST API.

= .4.4 - 2020-04-09 =
*  BUG FIX: Fixed issue where non variable pricing levels would still be able to adjust the price via query parameters.

= .4.3 =
* SECURITY: Escape and sanitization of strings.
* ENHANCEMENT: Show inline-warning if criteria is not met for variable pricing.
* ENHANCEMENT: Support right-handed currency symbol positioning.
* BUG FIX: Fixed issue where JavaScript would load on pages that did not have the variable pricing input enabled.

= .4.2 =
* BUG FIX: Fixed fatal error crash when PMPro is not activated.
* BUG FIX: Fixed issue where the variable price was not being loaded from SESSION for PayPal Express and other offsite gateways.

= .4.1 =
* ENHANCEMENT: French translation files. (Thanks, Alfonso Sánchez Uzábal)
* ENHANCEMENT: Consistent plugin titles and URLs
* ENHANCEMENT: WordPress Coding Standards

= .4 =
* BUG FIX: Allow blank variable price input (i.e. use the minimum price)
* BUG FIX/FEATURE: Fixed logic for hiding/showing billing fields if the price is free or not.
* FEATURE: Properly formatted translatable text
* FEATURE: Added translation domain labels
* FEATURE: Added language file load (when applicable)
* FEATURE: Added suggested price setting.
* FEATURE: No longer embedding JS in frontend sources/page.
* FEATURE: Priority of JS register/enqueue operation means you can unhook the Variable Prices JavaScript if needed

= .3.1 =
* BUG: Now hiding Variable Pricing options on checkout review page.

= .3 =
* Now storing price in session for offsite gateways like PayPal and 2Checkout.

= .2 =
* Updated JS logic to hide/show billing to work for PayPal, PayPal Express, and Stripe (with no billing fields) gateway options.
