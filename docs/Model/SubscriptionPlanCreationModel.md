# # SubscriptionPlanCreationModel

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**sku** | **string** | Unique SKU. |
**name** | **string** | Unique name. |
**month_count** | **int** | The number of months in the accounting period. | [optional]
**price** | **int** | Price. | [optional]
**credit_units_limit** | **int** | Credit units limit. | [optional]
**file_storage_size_limit_in_gb** | **int** | File storage limit in gigabytes (GB). | [optional]
**storefront_limit** | **int** | Storefront limit. | [optional]
**archived_date** | **\DateTime** | Date and time when the subscription plan was archived, or &#x60;null&#x60; if the plan is active. | [optional] [readonly]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
