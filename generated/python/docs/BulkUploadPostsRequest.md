# BulkUploadPostsRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**csv** | **str** |  | 
**defaults** | [**CreatePostRequest**](CreatePostRequest.md) |  | [optional] 

## Example

```python
from kavenio.models.bulk_upload_posts_request import BulkUploadPostsRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BulkUploadPostsRequest from a JSON string
bulk_upload_posts_request_instance = BulkUploadPostsRequest.from_json(json)
# print the JSON string representation of the object
print(BulkUploadPostsRequest.to_json())

# convert the object into a dict
bulk_upload_posts_request_dict = bulk_upload_posts_request_instance.to_dict()
# create an instance of BulkUploadPostsRequest from a dict
bulk_upload_posts_request_from_dict = BulkUploadPostsRequest.from_dict(bulk_upload_posts_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


