# CreateMediaPresign200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**upload_url** | **str** |  | 
**public_url** | **str** |  | 
**key** | **str** |  | 
**expires_in** | **int** |  | 

## Example

```python
from kavenio.models.create_media_presign200_response_data import CreateMediaPresign200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of CreateMediaPresign200ResponseData from a JSON string
create_media_presign200_response_data_instance = CreateMediaPresign200ResponseData.from_json(json)
# print the JSON string representation of the object
print(CreateMediaPresign200ResponseData.to_json())

# convert the object into a dict
create_media_presign200_response_data_dict = create_media_presign200_response_data_instance.to_dict()
# create an instance of CreateMediaPresign200ResponseData from a dict
create_media_presign200_response_data_from_dict = CreateMediaPresign200ResponseData.from_dict(create_media_presign200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


