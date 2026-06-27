# ListProfiles200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListProfiles200ResponseData**](ListProfiles200ResponseData.md) |  | 

## Example

```python
from kavenio.models.list_profiles200_response import ListProfiles200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListProfiles200Response from a JSON string
list_profiles200_response_instance = ListProfiles200Response.from_json(json)
# print the JSON string representation of the object
print(ListProfiles200Response.to_json())

# convert the object into a dict
list_profiles200_response_dict = list_profiles200_response_instance.to_dict()
# create an instance of ListProfiles200Response from a dict
list_profiles200_response_from_dict = ListProfiles200Response.from_dict(list_profiles200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


