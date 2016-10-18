# CampaignRequest

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The name of the campaign. | [default to 'API Test Campaign']
**budget** | **float** | The budget of the campaign. | [default to 10000.0]
**bid_type** | **string** | Type of bid model: cpm (Cost Per Thousand Impressions), cpc (Cost Per Click), cpe (Cost Per Engagement), cps (Cost Per Session) bid model. | [default to 'cpm']
**bid_amount_total** | **float** | The bid amount of the campaign. | [default to 5.0]
**optimize_type** | **string** | The type of optimization used for the campaign: ctr (CTR floor), cpc (CPC goal). | [optional] [default to 'cpc']
**optimize_value** | **float** | The value of the optimization. Example: The value is 0.2 for a $0.2 CPC goal, or a 0.2% CTR floor. | [optional] [default to 1.5]
**daily_cap** | **float** | The maximum budget to be spent in a single day. This value is only used if pace_evenly is NULL or false. | [optional] 
**pace_evenly** | **bool** | Whether or not to pace the campaign budget evenly over the course of the campaign. This value is only used if a valid end_date is specified. | [optional] [default to true]
**state** | **string** | The state of the campaign. | [optional] [default to 'active']
**start_date** | [**\DateTime**](Date.md) | The timestamp in UTC when the campaign will begin. | [optional] 
**end_date** | [**\DateTime**](Date.md) | The timestamp in UTC when the campaign will end. | [optional] 
**category_options** | **string[]** | The list of IAB categories to be included in the campaign. &lt;a class&#x3D;\&quot;campaign-link\&quot; target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://docs.google.com/document/d/1oZEWp_b9ccLsPNbTJf-w5ENHSSHiAjVQVcfjUh7LBsg/edit?usp&#x3D;sharing#bookmark&#x3D;id.wwmc2j4w9weo\&quot;&gt;Click Here&lt;/a&gt; for full list of IB categories. Leave empty to choose all. | [optional] 
**advertiser** | [**\CollingMedia\StackAdapt\Model\SubAdvertiser**](SubAdvertiser.md) |  | [optional] 
**country_options** | **string[]** | The list of ISO 3166-1 alpha-2 country codes to be included in the campaign. | [optional] 
**us_state_options** | **string[]** | The list of ISO 3166-2 US state codes to be included in the campaign. | [optional] 
**canada_province_options** | **string[]** | The list of ISO 3166-2 Canadian province codes to be included in the campaign. | [optional] 
**city_options** | **string** | The list of city ID objects to be included in the campaign. For more information &lt;a class&#x3D;\&quot;campaign-link\&quot; target&#x3D;\&quot;_blank\&quot; href&#x3D;\&quot;https://docs.google.com/document/d/1oZEWp_b9ccLsPNbTJf-w5ENHSSHiAjVQVcfjUh7LBsg/edit?usp&#x3D;sharing#bookmark&#x3D;id.19kxqs63mxbn\&quot;&gt;Click Here&lt;/a&gt;. | [optional] [default to 'Sugar Land > TX > US:618@ Missouri City > TX > US:618@ Houston > TX > US:618@ Austin > TX > US:635']
**domain_action** | **string** | Action to be taken on the \&quot;domain_options\&quot; list. | [optional] [default to 'exclude']
**domain_options** | **string[]** | The list of domains or subdomains to be included or excluded in the campaign. \&quot;domain_action\&quot; must also be set. Example: [\&quot;ford.com\&quot;, \&quot;www.american express.com\&quot;] | [optional] 
**device_type_options** | **string[]** | The list of device types to be included in the campaign. | [optional] 
**supply_type_options** | **string[]** | The list of mobile supply types to be included in the campaign. | [optional] 
**supply_source_options** | **string[]** | The list of supply sources to be included in the campaign. Please reach out to CSM for the list of supply sources. | [optional] 
**freq_cap_limit** | **int** | The user frequency cap value, which is the maximum amount of impressions that a unique user can see. | [optional] [default to 7]
**freq_cap_time** | **int** | The length of time in milliseconds when the user frequency cap counter restarts. | [optional] [default to 86400000]
**language_options** | **string[]** | A list of language(s) that are targeted. The campaign will only target sites or users whose language is included in the list. | [optional] 
**use_dma** | **bool** | Enable campaign to target city by Designated Market Area (DMA). | [optional] 
**conversion_trackers** | [**\CollingMedia\StackAdapt\Model\ConversionTracker[]**](ConversionTracker.md) |  | [optional] 
**allow_iframe_engagement** | **bool** | Allow engagement tracking by placing add within an iframe | [optional] [default to true]
**all_native_ads** | [**\CollingMedia\StackAdapt\Model\NativeAdRequest[]**](NativeAdRequest.md) | Native ad model | 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


