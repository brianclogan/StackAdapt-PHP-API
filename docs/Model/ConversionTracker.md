# ConversionTracker

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | The ID of the conversion_tracker. | [default to 102]
**name** | **string** | The name of the conversion_tracker. | [default to 'API Tracker']
**code** | **string** | Code of the conversion_tracker. | [optional] [default to 'null']
**description** | **string** | Some description of the conversion_tracker. | [optional] [default to 'This is a tracker']
**user_id** | **string** | User who owns the conversion_tracker. | [optional] [default to '30']
**conv_type** | **string** | Specifies whether the conversion is matched by an impression or a click. | [default to 'imp']
**post_time** | **int** | Time till tracker expires for each user. Max: 2592000000 (30 days) | [default to 2592000000]
**count_type** | **string** | Specifies whether the conversion can be counted multiple times, or only once, by the same user. | [optional] [default to 'once']

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


