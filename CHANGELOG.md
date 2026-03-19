1.1.3 / 2026-03-19
==================

  * KUSTOM-52 Disable Sign in with Klarna (SIWK) - [DEPRECATED] - admin-settings:1.1.3
  * KUSTOM-54 Fixed a type error that could cause checkout to fail when address prefill was used. - kco:12.0.21
  * KUSTOM-55 Fixed an issue where no error message was shown when a Klarna API exception occurred - base:11.0.17
  * KUSTOM-56 Fixed sanitization of merchant checkbox labels to preserve spaces and special characters - admin-settings:1.1.3
  * KUSTOM-57 Cleanup leftover debugging code - backend:11.0.18
  * KUSTOM-63 Fixed compatibility with PKSA-y2cr-5h3j-g3ys Security Advisory - siwk:1.0.15
  * KUSTOM-68 Fixed guzzlehttp/guzzle compatibility for Magento versions earlier than 2.4.5 - base:11.0.17, klarna-api:1.0.8

1.1.2 / 2026-02-24
==================

  * KUSTOM-42 Removed obsolete "Client identifier" field from API credentials in admin configuration panel
  * KUSTOM-49 Fixed critical error around logging address data into file when updating logged in user address
  * KUSTOM-51 Changed the direct linking to Kustom's merchant portal on the admin panel
    fix type error that could break checkout when the address pre-fill was used
