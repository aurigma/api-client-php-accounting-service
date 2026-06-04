# Aurigma\AssetStorage\SubscriptionPlanApi

All URIs are relative to http://localhost, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**subscriptionPlanArchive()**](SubscriptionPlanApi.md#subscriptionPlanArchive) | **POST** /api/accounting-operational/v1/subscription-plans/{id}/archive | Archives the subscription plan. |
| [**subscriptionPlanCreate()**](SubscriptionPlanApi.md#subscriptionPlanCreate) | **POST** /api/accounting-operational/v1/subscription-plans | Creates a new subscription plan. |
| [**subscriptionPlanGetAll()**](SubscriptionPlanApi.md#subscriptionPlanGetAll) | **GET** /api/accounting-operational/v1/subscription-plans | Returns subscription plans. |
| [**subscriptionPlanGetById()**](SubscriptionPlanApi.md#subscriptionPlanGetById) | **GET** /api/accounting-operational/v1/subscription-plans/{id} | Returns a subscription plan by ID. |
| [**subscriptionPlanImportFromCsv()**](SubscriptionPlanApi.md#subscriptionPlanImportFromCsv) | **POST** /api/accounting-operational/v1/subscription-plans/import-from-csv |  |


## `subscriptionPlanArchive()`

```php
subscriptionPlanArchive($id): \Aurigma\AssetStorage\Model\SubscriptionPlanDto
```

Archives the subscription plan.

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


$apiInstance = new Aurigma\AssetStorage\Api\SubscriptionPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | ID of the subscription plan.

try {
    $result = $apiInstance->subscriptionPlanArchive($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionPlanApi->subscriptionPlanArchive: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| ID of the subscription plan. | |

### Return type

[**\Aurigma\AssetStorage\Model\SubscriptionPlanDto**](../Model/SubscriptionPlanDto.md)

### Authorization

[ApiKey](../../README.md#ApiKey), [OAuth2ClientCredentials](../../README.md#OAuth2ClientCredentials), [OAuth2Code](../../README.md#OAuth2Code), [OAuth2Implicit](../../README.md#OAuth2Implicit), [Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `text/plain`, `application/json`, `text/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `subscriptionPlanCreate()`

```php
subscriptionPlanCreate($subscription_plan_creation_model): \Aurigma\AssetStorage\Model\SubscriptionPlanDto
```

Creates a new subscription plan.

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


$apiInstance = new Aurigma\AssetStorage\Api\SubscriptionPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$subscription_plan_creation_model = new \Aurigma\AssetStorage\Model\SubscriptionPlanCreationModel(); // \Aurigma\AssetStorage\Model\SubscriptionPlanCreationModel | The model to create a subscription plan.

try {
    $result = $apiInstance->subscriptionPlanCreate($subscription_plan_creation_model);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionPlanApi->subscriptionPlanCreate: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subscription_plan_creation_model** | [**\Aurigma\AssetStorage\Model\SubscriptionPlanCreationModel**](../Model/SubscriptionPlanCreationModel.md)| The model to create a subscription plan. | |

### Return type

[**\Aurigma\AssetStorage\Model\SubscriptionPlanDto**](../Model/SubscriptionPlanDto.md)

### Authorization

[ApiKey](../../README.md#ApiKey), [OAuth2ClientCredentials](../../README.md#OAuth2ClientCredentials), [OAuth2Code](../../README.md#OAuth2Code), [OAuth2Implicit](../../README.md#OAuth2Implicit), [Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json-patch+json`, `application/json`, `text/json`, `application/*+json`
- **Accept**: `text/plain`, `application/json`, `text/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `subscriptionPlanGetAll()`

```php
subscriptionPlanGetAll($type, $skip, $take, $search, $sorting): \Aurigma\AssetStorage\Model\PagedOfSubscriptionPlanDto
```

Returns subscription plans.

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


$apiInstance = new Aurigma\AssetStorage\Api\SubscriptionPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$type = new \Aurigma\AssetStorage\Model\\Aurigma\AssetStorage\Model\SubscriptionPlanFilterType(); // \Aurigma\AssetStorage\Model\SubscriptionPlanFilterType | Subscription plan type.  The default value is Aurigma.AccountingService.Operational.AppServices.Enums.SubscriptionPlanFilterType.All.
$skip = 56; // int | Number of items to skip before starting to return results.
$take = 56; // int | Maximum number of items to return.
$search = 'search_example'; // string | Search text used to filter subscription plans by partial match.
$sorting = 'sorting_example'; // string | Defines the sorting order of the result list in SQL ORDER BY format,  e.g.: `Name ASC`, `Sku DESC` (case insensitive).

try {
    $result = $apiInstance->subscriptionPlanGetAll($type, $skip, $take, $search, $sorting);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionPlanApi->subscriptionPlanGetAll: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **type** | [**\Aurigma\AssetStorage\Model\SubscriptionPlanFilterType**](../Model/.md)| Subscription plan type.  The default value is Aurigma.AccountingService.Operational.AppServices.Enums.SubscriptionPlanFilterType.All. | [optional] |
| **skip** | **int**| Number of items to skip before starting to return results. | [optional] |
| **take** | **int**| Maximum number of items to return. | [optional] |
| **search** | **string**| Search text used to filter subscription plans by partial match. | [optional] |
| **sorting** | **string**| Defines the sorting order of the result list in SQL ORDER BY format,  e.g.: &#x60;Name ASC&#x60;, &#x60;Sku DESC&#x60; (case insensitive). | [optional] |

### Return type

[**\Aurigma\AssetStorage\Model\PagedOfSubscriptionPlanDto**](../Model/PagedOfSubscriptionPlanDto.md)

### Authorization

[ApiKey](../../README.md#ApiKey), [OAuth2ClientCredentials](../../README.md#OAuth2ClientCredentials), [OAuth2Code](../../README.md#OAuth2Code), [OAuth2Implicit](../../README.md#OAuth2Implicit), [Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `text/plain`, `application/json`, `text/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `subscriptionPlanGetById()`

```php
subscriptionPlanGetById($id): \Aurigma\AssetStorage\Model\SubscriptionPlanDto
```

Returns a subscription plan by ID.

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


$apiInstance = new Aurigma\AssetStorage\Api\SubscriptionPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 'id_example'; // string | Subscription plan ID.

try {
    $result = $apiInstance->subscriptionPlanGetById($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionPlanApi->subscriptionPlanGetById: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **string**| Subscription plan ID. | |

### Return type

[**\Aurigma\AssetStorage\Model\SubscriptionPlanDto**](../Model/SubscriptionPlanDto.md)

### Authorization

[ApiKey](../../README.md#ApiKey), [OAuth2ClientCredentials](../../README.md#OAuth2ClientCredentials), [OAuth2Code](../../README.md#OAuth2Code), [OAuth2Implicit](../../README.md#OAuth2Implicit), [Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `text/plain`, `application/json`, `text/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `subscriptionPlanImportFromCsv()`

```php
subscriptionPlanImportFromCsv($csv_file): \Aurigma\AssetStorage\Model\PagedOfSubscriptionPlanDto
```



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


$apiInstance = new Aurigma\AssetStorage\Api\SubscriptionPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$csv_file = "/path/to/file.txt"; // \SplFileObject

try {
    $result = $apiInstance->subscriptionPlanImportFromCsv($csv_file);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SubscriptionPlanApi->subscriptionPlanImportFromCsv: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **csv_file** | **\SplFileObject****\SplFileObject**|  | [optional] |

### Return type

[**\Aurigma\AssetStorage\Model\PagedOfSubscriptionPlanDto**](../Model/PagedOfSubscriptionPlanDto.md)

### Authorization

[ApiKey](../../README.md#ApiKey), [OAuth2ClientCredentials](../../README.md#OAuth2ClientCredentials), [OAuth2Code](../../README.md#OAuth2Code), [OAuth2Implicit](../../README.md#OAuth2Implicit), [Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `multipart/form-data`
- **Accept**: `text/plain`, `application/json`, `text/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
