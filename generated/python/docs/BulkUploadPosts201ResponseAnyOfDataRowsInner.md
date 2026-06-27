# BulkUploadPosts201ResponseAnyOfDataRowsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**row_number** | **int** |  | 
**status** | **str** |  | 
**post** | [**CreatePost201ResponseAnyOfData**](CreatePost201ResponseAnyOfData.md) |  | [optional] 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | [optional] 
**warnings** | [**List[BulkUploadPosts201ResponseAnyOfDataRowsInnerWarningsInner]**](BulkUploadPosts201ResponseAnyOfDataRowsInnerWarningsInner.md) |  | 

## Example

```python
from kavenio.models.bulk_upload_posts201_response_any_of_data_rows_inner import BulkUploadPosts201ResponseAnyOfDataRowsInner

# TODO update the JSON string below
json = "{}"
# create an instance of BulkUploadPosts201ResponseAnyOfDataRowsInner from a JSON string
bulk_upload_posts201_response_any_of_data_rows_inner_instance = BulkUploadPosts201ResponseAnyOfDataRowsInner.from_json(json)
# print the JSON string representation of the object
print(BulkUploadPosts201ResponseAnyOfDataRowsInner.to_json())

# convert the object into a dict
bulk_upload_posts201_response_any_of_data_rows_inner_dict = bulk_upload_posts201_response_any_of_data_rows_inner_instance.to_dict()
# create an instance of BulkUploadPosts201ResponseAnyOfDataRowsInner from a dict
bulk_upload_posts201_response_any_of_data_rows_inner_from_dict = BulkUploadPosts201ResponseAnyOfDataRowsInner.from_dict(bulk_upload_posts201_response_any_of_data_rows_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


