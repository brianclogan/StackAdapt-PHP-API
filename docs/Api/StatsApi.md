# CollingMedia\StackAdapt\StatsApi

All URIs are relative to *http://api.stackadapt.com/service/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getStats**](StatsApi.md#getStats) | **GET** /stats | Get stats
[**getStats_0**](StatsApi.md#getStats_0) | **GET** /stats | Get stats


# **getStats**
> getStats($resource, $type, $id, $start_date, $end_date, $timezone, $group_by_resource)

Get stats

Returns stats on user query. Reponse depends on what stats you query for we recommend you try out this function to see what the responses are. <a target=\"_blank\" href=\"https://docs.google.com/document/d/1oZEWp_b9ccLsPNbTJf-w5ENHSSHiAjVQVcfjUh7LBsg/edit?usp=sharing#bookmark=id.t8vzvev042c4\">Click Here</a> for examples of stats requests and responses

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

$api_instance = new CollingMedia\StackAdapt\Api\StatsApi();
$resource = "resource_example"; // string | The resource type to retrieve. Valid resources are: \"campaign\", \"conversion_tracker\" \"line_item\", \"native_ad\", \"advertiser\", or \"buyer_account\" (total account stats)
$type = "type_example"; // string | The type of stats to retrieve. Valid types are: \"domain\", \"total\", \"daily\", and \"hourly\". \"domain\" type is only supported if resource is \"campaign\"
$id = 56; // int | Id of resource
$start_date = new \DateTime(); // \DateTime | The start date in the format of \"yyyy-mm-dd\"
$end_date = new \DateTime(); // \DateTime | The end date in the format of \"yyyy-mm-dd\"
$timezone = "timezone_example"; // string | The timezone of the start and end date, if applicable.
$group_by_resource = "group_by_resource_example"; // string | The resource type to group by when retrieve stats. Valid group_by_resources are: \"advertiser\", \"line_item\", \"campaign\", \"native_ad\". The group_by_resource should be subordinated to resource for group by action.

try {
    $api_instance->getStats($resource, $type, $id, $start_date, $end_date, $timezone, $group_by_resource);
} catch (Exception $e) {
    echo 'Exception when calling StatsApi->getStats: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **resource** | **string**| The resource type to retrieve. Valid resources are: \&quot;campaign\&quot;, \&quot;conversion_tracker\&quot; \&quot;line_item\&quot;, \&quot;native_ad\&quot;, \&quot;advertiser\&quot;, or \&quot;buyer_account\&quot; (total account stats) |
 **type** | **string**| The type of stats to retrieve. Valid types are: \&quot;domain\&quot;, \&quot;total\&quot;, \&quot;daily\&quot;, and \&quot;hourly\&quot;. \&quot;domain\&quot; type is only supported if resource is \&quot;campaign\&quot; |
 **id** | **int**| Id of resource | [optional]
 **start_date** | **\DateTime**| The start date in the format of \&quot;yyyy-mm-dd\&quot; | [optional]
 **end_date** | **\DateTime**| The end date in the format of \&quot;yyyy-mm-dd\&quot; | [optional]
 **timezone** | **string**| The timezone of the start and end date, if applicable. | [optional]
 **group_by_resource** | **string**| The resource type to group by when retrieve stats. Valid group_by_resources are: \&quot;advertiser\&quot;, \&quot;line_item\&quot;, \&quot;campaign\&quot;, \&quot;native_ad\&quot;. The group_by_resource should be subordinated to resource for group by action. | [optional]

### Return type

void (empty response body)

### Authorization

[api_key](../../README.md#api_key), [X-Authorization](../../README.md#X-Authorization)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)
