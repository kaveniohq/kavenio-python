# BulkUploadPosts201ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**summary** | [**BulkUploadPosts201ResponseAnyOfDataSummary**](BulkUploadPosts201ResponseAnyOfDataSummary.md) |  | 
**rows** | [**List[BulkUploadPosts201ResponseAnyOfDataRowsInner]**](BulkUploadPosts201ResponseAnyOfDataRowsInner.md) |  | 
**warnings** | [**List[BulkUploadPosts201ResponseAnyOfDataRowsInnerWarningsInner]**](BulkUploadPosts201ResponseAnyOfDataRowsInnerWarningsInner.md) |  | 

## Example

```python
from kavenio.models.bulk_upload_posts201_response_any_of_data import BulkUploadPosts201ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of BulkUploadPosts201ResponseAnyOfData from a JSON string
bulk_upload_posts201_response_any_of_data_instance = BulkUploadPosts201ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(BulkUploadPosts201ResponseAnyOfData.to_json())

# convert the object into a dict
bulk_upload_posts201_response_any_of_data_dict = bulk_upload_posts201_response_any_of_data_instance.to_dict()
# create an instance of BulkUploadPosts201ResponseAnyOfData from a dict
bulk_upload_posts201_response_any_of_data_from_dict = BulkUploadPosts201ResponseAnyOfData.from_dict(bulk_upload_posts201_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


