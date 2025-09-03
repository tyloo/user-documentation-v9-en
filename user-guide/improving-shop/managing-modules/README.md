# Managing your Modules

PrestaShop comes with a set of modules that can be installed/uninstalled and configured as desired, in order to customize and complete your shop.

The range of actions is virtually unlimited: the extensibility of PrestaShop makes it possible to turn your shop into exactly what you intend it to do, instead of you having to comply with constraints that you did not choose – provided you can find the module that does exactly what you need.

This chapter contains the following sections:

* [Modules and Services](modules-and-services/)
* [Modules Catalog](broken-reference)

## PrestaShop 9 Module Management

PrestaShop 9 introduces significant improvements to module management:

### New CQRS Commands
- **Install Module Command**: Streamlined module installation process
- **Uninstall Module Command**: Improved module removal with better cleanup
- **Upgrade Module Command**: Enhanced upgrade process with better error handling
- **Toggle Module Status Command**: Quick enable/disable functionality
- **Reset Module Command**: Complete module reset to default state

### Enhanced Module Tracking
- **Action Logging**: All module actions (install, uninstall, upgrade) are now logged
- **Better Notifications**: Improved module status and update notifications
- **Configuration Migration**: Automatic module configuration migration during upgrades

### Improved Developer Experience
- **Module Configuration Feature**: Enhanced module configuration management
- **Better Error Handling**: More informative error messages and debugging
- **Hook Management**: Improved hook system for better module integration

The "Modules" section of the back office is currently being reworked. Changes are expected from PrestaShop 1.7.5 to the next minor versions, and that is why we would rather not document it right now but wait for the whole rework to be over. Don't panic, as we want it to remain intuitive, you probably won't need help!

![](<../../../.gitbook/assets/51839886 (7) (7) (6).png>)
