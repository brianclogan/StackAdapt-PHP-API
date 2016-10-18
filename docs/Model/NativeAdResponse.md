# NativeAdResponse

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the native ad. | [default to 22]
**click_url** | **string** | The click URL of the native ad. Not used for App Install Campaigns, where the click url is on the campaign object. | [default to 'www.stackadapt.com']
**input_data** | [**\CollingMedia\StackAdapt\Model\InputData**](InputData.md) |  | 
**audit_status** | **string** | The audit status of the audit. | [optional] [default to 'pending']
**name** | **string** | The name of the native ad | [default to 'API New Native Ad']
**state** | **string** | The state of the campaign. | [optional] [default to 'active']
**imp_tracker_urls** | **string[]** | List of URLs for impression tracking. | [optional] 
**brandname** | **string** | Brand name associated with the creative. | [default to 'My Brand']
**creatives** | [**\CollingMedia\StackAdapt\Model\CreativeResponse[]**](CreativeResponse.md) |  | 
**icon** | [**\CollingMedia\StackAdapt\Model\CreativeResponse**](CreativeResponse.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


