# Experimental features

Enabling an experimental feature allows you to test a new feature under development before its official release.

Experimental features (also known as "feature flags") are aimed at experienced and adventurous users, who want to test a feature that is not yet stable enough for general use. Even though it sounds exciting, you should be aware of the risks of such experiments:

* Experimental features are still under development. Enabling them could therefore have unintended consequences and cause data loss.
* In any case, you never experiment in production.

### Enabling the experimental product page

The experimental product page is available on PrestaShop 1.7.8. This page benefits from increased performance and includes new features such as a new combination management system. It is a work in progress and some features are not available yet.

To make the experimental product page visible in your back office, enable the feature in **Advanced Parameters > Experimental Features** and save.

![](<../../../.gitbook/assets/image (43) (2).png>)

Then, go to **Catalog > Products**. You should notice some changes, specifically a new button: "New product on experimental page". Click on it to open the experimental product page.

You can also edit an existing product on the experimental page, by selecting this option in the hamburger menu in the Actions column of the product listing.

## New & Experimental features (PrestaShop 8.1)

{% hint style="info" %}
PrestaShop 8.1 features a new, reworked, [product page](../../selling/managing-catalog/new-product-page-prestashop-8.1.md).

To use this new product page, you must enable it in the **News & Experimental** page on PrestaShop 8.1.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (37) (3).png" alt=""><figcaption></figcaption></figure>

## PrestaShop 9 New Features

PrestaShop 9 introduces several major new features and improvements:

### New Admin API
PrestaShop 9 features a completely new **Admin API** powered by API Platform, providing:
- RESTful API endpoints for better integration with external systems
- Improved automation capabilities for store management
- Modern API design using JSON and REST standards
- Better developer experience for custom integrations

### Hummingbird Theme
A brand-new front office theme built with:
- Bootstrap 5 LTS for modern, consistent design components
- TypeScript and BEM CSS naming convention
- Improved performance and maintainability
- Support for dark mode and modern web standards

### Enhanced Product Management
- New product page interface in the back office
- Improved combination management system
- Better performance and user experience

### WebP and AVIF Support
- Native support for modern image formats
- Improved page loading performance
- Better SEO optimization

### Symfony 6.4 LTS
- Long-term support until November 2027
- Improved performance and security
- Modern PHP 8.1-8.4 compatibility
- Better developer tools and architecture

{% hint style="info" %}
These features are now stable in PrestaShop 9 and no longer require experimental feature flags to be enabled.
{% endhint %}
