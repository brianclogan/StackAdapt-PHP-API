# CollingMedia\StackAdapt\NativeadApi

All URIs are relative to *http://api.stackadapt.com/service/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addNativeAd**](NativeadApi.md#addNativeAd) | **POST** /native_ad | Create new native ad
[**deleteNativeAd**](NativeadApi.md#deleteNativeAd) | **DELETE** /native_ad/{id} | Delete a native ad
[**findNativeAd**](NativeadApi.md#findNativeAd) | **GET** /native_ad/{id} | Find native ad by id
[**updateNativeAd**](NativeadApi.md#updateNativeAd) | **PUT** /native_ad/{id} | Update existing native ad


# **addNativeAd**
> \CollingMedia\StackAdapt\Model\NativeAdResponse addNativeAd($body)

Create new native ad

Creates a new native ad

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

$api_instance = new CollingMedia\StackAdapt\Api\NativeadApi();
$body = new \CollingMedia\StackAdapt\Model\NativeAdRequest(); // \CollingMedia\StackAdapt\Model\NativeAdRequest | 

try {
    $result = $api_instance->addNativeAd($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NativeadApi->addNativeAd: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\CollingMedia\StackAdapt\Model\NativeAdRequest**](../Model/\CollingMedia\StackAdapt\Model\NativeAdRequest.md)|  | [optional]

### Return type

[**\CollingMedia\StackAdapt\Model\NativeAdResponse**](../Model/NativeAdResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteNativeAd**
> deleteNativeAd($id)

Delete a native ad

Deletes an existing native ad

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

$api_instance = new CollingMedia\StackAdapt\Api\NativeadApi();
$id = 56; // int | Id of campaign

try {
    $api_instance->deleteNativeAd($id);
} catch (Exception $e) {
    echo 'Exception when calling NativeadApi->deleteNativeAd: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of campaign |

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findNativeAd**
> \CollingMedia\StackAdapt\Model\NativeAdResponse findNativeAd($id)

Find native ad by id

Returns a specific native ad with the corresponding id from the system that the user has access to

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

$api_instance = new CollingMedia\StackAdapt\Api\NativeadApi();
$id = 56; // int | Id of campaign

try {
    $result = $api_instance->findNativeAd($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NativeadApi->findNativeAd: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of campaign |

### Return type

[**\CollingMedia\StackAdapt\Model\NativeAdResponse**](../Model/NativeAdResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateNativeAd**
> \CollingMedia\StackAdapt\Model\NativeAdResponse updateNativeAd($id, $body)

Update existing native ad

Updates an existing native ad

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

$api_instance = new CollingMedia\StackAdapt\Api\NativeadApi();
$id = 56; // int | Id of campaign
$body = new \CollingMedia\StackAdapt\Model\NativeAdRequest(); // \CollingMedia\StackAdapt\Model\NativeAdRequest | 

try {
    $result = $api_instance->updateNativeAd($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling NativeadApi->updateNativeAd: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of campaign |
 **body** | [**\CollingMedia\StackAdapt\Model\NativeAdRequest**](../Model/\CollingMedia\StackAdapt\Model\NativeAdRequest.md)|  | [optional]

### Return type

[**\CollingMedia\StackAdapt\Model\NativeAdResponse**](../Model/NativeAdResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

