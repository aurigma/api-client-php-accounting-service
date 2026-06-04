# # OutputFilesInfoDto

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**job_id** | **string** | Job ID. | [optional]
**project_id** | **int** | Project ID. | [optional]
**project_item_id** | **int** | Project item ID. | [optional]
**tenant_id** | **int** | Tenant ID. | [optional]
**files_infos** | **string** | Information about image files in JSON format.  It&#39;s the serialized value of &#x60;Dictionary{string,long[]}&#x60;.  The file name is used as the key and the page areas are used as the value.  For example: &#x60;\&quot;{\\\&quot;FileName1\\\&quot;:[1,2],\\\&quot;FileName2\\\&quot;:[3,4]}\&quot;&#x60;. | [optional]
**trace_date** | **\DateTime** | Date the trace was generated. | [optional]

[[Back to Model list]](../../README.md#models) [[Back to API list]](../../README.md#endpoints) [[Back to README]](../../README.md)
