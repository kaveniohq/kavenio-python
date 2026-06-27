# CreateMediaPresign200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**CreateMediaPresign200ResponseData**](CreateMediaPresign200ResponseData.md) |  | 

## Example

```python
from kavenio.models.create_media_presign200_response import CreateMediaPresign200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateMediaPresign200Response from a JSON string
create_media_presign200_response_instance = CreateMediaPresign200Response.from_json(json)
# print the JSON string representation of the object
print(CreateMediaPresign200Response.to_json())

# convert the object into a dict
create_media_presign200_response_dict = create_media_presign200_response_instance.to_dict()
# create an instance of CreateMediaPresign200Response from a dict
create_media_presign200_response_from_dict = CreateMediaPresign200Response.from_dict(create_media_presign200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


