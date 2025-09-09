# Hummingbird Theme

PrestaShop 9 introduces **Hummingbird**, a brand-new front office theme that represents the next generation of PrestaShop themes. Built with modern web technologies and best practices, Hummingbird provides a solid foundation for creating fast, accessible, and beautiful online stores.

## Overview

Hummingbird is a modern theme built specifically for PrestaShop 9, designed to showcase the platform's capabilities while providing an excellent user experience. It serves as both a production-ready theme and a reference implementation for developers.

### Key Features

- **Bootstrap 5.2 LTS**: Built on the latest Bootstrap framework for modern, consistent design
- **TypeScript**: Enhanced JavaScript development with type safety
- **BEM CSS Architecture**: Clean, maintainable CSS using BEM naming convention
- **Performance Optimized**: Faster loading times and better Core Web Vitals
- **Mobile First**: Responsive design optimized for all devices
- **Dark Mode Support**: Built-in support for dark mode themes
- **Accessibility**: WCAG 2.1 AA compliant design
- **Modern Standards**: Follows current web development best practices

## Technology Stack

### Frontend Technologies
- **Bootstrap 5.2 LTS**: CSS framework for responsive design
- **TypeScript**: Type-safe JavaScript development
- **Webpack**: Modern build system for asset compilation
- **Sass/SCSS**: CSS preprocessing for better maintainability
- **BEM Methodology**: Block Element Modifier CSS naming convention

### Performance Features
- **Lazy Loading**: Images and content loaded on demand
- **Code Splitting**: JavaScript bundles split for optimal loading
- **Critical CSS**: Above-the-fold styles inlined for faster rendering
- **Modern Image Formats**: Support for WebP and AVIF images
- **Optimized Assets**: Minified and compressed CSS/JS files

## Design Philosophy

### Modern Aesthetics
Hummingbird embraces contemporary design trends while maintaining usability:

- **Clean Layout**: Minimalist design with focus on content
- **Typography**: Modern font choices with proper hierarchy
- **Color Scheme**: Carefully selected color palette for brand consistency
- **Spacing**: Generous whitespace for better readability
- **Visual Hierarchy**: Clear information architecture

### User Experience
- **Intuitive Navigation**: Easy-to-use menu structure
- **Fast Interactions**: Smooth animations and transitions
- **Clear CTAs**: Prominent call-to-action buttons
- **Search Optimization**: Enhanced search functionality
- **Checkout Flow**: Streamlined purchasing process

## Installation and Setup

### Prerequisites
- PrestaShop 9.0 or higher
- PHP 8.1 or higher
- Modern web server (Apache/Nginx)
- SSL certificate (recommended)

### Installation Steps

1. **Download the Theme**
   - Hummingbird is included with PrestaShop 9
   - Located in `/themes/hummingbird/` directory

2. **Activate the Theme**
   - Go to **Design > Theme & Logo**
   - Select **Hummingbird** from available themes
   - Click **"Use this theme"**

3. **Configure Theme Settings**
   - Access theme configuration in **Design > Theme & Logo**
   - Customize colors, fonts, and layout options
   - Upload your logo and favicon

### Initial Configuration

After installation, configure the following:

1. **Logo and Branding**
   - Upload your store logo
   - Set brand colors
   - Configure favicon

2. **Layout Settings**
   - Choose homepage layout
   - Configure product page layout
   - Set up category page display

3. **Performance Settings**
   - Enable image optimization
   - Configure lazy loading
   - Set up caching options

## Customization Options

### Color Customization
Hummingbird provides extensive color customization:

- **Primary Colors**: Brand colors for buttons and links
- **Secondary Colors**: Supporting color palette
- **Background Colors**: Page and section backgrounds
- **Text Colors**: Headings, body text, and links
- **Accent Colors**: Highlights and special elements

### Typography
- **Font Families**: Choose from web-safe fonts or custom fonts
- **Font Sizes**: Responsive typography scale
- **Line Heights**: Optimized for readability
- **Font Weights**: Multiple weight options

### Layout Options
- **Header Layout**: Choose from different header styles
- **Footer Layout**: Configure footer content and layout
- **Product Grid**: Customize product listing display
- **Sidebar**: Enable/disable sidebar on different pages

## Performance Optimization

### Built-in Optimizations
Hummingbird includes several performance optimizations:

- **Critical CSS**: Above-the-fold styles inlined
- **Lazy Loading**: Images loaded as needed
- **Code Splitting**: JavaScript split into chunks
- **Asset Compression**: Minified CSS and JavaScript
- **Image Optimization**: Automatic image compression

### Additional Optimizations
To further improve performance:

1. **Enable Caching**
   - Configure browser caching
   - Set up server-side caching
   - Use CDN for static assets

2. **Optimize Images**
   - Use WebP format when possible
   - Compress images before upload
   - Implement responsive images

3. **Minimize HTTP Requests**
   - Combine CSS and JavaScript files
   - Use CSS sprites for icons
   - Enable HTTP/2

## Mobile Experience

### Responsive Design
Hummingbird is built with a mobile-first approach:

