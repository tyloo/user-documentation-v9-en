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

PrestaShop 9 introduces several major new features and improvements that are now **stable and production-ready**:

### 🚀 New Admin API
PrestaShop 9 features a completely new **Admin API** powered by API Platform, providing:
- **API Platform 3**: RESTful API endpoints with modern architecture
- **OAuth2 Authentication**: Secure, modern authentication system
- **Auto-generated Documentation**: Interactive API docs at `/api/docs`
- **CQRS Architecture**: Better separation of concerns and performance
- **Granular Permissions**: Fine-grained access control with scopes
- **Rate Limiting**: Built-in protection against abuse

### 🎨 Hummingbird Theme
A brand-new front office theme built with modern technologies:
- **Bootstrap 5.2 LTS**: Latest Bootstrap framework for consistent design
- **TypeScript & BEM CSS**: Enhanced development with type safety and clean architecture
- **Performance Optimized**: Faster loading times and better Core Web Vitals
- **Dark Mode Support**: Built-in dark theme capability
- **Accessibility**: WCAG 2.1 AA compliant design
- **Mobile First**: Responsive design optimized for all devices

### 🛍️ Enhanced Product Management
- **New Product Page**: Now the default interface with Symfony migration
- **Enhanced Combination Management**: Improved generation and bulk operations
- **Delta Stock System**: Add/subtract stock quantities with better tracking
- **Real-time Validation**: Instant feedback on form inputs
- **New Developer Hooks**: Enhanced customization options for modules

### ⚡ Performance & Technology
- **Symfony 6.4 LTS**: Long-term support until November 2027
- **PHP 8.1-8.4 Compatibility**: Support for modern PHP versions
- **WebP and AVIF Support**: Native support for modern image formats
- **Critical CSS**: Above-the-fold styles inlined for faster rendering
- **Lazy Loading**: Images and content loaded on demand

### 🔒 Security Enhancements
- **Enhanced Authentication**: OAuth2 for Admin API
- **Better Input Validation**: Improved security practices
- **XSS Protection**: Enhanced cross-site scripting protection
- **Session Security**: Improved session management

{% hint style="success" %}
**All PrestaShop 9 features are now stable and production-ready.** No experimental feature flags are required - these features are the default experience in PrestaShop 9.
{% endhint %}

{% hint style="info" %}
For detailed information about these features, see the [PrestaShop 9 Changelog](../prestashop-9-changelog.md) and the [Admin API documentation](admin-api.md).
{% endhint %}
