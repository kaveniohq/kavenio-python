# UploadMediaBatchRequestItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_name** | **str** |  | 
**content_type** | **str** |  | 
**base64_data** | **str** |  | 

## Example

```python
from kavenio.models.upload_media_batch_request_items_inner import UploadMediaBatchRequestItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of UploadMediaBatchRequestItemsInner from a JSON string
upload_media_batch_request_items_inner_instance = UploadMediaBatchRequestItemsInner.from_json(json)
# print the JSON string representation of the object
print(UploadMediaBatchRequestItemsInner.to_json())

# convert the object into a dict
upload_media_batch_request_items_inner_dict = upload_media_batch_request_items_inner_instance.to_dict()
# create an instance of UploadMediaBatchRequestItemsInner from a dict
upload_media_batch_request_items_inner_from_dict = UploadMediaBatchRequestItemsInner.from_dict(upload_media_batch_request_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


