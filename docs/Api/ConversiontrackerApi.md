# Swagger\Client\ConversiontrackerApi

All URIs are relative to *http://api.stackadapt.com/service/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createConversionTracker**](ConversiontrackerApi.md#createConversionTracker) | **POST** /conversion_tracker | Create new conversion tracker
[**deleteConversionTrackers**](ConversiontrackerApi.md#deleteConversionTrackers) | **DELETE** /conversion_tracker/{id} | Delete a conversion tracker
[**findConversionTracker**](ConversiontrackerApi.md#findConversionTracker) | **GET** /conversion_tracker/{id} | Find conversion tracker by id
[**updateConversionTracker**](ConversiontrackerApi.md#updateConversionTracker) | **PUT** /conversion_tracker/{id} | Update exisiting conversion tracker


# **createConversionTracker**
> \Swagger\Client\Model\ConversionTracker createConversionTracker($body)

Create new conversion tracker

Creates a new conversion_tracker

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('api_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('api_key', 'Bearer');
// Configure API key authorization: X-Authorization
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Authorization', 'Bearer');

$api_instance = new Swagger\Client\Api\ConversiontrackerApi();
$body = new \Swagger\Client\Model\ConversionTracker(); // \Swagger\Client\Model\ConversionTracker | 

try {
    $result = $api_instance->createConversionTracker($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ConversiontrackerApi->createConversionTracker: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ConversionTracker**](../Model/\Swagger\Client\Model\ConversionTracker.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\ConversionTracker**](../Model/ConversionTracker.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteConversionTrackers**
> deleteConversionTrackers($id)

Delete a conversion tracker

Deletes a conversion tracker from the system that the user has access to

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('api_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('api_key', 'Bearer');
// Configure API key authorization: X-Authorization
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Authorization', 'Bearer');

$api_instance = new Swagger\Client\Api\ConversiontrackerApi();
$id = 56; // int | Id of conversion_tracker

try {
    $api_instance->deleteConversionTrackers($id);
} catch (Exception $e) {
    echo 'Exception when calling ConversiontrackerApi->deleteConversionTrackers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of conversion_tracker |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findConversionTracker**
> \Swagger\Client\Model\ConversionTracker findConversionTracker($id)

Find conversion tracker by id

Returns a conversion tracker from the system that the user has access to

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('api_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('api_key', 'Bearer');
// Configure API key authorization: X-Authorization
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Authorization', 'Bearer');

$api_instance = new Swagger\Client\Api\ConversiontrackerApi();
$id = 56; // int | Id of conversion_tracker

try {
    $result = $api_instance->findConversionTracker($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ConversiontrackerApi->findConversionTracker: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of conversion_tracker |

### Return type

[**\Swagger\Client\Model\ConversionTracker**](../Model/ConversionTracker.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateConversionTracker**
> \Swagger\Client\Model\ConversionTracker updateConversionTracker($id, $body)

Update exisiting conversion tracker

Updates a new conversion_tracker

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('api_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('api_key', 'Bearer');
// Configure API key authorization: X-Authorization
Swagger\Client\Configuration::getDefaultConfiguration()->setApiKey('X-Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// Swagger\Client\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Authorization', 'Bearer');

$api_instance = new Swagger\Client\Api\ConversiontrackerApi();
$id = 56; // int | Id of conversion_tracker
$body = new \Swagger\Client\Model\ConversionTracker(); // \Swagger\Client\Model\ConversionTracker | 

try {
    $result = $api_instance->updateConversionTracker($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ConversiontrackerApi->updateConversionTracker: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of conversion_tracker |
 **body** | [**\Swagger\Client\Model\ConversionTracker**](../Model/\Swagger\Client\Model\ConversionTracker.md)|  | [optional]

### Return type

[**\Swagger\Client\Model\ConversionTracker**](../Model/ConversionTracker.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

