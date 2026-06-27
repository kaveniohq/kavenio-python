# DeletePost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**DeletePost200ResponseAnyOfData**](DeletePost200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.delete_post200_response import DeletePost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of DeletePost200Response from a JSON string
delete_post200_response_instance = DeletePost200Response.from_json(json)
# print the JSON string representation of the object
print(DeletePost200Response.to_json())

# convert the object into a dict
delete_post200_response_dict = delete_post200_response_instance.to_dict()
# create an instance of DeletePost200Response from a dict
delete_post200_response_from_dict = DeletePost200Response.from_dict(delete_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


