# CollingMedia\StackAdapt\ConversiontrackersApi

All URIs are relative to *http://api.stackadapt.com/service/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**findConversionTrackers**](ConversiontrackersApi.md#findConversionTrackers) | **GET** /conversion_trackers | Returns all conversion trackers


# **findConversionTrackers**
> \CollingMedia\StackAdapt\Model\ConversionTracker[] findConversionTrackers()

Returns all conversion trackers

Returns all conversion trackers from the system that the user has access to

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure API key authorization: api_key
CollingMedia\StackAdapt\Configuration::getDefaultConfiguration()->setApiKey('api_key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// CollingMedia\StackAdapt\Configuration::getDefaultConfiguration()->setApiKeyPrefix('api_key', 'Bearer');
// Configure API key authorization: X-Authorization
CollingMedia\StackAdapt\Configuration::getDefaultConfiguration()->setApiKey('X-Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// CollingMedia\StackAdapt\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Authorization', 'Bearer');

$api_instance = new CollingMedia\StackAdapt\Api\ConversiontrackersApi();

try {
    $result = $api_instance->findConversionTrackers();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ConversiontrackersApi->findConversionTrackers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\CollingMedia\StackAdapt\Model\ConversionTracker[]**](../Model/ConversionTracker.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

