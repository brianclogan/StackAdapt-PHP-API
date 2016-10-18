# Swagger\Client\NativeadsApi

All URIs are relative to *http://api.stackadapt.com/service/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**findNativeAds**](NativeadsApi.md#findNativeAds) | **GET** /native_ads | Returns all native ads


# **findNativeAds**
> \Swagger\Client\Model\NativeAdResponse[] findNativeAds()

Returns all native ads

Returns all native ads from the system that the user has access to

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

$api_instance = new Swagger\Client\Api\NativeadsApi();

try {
    $result = $api_instance->findNativeAds();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NativeadsApi->findNativeAds: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\NativeAdResponse[]**](../Model/NativeAdResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

