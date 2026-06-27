# CreateMediaPresignRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**filename** | **str** |  | 
**content_type** | **str** |  | 
**size** | **int** |  | [optional] 

## Example

```python
from kavenio.models.create_media_presign_request import CreateMediaPresignRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateMediaPresignRequest from a JSON string
create_media_presign_request_instance = CreateMediaPresignRequest.from_json(json)
# print the JSON string representation of the object
print(CreateMediaPresignRequest.to_json())

# convert the object into a dict
create_media_presign_request_dict = create_media_presign_request_instance.to_dict()
# create an instance of CreateMediaPresignRequest from a dict
create_media_presign_request_from_dict = CreateMediaPresignRequest.from_dict(create_media_presign_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


