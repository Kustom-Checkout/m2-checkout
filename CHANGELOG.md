# Changelog

## 1.2.1 / 2026-08-10

### Affected packages

| Package                         | From   | To     |
|---------------------------------|--------|--------|
| kustom/module-kco               | 12.1.0 | 12.1.1 |
| kustom/module-base              | 11.1.0 | 11.1.1 |

### Breaking changes

* None

### Features / changes

* KUSTOM-6: Hyvä theme compatibility support.

### Fixes

* KUSTOM-46: Fix where product names and space cause problems with new Kustom module.

## 1.2.0 / 2026-06-26

### Affected packages

| Package                         | From    | To     |
|---------------------------------|---------|--------|
| kustom/module-admin-settings    | 1.1.4   | 1.2.0  |
| kustom/module-backend           | 11.0.18 | 11.1.0 |
| kustom/module-base              | 11.0.17 | 11.1.0 |
| kustom/module-kco               | 12.0.23 | 12.1.0 |
| kustom/module-klarna-api        | 1.0.8   | 1.1.0  |
| kustom/module-kss               | 3.0.17  | 3.1.0  |
| kustom/module-logger            | 3.0.9   | 3.1.0  |
| kustom/module-orderlines        | 3.0.17  | 3.1.0  |
| kustom/module-osm               | 4.0.17  | 4.1.0  |
| kustom/module-payments          | 10.0.19 | 10.1.0 |
| kustom/module-payments-graph-ql | 3.0.19  | 3.1.0  |
| kustom/module-plugins-api       | 1.0.6   | 1.1.0  |
| kustom/module-siwk              | 1.0.15  | 1.1.0  |
| kustom/module-support           | 3.0.15  | 3.1.0  |

### Breaking changes

* None

### Features / changes

* KUSTOM-92: Refactored push controller to rely a little less on exceptions for logic flows. Also
  removed logic to cancel orders on error since this isn't desired in the first place. Considering
  exceptions are anyway unreliable for logic flows this has huge risk of prematurely cancelling
  successfully placed orders. Applied similar changes also in confirmation controller.
* KUSTOM-93: Loosened up PHP version constraint to allow installing the packages on Magento 2.4.9
  and PHP 8.5. Adjusted integration and unit tests in the packages to run on currently supported
  Magento, PHP and PHPUnit versions.
* KUSTOM-94: Updated labels and strings from Klarna to Kustom in few places.

### Fixes

* KUSTOM-78: Fixed issue with shipping info API request passing incorrect request body when no tracking
  info is passed during capture
* KUSTOM-90: Updated workflow implementation to reset data on the workflow instance when new order
  id is set, to prevent existing data from causing issues for example in loops.

## 1.1.3 / 2026-04-30

* KUSTOM-52 Disable Sign in with Klarna (SIWK) - [DEPRECATED] - admin-settings:1.1.3
* KUSTOM-54 Fixed a type error that could cause checkout to fail when address prefill was used. - kco:12.0.21
* KUSTOM-55 Fixed an issue where no error message was shown when a Klarna API exception occurred - base:11.0.17
* KUSTOM-56 Fixed sanitization of merchant checkbox labels to preserve spaces and special characters - admin-settings:1.1.3
* KUSTOM-57 Cleanup leftover debugging code - backend:11.0.18
* KUSTOM-63 Fixed compatibility with PKSA-y2cr-5h3j-g3ys Security Advisory - siwk:1.0.15
* KUSTOM-68 Fixed guzzlehttp/guzzle compatibility for Magento versions earlier than 2.4.5 - base:11.0.17, klarna-api:1.0.8
* KUSTOM-76 Fix Shipping amount does not match for order between Kustom and Magento - kco:12.0.22
* [KUSTOM-58][KUSTOM-77][KUSTOM-82][KUSTOM-83][KUSTOM-84] Fix Orders instantly cancelled by api because of uncaught exceptions kco:12.0.22
* KUSTOM-88 DEPRECATED Hide/Disable Klarna Payments, On-Site Messaging and Express Checkout - admin-settings:1.1.4
* KUSTOM-20 Fix broken merchant portal link in order detail page - base:11.0.17
* KUSTOM-83 Fix Magento cancel status if klarna order is cancelled

## 1.1.2 / 2026-02-24

* KUSTOM-42 Removed obsolete "Client identifier" field from API credentials in admin configuration panel
* KUSTOM-49 Fixed critical error around logging address data into file when updating logged in user address
* KUSTOM-51 Changed the direct linking to Kustom's merchant portal on the admin panel
