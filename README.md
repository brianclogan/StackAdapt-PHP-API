# SwaggerClient-php
Use this API to create Native Ads and Campaigns on the StackAdapt Platform Use this API to create Native Ads and Campaigns on the StackAdapt Platform

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 2.0.0
- Build date: 2016-10-18T22:29:35.986Z
- Build package: class io.swagger.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.4.0 and later

## Installation & Usage
### Composer

```composer require colling-media/stackadapt-api
```

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit lib/Tests
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## Documentation for API Endpoints

All URIs are relative to *http://api.stackadapt.com/service/v2*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CampaignApi* | [**createCampaign**](docs/Api/CampaignApi.md#createcampaign) | **POST** /campaign | Create new campaign
*CampaignApi* | [**createCampaign_0**](docs/Api/CampaignApi.md#createcampaign_0) | **POST** /campaign | Create new campaign
*CampaignApi* | [**deleteCampaign**](docs/Api/CampaignApi.md#deletecampaign) | **DELETE** /campaign/{id} | Delete a campaign
*CampaignApi* | [**deleteCampaign_0**](docs/Api/CampaignApi.md#deletecampaign_0) | **DELETE** /campaign/{id} | Delete a campaign
*CampaignApi* | [**findCampaign**](docs/Api/CampaignApi.md#findcampaign) | **GET** /campaign/{id} | Find campaign by id
*CampaignApi* | [**findCampaign_0**](docs/Api/CampaignApi.md#findcampaign_0) | **GET** /campaign/{id} | Find campaign by id
*CampaignApi* | [**findCampaigns**](docs/Api/CampaignApi.md#findcampaigns) | **GET** /campaigns | Return all campaigns
*CampaignApi* | [**updateCampaign**](docs/Api/CampaignApi.md#updatecampaign) | **PUT** /campaign/{id} | Update existing campaign
*CampaignApi* | [**updateCampaign_0**](docs/Api/CampaignApi.md#updatecampaign_0) | **PUT** /campaign/{id} | Update existing campaign
*CampaignsApi* | [**findCampaigns**](docs/Api/CampaignsApi.md#findcampaigns) | **GET** /campaigns | Return all campaigns
*ConversionTrackersApi* | [**createConversionTracker**](docs/Api/ConversionTrackersApi.md#createconversiontracker) | **POST** /conversion_tracker | Create new conversion tracker
*ConversionTrackersApi* | [**deleteConversionTrackers**](docs/Api/ConversionTrackersApi.md#deleteconversiontrackers) | **DELETE** /conversion_tracker/{id} | Delete a conversion tracker
*ConversionTrackersApi* | [**findConversionTracker**](docs/Api/ConversionTrackersApi.md#findconversiontracker) | **GET** /conversion_tracker/{id} | Find conversion tracker by id
*ConversionTrackersApi* | [**findConversionTrackers**](docs/Api/ConversionTrackersApi.md#findconversiontrackers) | **GET** /conversion_trackers | Returns all conversion trackers
*ConversionTrackersApi* | [**updateConversionTracker**](docs/Api/ConversionTrackersApi.md#updateconversiontracker) | **PUT** /conversion_tracker/{id} | Update exisiting conversion tracker
*ConversiontrackerApi* | [**createConversionTracker**](docs/Api/ConversiontrackerApi.md#createconversiontracker) | **POST** /conversion_tracker | Create new conversion tracker
*ConversiontrackerApi* | [**deleteConversionTrackers**](docs/Api/ConversiontrackerApi.md#deleteconversiontrackers) | **DELETE** /conversion_tracker/{id} | Delete a conversion tracker
*ConversiontrackerApi* | [**findConversionTracker**](docs/Api/ConversiontrackerApi.md#findconversiontracker) | **GET** /conversion_tracker/{id} | Find conversion tracker by id
*ConversiontrackerApi* | [**updateConversionTracker**](docs/Api/ConversiontrackerApi.md#updateconversiontracker) | **PUT** /conversion_tracker/{id} | Update exisiting conversion tracker
*ConversiontrackersApi* | [**findConversionTrackers**](docs/Api/ConversiontrackersApi.md#findconversiontrackers) | **GET** /conversion_trackers | Returns all conversion trackers
*NativeAdApi* | [**addNativeAd**](docs/Api/NativeAdApi.md#addnativead) | **POST** /native_ad | Create new native ad
*NativeAdApi* | [**deleteNativeAd**](docs/Api/NativeAdApi.md#deletenativead) | **DELETE** /native_ad/{id} | Delete a native ad
*NativeAdApi* | [**findNativeAd**](docs/Api/NativeAdApi.md#findnativead) | **GET** /native_ad/{id} | Find native ad by id
*NativeAdApi* | [**findNativeAds**](docs/Api/NativeAdApi.md#findnativeads) | **GET** /native_ads | Returns all native ads
*NativeAdApi* | [**updateNativeAd**](docs/Api/NativeAdApi.md#updatenativead) | **PUT** /native_ad/{id} | Update existing native ad
*NativeadApi* | [**addNativeAd**](docs/Api/NativeadApi.md#addnativead) | **POST** /native_ad | Create new native ad
*NativeadApi* | [**deleteNativeAd**](docs/Api/NativeadApi.md#deletenativead) | **DELETE** /native_ad/{id} | Delete a native ad
*NativeadApi* | [**findNativeAd**](docs/Api/NativeadApi.md#findnativead) | **GET** /native_ad/{id} | Find native ad by id
*NativeadApi* | [**updateNativeAd**](docs/Api/NativeadApi.md#updatenativead) | **PUT** /native_ad/{id} | Update existing native ad
*NativeadsApi* | [**findNativeAds**](docs/Api/NativeadsApi.md#findnativeads) | **GET** /native_ads | Returns all native ads
*StatsApi* | [**getStats**](docs/Api/StatsApi.md#getstats) | **GET** /stats | Get stats
*StatsApi* | [**getStats_0**](docs/Api/StatsApi.md#getstats_0) | **GET** /stats | Get stats


## Documentation For Models

 - [Campaign](docs/Model/Campaign.md)
 - [CampaignRequest](docs/Model/CampaignRequest.md)
 - [CampaignResponse](docs/Model/CampaignResponse.md)
 - [ConversionTracker](docs/Model/ConversionTracker.md)
 - [CreativeRequest](docs/Model/CreativeRequest.md)
 - [CreativeResponse](docs/Model/CreativeResponse.md)
 - [ErrorModel](docs/Model/ErrorModel.md)
 - [ErrorObjectModel](docs/Model/ErrorObjectModel.md)
 - [InputData](docs/Model/InputData.md)
 - [LineItem](docs/Model/LineItem.md)
 - [NativeAd](docs/Model/NativeAd.md)
 - [NativeAdRequest](docs/Model/NativeAdRequest.md)
 - [NativeAdResponse](docs/Model/NativeAdResponse.md)
 - [SubAdvertiser](docs/Model/SubAdvertiser.md)


## Documentation For Authorization


## X-Authorization

- **Type**: API key
- **API key parameter name**: X-Authorization
- **Location**: HTTP header

## api_key

- **Type**: API key
- **API key parameter name**: api_key
- **Location**: URL query string


## Author




