# Aurigma\AssetStorage\TenantFilesInfoApi

All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**tenantFilesInfoGetTenantFilesInfos()**](TenantFilesInfoApi.md#tenantFilesInfoGetTenantFilesInfos) | **GET** /api/accounting-operational/v1/tenant-files-infos | Returns information about file storage usage for the specified time period. |


## `tenantFilesInfoGetTenantFilesInfos()`

```php
tenantFilesInfoGetTenantFilesInfos($start_time, $end_time, $granularity_options_days, $granularity_options_strategy, $tenant_id): \Aurigma\AssetStorage\Model\TenantFilesInfoDto[]
```

Returns information about file storage usage for the specified time period.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: ApiKey
$config = Aurigma\AssetStorage\Configuration::getDefaultConfiguration()->setApiKey('X-API-Key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Aurigma\AssetStorage\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-API-Key', 'Bearer');

// Configure OAuth2 access token for authorization: OAuth2ClientCredentials
$config = Aurigma\AssetStorage\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

// Configure OAuth2 access token for authorization: OAuth2Code
$config = Aurigma\AssetStorage\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

// Configure OAuth2 access token for authorization: OAuth2Implicit
$config = Aurigma\AssetStorage\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');

// Configure API key authorization: Bearer
$config = Aurigma\AssetStorage\Configuration::getDefaultConfiguration()->setApiKey('Authorization', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Aurigma\AssetStorage\Configuration::getDefaultConfiguration()->setApiKeyPrefix('Authorization', 'Bearer');


$apiInstance = new Aurigma\AssetStorage\Api\TenantFilesInfoApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$start_time = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | Start date in UTC time format.
$end_time = new \DateTime("2013-10-20T19:20:30+01:00"); // \DateTime | End date in UTC time format. If not specified, the current UTC time is used by default.
$granularity_options_days = 56; // int | Number of days per group.  Set to `0` to keep the original array unchanged.
$granularity_options_strategy = new \Aurigma\AssetStorage\Model\\Aurigma\AssetStorage\Model\GranularityStrategyType(); // \Aurigma\AssetStorage\Model\GranularityStrategyType | Granularity calculation strategy.
$tenant_id = 56; // int | Tenant ID.

try {
    $result = $apiInstance->tenantFilesInfoGetTenantFilesInfos($start_time, $end_time, $granularity_options_days, $granularity_options_strategy, $tenant_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling TenantFilesInfoApi->tenantFilesInfoGetTenantFilesInfos: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **start_time** | **\DateTime**| Start date in UTC time format. | [optional] |
| **end_time** | **\DateTime**| End date in UTC time format. If not specified, the current UTC time is used by default. | [optional] |
| **granularity_options_days** | **int**| Number of days per group.  Set to &#x60;0&#x60; to keep the original array unchanged. | [optional] |
| **granularity_options_strategy** | [**\Aurigma\AssetStorage\Model\GranularityStrategyType**](../Model/.md)| Granularity calculation strategy. | [optional] |
| **tenant_id** | **int**| Tenant ID. | [optional] |

### Return type

[**\Aurigma\AssetStorage\Model\TenantFilesInfoDto[]**](../Model/TenantFilesInfoDto.md)

### Authorization

[ApiKey](../../README.md#ApiKey), [OAuth2ClientCredentials](../../README.md#OAuth2ClientCredentials), [OAuth2Code](../../README.md#OAuth2Code), [OAuth2Implicit](../../README.md#OAuth2Implicit), [Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `text/plain`, `application/json`, `text/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
