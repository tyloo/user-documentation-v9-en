# Admin API

PrestaShop 9 introduces a completely new **Admin API** powered by API Platform, replacing the legacy webservice system. This modern API provides better security, performance, and developer experience for integrating with external systems and applications.

## Overview

The Admin API is built on **API Platform version 3** and uses **OAuth2** for authentication and authorization. It follows modern REST API standards and provides comprehensive endpoints for managing your PrestaShop store programmatically.

### Key Benefits

- **Modern Architecture**: Built on API Platform with CQRS (Command Query Responsibility Segregation) pattern
- **Enhanced Security**: OAuth2 authentication with granular permissions
- **Better Performance**: Optimized endpoints with improved response times
- **Comprehensive Documentation**: Auto-generated API documentation
- **Developer Friendly**: JSON-based responses with clear error handling
- **Extensible**: Easy to extend with custom modules

## Getting Started

### Accessing the API Documentation

The Admin API documentation is automatically generated and available in your back office:

1. Navigate to **Advanced Parameters > Admin API**
2. Click on **"View API Documentation"** to access the interactive documentation
3. The documentation is also available at `/api/docs` on your store

### Base URL

All API endpoints are available under the `/api/v1/` path:

```
https://your-store.com/api/v1/
```

## Authentication

The Admin API uses **OAuth2** for secure authentication. You'll need to:

1. **Create an API Client**: Generate client credentials in the back office
2. **Obtain Access Token**: Use your credentials to get an access token
3. **Include Token**: Add the token to your API requests

### Creating API Credentials

1. Go to **Advanced Parameters > Admin API**
2. Click **"Add new API client"**
3. Fill in the required information:
   - **Client Name**: A descriptive name for your application
   - **Description**: What this API client will be used for
   - **Scopes**: Select the permissions your application needs
4. Click **"Save"** to generate your client credentials

### Available Scopes

The Admin API provides granular permissions through scopes:

- **Products**: Manage product catalog, categories, and attributes
- **Orders**: Handle orders, customers, and order management
- **Modules**: Install, configure, and manage modules
- **Configuration**: Access and modify store settings
- **Statistics**: View analytics and reports
- **Files**: Manage file uploads and downloads

## Available Endpoints

### Products & Catalog
- `GET /api/v1/products` - List all products
- `POST /api/v1/products` - Create a new product
- `GET /api/v1/products/{id}` - Get product details
- `PUT /api/v1/products/{id}` - Update a product
- `DELETE /api/v1/products/{id}` - Delete a product
- `GET /api/v1/categories` - List categories
- `GET /api/v1/attributes` - List product attributes

### Orders & Customers
- `GET /api/v1/orders` - List all orders
- `GET /api/v1/orders/{id}` - Get order details
- `PUT /api/v1/orders/{id}` - Update order status
- `GET /api/v1/customers` - List customers
- `GET /api/v1/customers/{id}` - Get customer details

### Modules
- `GET /api/v1/modules` - List installed modules
- `POST /api/v1/modules/{name}/install` - Install a module
- `POST /api/v1/modules/{name}/uninstall` - Uninstall a module
- `GET /api/v1/modules/{name}/configuration` - Get module configuration

### Configuration
- `GET /api/v1/configuration` - Get store configuration
- `PUT /api/v1/configuration/{key}` - Update configuration value

## Example Usage

### Getting Product Information

```bash
curl -H "Authorization: Bearer YOUR_ACCESS_TOKEN" \
     -H "Content-Type: application/json" \
     https://your-store.com/api/v1/products
```

### Creating a New Product

```bash
curl -X POST \
     -H "Authorization: Bearer YOUR_ACCESS_TOKEN" \
     -H "Content-Type: application/json" \
     -d '{
       "name": "New Product",
       "price": 29.99,
       "description": "Product description",
       "active": true
     }' \
     https://your-store.com/api/v1/products
```

### Updating Order Status

```bash
curl -X PUT \
     -H "Authorization: Bearer YOUR_ACCESS_TOKEN" \
     -H "Content-Type: application/json" \
     -d '{
       "status": "shipped"
     }' \
     https://your-store.com/api/v1/orders/123
```

## Error Handling

The Admin API provides clear error responses with HTTP status codes:

- **200 OK**: Request successful
- **201 Created**: Resource created successfully
- **400 Bad Request**: Invalid request data
- **401 Unauthorized**: Authentication required
- **403 Forbidden**: Insufficient permissions
- **404 Not Found**: Resource not found
- **500 Internal Server Error**: Server error

### Error Response Format

```json
{
  "error": "validation_failed",
  "message": "The provided data is invalid",
  "details": {
    "name": "This field is required",
    "price": "Price must be a positive number"
  }
}
```

## Rate Limiting

The Admin API includes rate limiting to ensure fair usage:

- **Default Limit**: 1000 requests per hour per client
- **Burst Limit**: 100 requests per minute
- **Headers**: Rate limit information is included in response headers

## Migration from Legacy Webservice

If you're upgrading from PrestaShop 8, the legacy webservice system has been replaced. Key differences:

### What's Changed
- **Authentication**: OAuth2 instead of API keys
- **URL Structure**: `/api/v1/` instead of `/api/`
- **Response Format**: JSON instead of XML
- **Error Handling**: Improved error responses
- **Documentation**: Interactive API documentation

### Migration Steps
1. **Update Authentication**: Switch from API keys to OAuth2
2. **Update URLs**: Change endpoint URLs to new structure
3. **Update Parsing**: Switch from XML to JSON parsing
4. **Test Integration**: Verify all functionality works correctly

## Best Practices

### Security
- **Use HTTPS**: Always use secure connections
- **Rotate Tokens**: Regularly refresh access tokens
- **Limit Scopes**: Only request necessary permissions
- **Monitor Usage**: Keep track of API usage

### Performance
- **Use Pagination**: For large datasets, use pagination parameters
- **Cache Responses**: Cache frequently accessed data
- **Batch Operations**: Use bulk endpoints when available
- **Optimize Queries**: Use filters to reduce response size

### Development
- **Use Documentation**: Always refer to the interactive documentation
- **Handle Errors**: Implement proper error handling
- **Test Thoroughly**: Test all API interactions
- **Version Control**: Keep track of API versions

## Troubleshooting

### Common Issues

**Authentication Errors**
- Verify your client credentials are correct
- Check that your access token is valid and not expired
- Ensure you're using the correct authorization header format

**Permission Errors**
- Verify your API client has the required scopes
- Check that the user account has necessary permissions
- Ensure the resource exists and is accessible

**Rate Limiting**
- Monitor your request frequency
- Implement exponential backoff for retries
- Consider caching responses to reduce API calls

### Getting Help

- **API Documentation**: Use the interactive documentation at `/api/docs`
- **Developer Documentation**: Visit [devdocs.prestashop-project.org](https://devdocs.prestashop-project.org/9/admin-api/)
- **Community Support**: Join the PrestaShop community forums
- **Professional Support**: Contact PrestaShop for enterprise support

{% hint style="info" %}
The Admin API is designed to be the primary way to integrate with PrestaShop 9. It provides a modern, secure, and efficient way to manage your store programmatically.
{% endhint %}
