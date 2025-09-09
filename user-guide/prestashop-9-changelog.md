# PrestaShop 9 Changelog

This document provides a comprehensive overview of the new features, improvements, and changes introduced in PrestaShop 9.

## 🚀 Major New Features

### Admin API
PrestaShop 9 introduces a completely new **Admin API** powered by API Platform, replacing the legacy webservice system.

**Key Features:**
- **API Platform 3**: Built on the robust API Platform framework
- **OAuth2 Authentication**: Modern, secure authentication system
- **RESTful Design**: JSON-based API with standard HTTP methods
- **CQRS Architecture**: Command Query Responsibility Segregation pattern
- **Auto-generated Documentation**: Interactive API documentation at `/api/docs`
- **Granular Permissions**: Fine-grained access control with scopes
- **Rate Limiting**: Built-in protection against abuse

**Available Endpoints:**
- Products and catalog management
- Orders and customer management
- Module management
- Configuration settings
- Statistics and analytics

### Hummingbird Theme
A brand-new front office theme built with modern web technologies.

**Technology Stack:**
- **Bootstrap 5.2 LTS**: Latest Bootstrap framework
- **TypeScript**: Type-safe JavaScript development
- **BEM CSS Architecture**: Clean, maintainable CSS structure
- **Webpack**: Modern build system
- **Sass/SCSS**: CSS preprocessing

**Key Features:**
- **Performance Optimized**: Faster loading times and better Core Web Vitals
- **Mobile First**: Responsive design for all devices
- **Dark Mode Support**: Built-in dark theme capability
- **Accessibility**: WCAG 2.1 AA compliant
- **Modern Standards**: Follows current web development best practices

## 🛍️ Product Management Improvements

### New Product Page (Now Default)
The experimental product page from PrestaShop 8.1 is now the default interface.

**Technical Improvements:**
- **Symfony Migration**: Complete migration from legacy controllers
- **Twig Templates**: Replaced Smarty with modern Twig templating
- **Enhanced Performance**: Improved page loading and response times
- **Better Security**: Modern security practices and validation

**New Developer Hooks:**
- `displayAdminProductsOptionsStepTop`: Add content to Options tab top
- `displayAdminProductsOptionsStepBottom`: Add content to Options tab bottom
- `displayAdminProductsPriceStepBottom`: Add content to Price tab bottom
- `displayAdminProductsSeoStepBottom`: Add content to SEO tab bottom

**User Experience Enhancements:**
- **Improved Navigation**: Better tab organization and flow
- **Real-time Validation**: Instant feedback on form inputs
- **Better Error Handling**: Clear error messages and validation
- **Responsive Design**: Optimized for all screen sizes

### Enhanced Combination Management
- **Improved Generation**: Better combination generation interface
- **Bulk Operations**: Enhanced bulk editing capabilities
- **Filtering System**: Advanced filtering for large product catalogs
- **Pagination**: Better performance with large datasets

### Stock Management Improvements
- **Delta Quantity System**: Add/subtract stock quantities
- **Recent Stock Movements**: Preview of last 5 stock movements
- **Better Tracking**: Improved stock movement logging
- **Visual Indicators**: Color-coded stock status indicators

## 🔧 Technical Improvements

### Symfony 6.4 LTS
- **Long-term Support**: Support until November 2027
- **PHP 8.1-8.4 Compatibility**: Support for modern PHP versions
- **Performance Improvements**: Better caching and optimization
- **Security Enhancements**: Latest security patches and practices

### Modern Image Support
- **WebP Format**: Native support for WebP images
- **AVIF Format**: Support for next-generation AVIF format
- **Automatic Optimization**: Built-in image compression
- **Responsive Images**: Better mobile image handling

### Module Management
- **CQRS Commands**: Better module management with CQRS
- **Enhanced Tracking**: Improved module action logging
- **Better Notifications**: Enhanced module status notifications
- **Configuration Migration**: Automatic module configuration migration

## 🎨 Frontend Improvements

### Bootstrap 5 Compatibility
- **Bootstrap 5.2**: Latest Bootstrap framework
- **Compatibility Layer**: Support for Bootstrap 4 modules
- **Migration Tools**: Tools to help migrate from Bootstrap 4
- **Modern Components**: Updated UI components

### Performance Optimizations
- **Critical CSS**: Above-the-fold styles inlined
- **Lazy Loading**: Images and content loaded on demand
- **Code Splitting**: JavaScript bundles split for optimal loading
- **Asset Compression**: Minified and compressed files

