# CollingMedia\StackAdapt\CampaignApi

All URIs are relative to *http://api.stackadapt.com/service/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createCampaign**](CampaignApi.md#createCampaign) | **POST** /campaign | Create new campaign
[**createCampaign_0**](CampaignApi.md#createCampaign_0) | **POST** /campaign | Create new campaign
[**deleteCampaign**](CampaignApi.md#deleteCampaign) | **DELETE** /campaign/{id} | Delete a campaign
[**deleteCampaign_0**](CampaignApi.md#deleteCampaign_0) | **DELETE** /campaign/{id} | Delete a campaign
[**findCampaign**](CampaignApi.md#findCampaign) | **GET** /campaign/{id} | Find campaign by id
[**findCampaign_0**](CampaignApi.md#findCampaign_0) | **GET** /campaign/{id} | Find campaign by id
[**findCampaigns**](CampaignApi.md#findCampaigns) | **GET** /campaigns | Return all campaigns
[**updateCampaign**](CampaignApi.md#updateCampaign) | **PUT** /campaign/{id} | Update existing campaign
[**updateCampaign_0**](CampaignApi.md#updateCampaign_0) | **PUT** /campaign/{id} | Update existing campaign


# **createCampaign**
> \CollingMedia\StackAdapt\Model\CampaignResponse createCampaign($body)

Create new campaign

Creates a new campaign

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();
$body = new \CollingMedia\StackAdapt\Model\CampaignRequest(); // \CollingMedia\StackAdapt\Model\CampaignRequest | 

try {
    $result = $api_instance->createCampaign($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->createCampaign: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\CollingMedia\StackAdapt\Model\CampaignRequest**](../Model/\CollingMedia\StackAdapt\Model\CampaignRequest.md)|  | [optional]

### Return type

[**\CollingMedia\StackAdapt\Model\CampaignResponse**](../Model/CampaignResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createCampaign_0**
> \CollingMedia\StackAdapt\Model\CampaignResponse createCampaign_0($body)

Create new campaign

Creates a new campaign

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();
$body = new \CollingMedia\StackAdapt\Model\CampaignRequest(); // \CollingMedia\StackAdapt\Model\CampaignRequest | 

try {
    $result = $api_instance->createCampaign_0($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->createCampaign_0: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\CollingMedia\StackAdapt\Model\CampaignRequest**](../Model/\CollingMedia\StackAdapt\Model\CampaignRequest.md)|  | [optional]

### Return type

[**\CollingMedia\StackAdapt\Model\CampaignResponse**](../Model/CampaignResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteCampaign**
> deleteCampaign($id)

Delete a campaign

Deletes a campaign

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();
$id = 56; // int | Id of campaign

try {
    $api_instance->deleteCampaign($id);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->deleteCampaign: ', $e->getMessage(), PHP_EOL;
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

# **deleteCampaign_0**
> deleteCampaign_0($id)

Delete a campaign

Deletes a campaign

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();
$id = 56; // int | Id of campaign

try {
    $api_instance->deleteCampaign_0($id);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->deleteCampaign_0: ', $e->getMessage(), PHP_EOL;
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

# **findCampaign**
> \CollingMedia\StackAdapt\Model\CampaignResponse findCampaign($id)

Find campaign by id

Returns a specific campaign with the corresponding id from the system that the user has access to

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();
$id = 56; // int | Id of campaign

try {
    $result = $api_instance->findCampaign($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->findCampaign: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of campaign |

### Return type

[**\CollingMedia\StackAdapt\Model\CampaignResponse**](../Model/CampaignResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findCampaign_0**
> \CollingMedia\StackAdapt\Model\CampaignResponse findCampaign_0($id)

Find campaign by id

Returns a specific campaign with the corresponding id from the system that the user has access to

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();
$id = 56; // int | Id of campaign

try {
    $result = $api_instance->findCampaign_0($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->findCampaign_0: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of campaign |

### Return type

[**\CollingMedia\StackAdapt\Model\CampaignResponse**](../Model/CampaignResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **findCampaigns**
> \CollingMedia\StackAdapt\Model\CampaignResponse[] findCampaigns()

Return all campaigns

Returns all campaigns from the system that the user has access to

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();

try {
    $result = $api_instance->findCampaigns();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->findCampaigns: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\CollingMedia\StackAdapt\Model\CampaignResponse[]**](../Model/CampaignResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateCampaign**
> \CollingMedia\StackAdapt\Model\CampaignResponse updateCampaign($id, $body)

Update existing campaign

Updates an existing campaign

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();
$id = 56; // int | Id of campaign
$body = new \CollingMedia\StackAdapt\Model\CampaignRequest(); // \CollingMedia\StackAdapt\Model\CampaignRequest | 

try {
    $result = $api_instance->updateCampaign($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->updateCampaign: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of campaign |
 **body** | [**\CollingMedia\StackAdapt\Model\CampaignRequest**](../Model/\CollingMedia\StackAdapt\Model\CampaignRequest.md)|  | [optional]

### Return type

[**\CollingMedia\StackAdapt\Model\CampaignResponse**](../Model/CampaignResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateCampaign_0**
> \CollingMedia\StackAdapt\Model\CampaignResponse updateCampaign_0($id, $body)

Update existing campaign

Updates an existing campaign

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

$api_instance = new CollingMedia\StackAdapt\Api\CampaignApi();
$id = 56; // int | Id of campaign
$body = new \CollingMedia\StackAdapt\Model\CampaignRequest(); // \CollingMedia\StackAdapt\Model\CampaignRequest | 

try {
    $result = $api_instance->updateCampaign_0($id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CampaignApi->updateCampaign_0: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Id of campaign |
 **body** | [**\CollingMedia\StackAdapt\Model\CampaignRequest**](../Model/\CollingMedia\StackAdapt\Model\CampaignRequest.md)|  | [optional]

### Return type

[**\CollingMedia\StackAdapt\Model\CampaignResponse**](../Model/CampaignResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