- **Breakpoints**: Optimized for all screen sizes
- **Touch-Friendly**: Large touch targets for mobile
- **Fast Loading**: Optimized for mobile networks
- **Offline Support**: Basic offline functionality

### Mobile Features
- **Swipe Navigation**: Touch gestures for navigation
- **Mobile Menu**: Collapsible navigation menu
- **Touch Optimized**: Buttons and links sized for touch
- **Fast Checkout**: Streamlined mobile checkout

## Accessibility Features

### WCAG 2.1 AA Compliance
Hummingbird meets accessibility standards:

- **Keyboard Navigation**: Full keyboard accessibility
- **Screen Reader Support**: Proper ARIA labels
- **Color Contrast**: Sufficient contrast ratios
- **Focus Indicators**: Clear focus states
- **Alt Text**: Proper image descriptions

### Accessibility Tools
- **Skip Links**: Quick navigation for screen readers
- **Focus Management**: Proper focus handling
- **ARIA Labels**: Descriptive labels for elements
- **Semantic HTML**: Proper HTML structure

## Browser Compatibility

### Supported Browsers
Hummingbird supports modern browsers:

- **Chrome**: Version 90+
- **Firefox**: Version 88+
- **Safari**: Version 14+
- **Edge**: Version 90+
- **Mobile Browsers**: iOS Safari, Chrome Mobile

### Graceful Degradation
- **Progressive Enhancement**: Works without JavaScript
- **Fallbacks**: CSS fallbacks for modern features
- **Polyfills**: Support for older browsers when needed

## Developer Features

### Theme Structure
```
hummingbird/
├── assets/
│   ├── css/
│   ├── js/
│   └── images/
├── templates/
│   ├── layouts/
│   ├── components/
│   └── pages/
├── translations/
└── config/
```

### Customization Hooks
Hummingbird provides numerous hooks for customization:

- **Header Hooks**: Customize header content
- **Footer Hooks**: Modify footer elements
- **Product Hooks**: Extend product pages
- **Category Hooks**: Customize category listings
- **Checkout Hooks**: Modify checkout process

### Development Tools
- **Webpack**: Modern build system
- **TypeScript**: Type-safe development
- **Sass**: CSS preprocessing
- **ESLint**: Code quality tools
- **Prettier**: Code formatting

## Migration from Classic Theme

### Compatibility Considerations
When migrating from the Classic theme:

1. **Bootstrap Version**: Classic uses Bootstrap 4, Hummingbird uses Bootstrap 5
2. **CSS Classes**: Some CSS classes may have changed
3. **JavaScript**: jQuery dependencies may need updates
4. **Modules**: Some modules may need updates for Bootstrap 5

### Migration Steps
1. **Backup**: Create a full backup of your store
2. **Test Environment**: Test migration in a staging environment
3. **Module Compatibility**: Check module compatibility
4. **Custom CSS**: Update custom CSS for Bootstrap 5
5. **Testing**: Thoroughly test all functionality

### Bootstrap 5 Compatibility
For modules built with Bootstrap 4:

- **Compatibility Layer**: Use the Bootstrap 4 compatibility layer
- **CSS Updates**: Update CSS classes to Bootstrap 5
- **JavaScript Updates**: Update JavaScript for Bootstrap 5
- **Testing**: Test all module functionality

## Best Practices

### Performance
- **Optimize Images**: Use appropriate image formats and sizes
- **Minimize Plugins**: Only use necessary modules
- **Enable Caching**: Configure proper caching strategies
- **Monitor Performance**: Use tools to monitor site performance

### SEO
- **Meta Tags**: Ensure proper meta tag implementation
- **Structured Data**: Use schema markup for products
- **URL Structure**: Maintain clean, SEO-friendly URLs
- **Page Speed**: Optimize for Core Web Vitals

### Maintenance
- **Regular Updates**: Keep theme and modules updated
- **Backup Strategy**: Implement regular backup procedures
- **Security**: Keep PrestaShop and modules secure
- **Monitoring**: Monitor site performance and errors

## Troubleshooting

### Common Issues

**Theme Not Loading**
- Check file permissions
- Verify theme files are complete
- Clear cache and compiled assets

**Styling Issues**
- Check for CSS conflicts
- Verify Bootstrap 5 compatibility
- Clear browser cache

**JavaScript Errors**
- Check browser console for errors
- Verify module compatibility
- Update outdated modules

### Getting Help
- **Documentation**: Refer to theme documentation
- **Community**: Join PrestaShop community forums
- **Developer Resources**: Check developer documentation
- **Professional Support**: Contact PrestaShop for support

## Future Development

### Roadmap
Hummingbird is actively developed with planned improvements:

- **Additional Layouts**: More layout variations
- **Enhanced Customization**: More customization options
- **Performance Improvements**: Ongoing optimization
- **New Features**: Additional functionality

### Contributing
- **Bug Reports**: Report issues on GitHub
- **Feature Requests**: Suggest new features
- **Code Contributions**: Contribute to theme development
- **Documentation**: Help improve documentation

{% hint style="info" %}
Hummingbird represents the future of PrestaShop theming. It's designed to be fast, accessible, and maintainable while providing a solid foundation for custom development.
{% endhint %}
