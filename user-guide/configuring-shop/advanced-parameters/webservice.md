# Webservice

In this page, you can enable your shop's webservice, so that third-party tools can access your data. This potentially makes it possible for interesting tools to help you or your customers make better use of your shop (such as mobile applications).

A web service is a method of communication between two electronic devices over a network. It relies on a known set of methods, formats, and access rights, so as be able to use the webservice's content on any other authorized tool and build upon the original content. Read more about it on Wikipedia: [http://en.wikipedia.org/wiki/Web\_service](http://en.wikipedia.org/wiki/Web\_service).

The page starts by listing the currently existing webservice keys in a table if there are any. A webservice key is a unique access that you grant to a developer, which can be used to tie a tool to your shop. Share them sparingly, as you might not always want everyone to access your data.

<figure><img src="../../../.gitbook/assets/image (1) (3).png" alt=""><figcaption></figcaption></figure>

Not any app can access your shop through the PrestaShop webservice: you decide which can, and what they are allowed to do. Every app has a unique connection key, with specific access rights.

## Adding a new key <a href="#webservice-addinganewkey" id="webservice-addinganewkey"></a>

The **"Add new webservice key"** button takes you to the webservice key creation form:

* **Key**. A unique key. You can either create your own or choose to use a generated one, for instance by clicking the "Generate!" button or by using any online key generator. Generated keys are most of the time safer because they are harder to guess.
* **Key description**. A reminder of who that key is for, and what it gives access to.
* **Status**. You can disable a key anytime. This enables you to only temporarily grant access to your data from a certain key.
* **Permissions**. You do not have to share ALL your data with each key. You can choose among a wide array of permissions, either by section or by type of access. You might want some applications to only be able to view a handful of items, while some others (for instance, ones that you would use to manage the shop remotely) should be able to edit and delete just about everything. Choose wisely.

Click **"Save"** when your key is ready.

<figure><img src="../../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

## Configuration <a href="#webservice-configuration" id="webservice-configuration"></a>

For security reasons, make sure your shop's server supports secure SSL connection.

The webservice configuration is pretty easy:

* **Enable PrestaShop's webservice**. If you do not want anyone to access your shop through third-party tools and applications, just keep it disabled.
* **Enable CGI mode for PHP**. The CGI mode is a special setting for the Apache server, where you tell it to use PHP as a CGI script rather than an Apache module. While the CGI mode has a reputation of being more secure, it has been found to have a security flaw as recently as May 2012. Ask your web host for advice.

<figure><img src="../../../.gitbook/assets/image (1) (2).png" alt=""><figcaption></figcaption></figure>

## Enable PrestaShop webservice <a href="#webservice-configuration" id="webservice-configuration"></a>

When enabling PrestaShop's webservice, the **status and URL of your store’s webservice** are displayed at the **top of the page** in _Advanced parameters > Webservice > Webservice status._ This feature helps troubleshoot common problems.

<figure><img src="../../../.gitbook/assets/image (4) (2).png" alt=""><figcaption></figcaption></figure>

## Perform partial updates <a href="#webservice-configuration" id="webservice-configuration"></a>

You can **perform partial updates** on webservice endpoints using the [PATCH method](https://en.wikipedia.org/wiki/PATCH\_\(HTTP\)). This means integrations can update part of a resource, instead of all the fields at once.

## PrestaShop 9 Admin API

PrestaShop 9 introduces a completely new **Admin API** powered by API Platform, replacing the legacy webservice system. This new API provides:

### Key Features
- **RESTful Design**: Modern REST API with JSON responses
- **API Platform Integration**: Built on top of the robust API Platform framework
- **Better Authentication**: Improved security and access control
- **Comprehensive Documentation**: Auto-generated API documentation
- **Modern Standards**: Follows current API best practices

### Available Endpoints
The Admin API includes endpoints for:
- Products and catalog management
- Orders and customer management
- Module management
- Configuration settings
- And many more...

### Accessing the API
- **Documentation**: Available in your back office at `/api/docs`
- **Base URL**: `/api/v1/`
- **Authentication**: Uses modern token-based authentication

### Migration from Legacy Webservice
If you're upgrading from PrestaShop 8, note that the legacy webservice system has been replaced. The new Admin API provides better performance, security, and developer experience.

{% hint style="info" %}
For detailed API documentation and usage examples, visit the [PrestaShop Developer Documentation](https://devdocs.prestashop-project.org/9/admin-api/).
{% endhint %}
