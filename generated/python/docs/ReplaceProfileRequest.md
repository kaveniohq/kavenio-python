# ReplaceProfileRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**color** | **str** |  | [optional] 
**is_default** | **bool** |  | [optional] 

## Example

```python
from kavenio.models.replace_profile_request import ReplaceProfileRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReplaceProfileRequest from a JSON string
replace_profile_request_instance = ReplaceProfileRequest.from_json(json)
# print the JSON string representation of the object
print(ReplaceProfileRequest.to_json())

# convert the object into a dict
replace_profile_request_dict = replace_profile_request_instance.to_dict()
# create an instance of ReplaceProfileRequest from a dict
replace_profile_request_from_dict = ReplaceProfileRequest.from_dict(replace_profile_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


