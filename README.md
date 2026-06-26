# Kustom M2 Checkout

## Overview

`kustom/m2-checkout` is a metapackage for Magento 2 that orchestrates a comprehensive checkout
solution for e-commerce platforms. It aggregates multiple specialized modules designed to enhance
and streamline the checkout experience, payments processing, and order management within Magento 2.

## Purpose

This metapackage serves as a unified checkout ecosystem for Magento 2, combining the following key
functionalities:

- **Payment Processing**: Comprehensive payment methods support including Kustom and Kustom
  Checkout (KCO)
- **Order Management**: Advanced order line management and order status management
- **GraphQL Support**: GraphQL API endpoints for modern headless commerce implementations
- **Logging & Debugging**: Centralized logging for monitoring and troubleshooting
- **Admin Settings**: Customizable admin configuration panel for checkout features
- **API Integrations**: Plugin API support and Klarna API integrations
- **Sign-In Workflows**: Kustom Sign In With Klarna (SIWK) functionality
- **Knowledge Base System**: Kustom Service Support (KSS) module
- **Core Infrastructure**: Base modules for module support and interoperability

## Included Modules

The metapackage includes the following dependencies:

- `kustom/module-admin-settings` - Admin configuration
- `kustom/module-backend` - Backend services
- `kustom/module-base` - Base module utilities
- `kustom/module-kco` - Klarna Checkout integration
- `kustom/module-klarna-api` - Klarna API integration
- `kustom/module-kss` - Kustom Service Support
- `kustom/module-logger` - Logging utilities
- `kustom/module-orderlines` - Order line management
- `kustom/module-osm` - Order status management
- `kustom/module-payments-graph-ql` - GraphQL payment APIs
- `kustom/module-payments` - Payment processing
- `kustom/module-plugins-api` - Plugins API framework
- `kustom/module-siwk` - Sign In With Klarna
- `kustom/module-support` - Core support functionality

## Installation

This is a metapackage and should be installed via Composer as part of your Magento 2 project:

```bash
composer require kustom/m2-checkout
```

## Requirements

- Magento 2.x
- Composer
- Access to Magento Composer repository and Kustom GitHub repositories
