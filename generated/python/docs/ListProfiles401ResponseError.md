# ListProfiles401ResponseError


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**code** | **str** |  | 
**message** | **str** |  | 
**details** | **object** |  | [optional] 

## Example

```python
from kavenio.models.list_profiles401_response_error import ListProfiles401ResponseError

# TODO update the JSON string below
json = "{}"
# create an instance of ListProfiles401ResponseError from a JSON string
list_profiles401_response_error_instance = ListProfiles401ResponseError.from_json(json)
# print the JSON string representation of the object
print(ListProfiles401ResponseError.to_json())

# convert the object into a dict
list_profiles401_response_error_dict = list_profiles401_response_error_instance.to_dict()
# create an instance of ListProfiles401ResponseError from a dict
list_profiles401_response_error_from_dict = ListProfiles401ResponseError.from_dict(list_profiles401_response_error_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


