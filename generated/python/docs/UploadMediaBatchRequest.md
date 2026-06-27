# UploadMediaBatchRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**items** | [**List[UploadMediaBatchRequestItemsInner]**](UploadMediaBatchRequestItemsInner.md) |  | 

## Example

```python
from kavenio.models.upload_media_batch_request import UploadMediaBatchRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UploadMediaBatchRequest from a JSON string
upload_media_batch_request_instance = UploadMediaBatchRequest.from_json(json)
# print the JSON string representation of the object
print(UploadMediaBatchRequest.to_json())

# convert the object into a dict
upload_media_batch_request_dict = upload_media_batch_request_instance.to_dict()
# create an instance of UploadMediaBatchRequest from a dict
upload_media_batch_request_from_dict = UploadMediaBatchRequest.from_dict(upload_media_batch_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


