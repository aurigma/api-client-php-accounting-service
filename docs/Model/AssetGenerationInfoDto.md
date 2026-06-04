# # AssetGenerationInfoDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tenant_id** | **int** | Tenant ID. | [optional]
**environment_id** | **string** | Environment ID. | [optional]
**asset_id** | **string** | Asset ID. | [optional]
**asset_type** | **int** | Asset type. | [optional]
**spec_name** | **string** | Specification name. | [optional]
**spec_group** | **string** | Specification group. | [optional]
**spec_parameters** | **string** | Specification parameters.  It&#39;s the serialized value of &#x60;Dictionary{string,string}&#x60;.  The parameter name is used as the key, and the value is used as the value.  For example: &#x60;&#39;{\\\&quot;L\\\&quot;:\&quot;10\&quot;,\\\&quot;W\\\&quot;:\&quot;20\&quot;,\\\&quot;H\\\&quot;:\&quot;30\&quot;}&#39;&#x60;. | [optional]
**provider** | **string** | Provider. | [optional]
**licensed** | **bool** | Indicates if a license is required. | [optional]
**trace_date** | **\DateTime** | Date the trace was generated. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