### Accessibility Improvements
- **WCAG 2.1 AA**: Better accessibility compliance
- **Keyboard Navigation**: Enhanced keyboard support
- **Screen Reader Support**: Improved screen reader compatibility
- **Focus Management**: Better focus indicators

## 🔒 Security Enhancements

### Authentication & Authorization
- **OAuth2**: Modern authentication system for Admin API
- **Enhanced Permissions**: Granular access control
- **Token Management**: Secure token handling
- **Session Security**: Improved session management

### Data Protection
- **Input Validation**: Enhanced input validation
- **XSS Protection**: Better cross-site scripting protection
- **CSRF Protection**: Improved CSRF token handling
- **SQL Injection Prevention**: Enhanced database security

## 📊 Performance Improvements

### Core Performance
- **Faster Page Loading**: Optimized page rendering
- **Better Caching**: Improved caching strategies
- **Database Optimization**: Enhanced database queries
- **Memory Usage**: Reduced memory consumption

### Frontend Performance
- **Core Web Vitals**: Better Core Web Vitals scores
- **Image Optimization**: Automatic image optimization
- **CSS/JS Optimization**: Minified and compressed assets
- **CDN Ready**: Better CDN integration

## 🌐 Internationalization

### Translation Improvements
- **Better Translation System**: Enhanced translation management
- **Domain-based Translations**: Improved translation organization
- **Developer Tools**: Better tools for translators
- **Quality Assurance**: Improved translation quality checks

### Localization Features
- **RTL Support**: Better right-to-left language support
- **Currency Handling**: Enhanced currency management
- **Date/Time Formats**: Improved date and time formatting
- **Number Formats**: Better number formatting

## 🔌 Developer Experience

### Modern Development Tools
- **TypeScript Support**: Type-safe development
- **Modern Build Tools**: Webpack and modern tooling
- **Code Quality**: ESLint and Prettier integration
- **Testing Tools**: Enhanced testing capabilities

### API Development
- **RESTful API**: Modern API design
- **API Documentation**: Auto-generated documentation
- **SDK Support**: Better SDK development
- **Testing Tools**: API testing utilities

### Module Development
- **Enhanced Hooks**: New hooks for better integration
- **CQRS Support**: Better command/query separation
- **Form Integration**: Enhanced form handling
- **Validation Tools**: Better validation systems

## 🐛 Bug Fixes and Improvements

### Core Fixes
- **Memory Leaks**: Fixed various memory leak issues
- **Performance Issues**: Resolved performance bottlenecks
- **Security Vulnerabilities**: Patched security issues
- **Compatibility Issues**: Fixed browser compatibility problems

### UI/UX Improvements
- **Interface Polish**: Better user interface design
- **User Experience**: Improved user workflows
- **Error Handling**: Better error messages and handling
- **Responsive Design**: Enhanced mobile experience

## 📈 Migration and Upgrade

### From PrestaShop 8
- **Automatic Migration**: Most features migrate automatically
- **Legacy Support**: Temporary support for legacy features
- **Migration Tools**: Tools to help with migration
- **Documentation**: Comprehensive migration guides

### Breaking Changes
- **Legacy Webservice**: Replaced with Admin API
- **Bootstrap 4**: Modules may need updates for Bootstrap 5
- **Smarty Templates**: Some templates migrated to Twig
- **Legacy Controllers**: Some controllers migrated to Symfony

## 🔮 Future Roadmap

### Planned Features
- **Additional API Endpoints**: More API functionality
- **Enhanced Theme System**: More theme customization options
- **Performance Improvements**: Ongoing optimization
- **Security Enhancements**: Continuous security improvements

### Community Contributions
- **Open Source**: Continued open source development
- **Community Feedback**: Integration of community suggestions
- **Documentation**: Ongoing documentation improvements
- **Support**: Enhanced community support

## 📚 Resources

### Documentation
- **User Guide**: This comprehensive user guide
- **Developer Documentation**: [devdocs.prestashop-project.org](https://devdocs.prestashop-project.org/9/)
- **API Documentation**: Available at `/api/docs` in your store
- **Migration Guides**: Detailed migration documentation

### Support
- **Community Forums**: [prestashop.com/forums](https://www.prestashop.com/forums/)
- **GitHub**: [github.com/PrestaShop](https://github.com/PrestaShop)
- **Professional Support**: Available through PrestaShop partners
- **Training**: Official PrestaShop training programs

{% hint style="info" %}
PrestaShop 9 represents a significant step forward in e-commerce technology, providing merchants with modern tools and developers with a robust platform for building innovative solutions.
{% endhint %}
