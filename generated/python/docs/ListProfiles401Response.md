# ListProfiles401Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.list_profiles401_response import ListProfiles401Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListProfiles401Response from a JSON string
list_profiles401_response_instance = ListProfiles401Response.from_json(json)
# print the JSON string representation of the object
print(ListProfiles401Response.to_json())

# convert the object into a dict
list_profiles401_response_dict = list_profiles401_response_instance.to_dict()
# create an instance of ListProfiles401Response from a dict
list_profiles401_response_from_dict = ListProfiles401Response.from_dict(list_profiles401_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


