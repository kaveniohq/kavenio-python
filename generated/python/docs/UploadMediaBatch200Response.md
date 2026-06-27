# UploadMediaBatch200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**UploadMediaBatch200ResponseData**](UploadMediaBatch200ResponseData.md) |  | 

## Example

```python
from kavenio.models.upload_media_batch200_response import UploadMediaBatch200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UploadMediaBatch200Response from a JSON string
upload_media_batch200_response_instance = UploadMediaBatch200Response.from_json(json)
# print the JSON string representation of the object
print(UploadMediaBatch200Response.to_json())

# convert the object into a dict
upload_media_batch200_response_dict = upload_media_batch200_response_instance.to_dict()
# create an instance of UploadMediaBatch200Response from a dict
upload_media_batch200_response_from_dict = UploadMediaBatch200Response.from_dict(upload_media_batch200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


