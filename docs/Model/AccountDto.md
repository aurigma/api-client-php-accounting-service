# # AccountDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique identifier. | [optional]
**tenant_id** | **int** | Tenant ID. | [optional]
**is_active** | **bool** | Indicates if the account is active. | [optional]
**subscription_plan_sku** | **string** | SKU of the subscription plan (if the account was created based on SKU). | [optional]
**subscription_plan_name** | **string** | Name of the subscription plan (if the account was created based on SKU). | [optional]
**activation_date** | **\DateTime** | Activation date in UTC time format. | [optional]
**deactivation_date** | **\DateTime** | Deactivation date in UTC time format. | [optional]
**month_count** | **int** | The number of months in the accounting period. | [optional]
**credit_units_limit** | **int** | Credit units limit. | [optional]
**file_storage_size_limit_in_gb** | **int** | File storage limit in gigabytes (GB). | [optional]
**storefront_limit** | **int** | Storefront limit. | [optional]
**account_period_infos** | [**\Aurigma\AssetStorage\Model\AccountPeriodInfoDto[]**](AccountPeriodInfoDto.md) | Account&#39;s periods. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
