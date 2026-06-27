# BulkUploadPosts201ResponseAnyOfDataSummary


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total_rows** | **int** |  | 
**succeeded** | **int** |  | 
**failed** | **int** |  | 
**warning_count** | **int** |  | 

## Example

```python
from kavenio.models.bulk_upload_posts201_response_any_of_data_summary import BulkUploadPosts201ResponseAnyOfDataSummary

# TODO update the JSON string below
json = "{}"
# create an instance of BulkUploadPosts201ResponseAnyOfDataSummary from a JSON string
bulk_upload_posts201_response_any_of_data_summary_instance = BulkUploadPosts201ResponseAnyOfDataSummary.from_json(json)
# print the JSON string representation of the object
print(BulkUploadPosts201ResponseAnyOfDataSummary.to_json())

# convert the object into a dict
bulk_upload_posts201_response_any_of_data_summary_dict = bulk_upload_posts201_response_any_of_data_summary_instance.to_dict()
# create an instance of BulkUploadPosts201ResponseAnyOfDataSummary from a dict
bulk_upload_posts201_response_any_of_data_summary_from_dict = BulkUploadPosts201ResponseAnyOfDataSummary.from_dict(bulk_upload_posts201_response_any_of_data_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


