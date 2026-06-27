# BulkUploadPosts201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**BulkUploadPosts201ResponseAnyOfData**](BulkUploadPosts201ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.bulk_upload_posts201_response import BulkUploadPosts201Response

# TODO update the JSON string below
json = "{}"
# create an instance of BulkUploadPosts201Response from a JSON string
bulk_upload_posts201_response_instance = BulkUploadPosts201Response.from_json(json)
# print the JSON string representation of the object
print(BulkUploadPosts201Response.to_json())

# convert the object into a dict
bulk_upload_posts201_response_dict = bulk_upload_posts201_response_instance.to_dict()
# create an instance of BulkUploadPosts201Response from a dict
bulk_upload_posts201_response_from_dict = BulkUploadPosts201Response.from_dict(bulk_upload_posts201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


