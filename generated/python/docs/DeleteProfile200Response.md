# DeleteProfile200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**DeleteProfile200ResponseData**](DeleteProfile200ResponseData.md) |  | 

## Example

```python
from kavenio.models.delete_profile200_response import DeleteProfile200Response

# TODO update the JSON string below
json = "{}"
# create an instance of DeleteProfile200Response from a JSON string
delete_profile200_response_instance = DeleteProfile200Response.from_json(json)
# print the JSON string representation of the object
print(DeleteProfile200Response.to_json())

# convert the object into a dict
delete_profile200_response_dict = delete_profile200_response_instance.to_dict()
# create an instance of DeleteProfile200Response from a dict
delete_profile200_response_from_dict = DeleteProfile200Response.from_dict(delete_profile200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


