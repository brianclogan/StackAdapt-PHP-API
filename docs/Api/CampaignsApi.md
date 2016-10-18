# Swagger\Client\CampaignsApi

All URIs are relative to *http://api.stackadapt.com/service/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**findCampaigns**](CampaignsApi.md#findCampaigns) | **GET** /campaigns | Return all campaigns


# **findCampaigns**
> \Swagger\Client\Model\CampaignResponse[] findCampaigns()

Return all campaigns

Returns all campaigns from the system that the user has access to

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

$api_instance = new Swagger\Client\Api\CampaignsApi();

try {
    $result = $api_instance->findCampaigns();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CampaignsApi->findCampaigns: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Model\CampaignResponse[]**](../Model/CampaignResponse.md)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

