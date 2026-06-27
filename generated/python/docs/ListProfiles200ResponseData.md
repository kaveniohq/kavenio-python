# ListProfiles200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profiles** | [**List[ListProfiles200ResponseDataProfilesInner]**](ListProfiles200ResponseDataProfilesInner.md) |  | 

## Example

```python
from kavenio.models.list_profiles200_response_data import ListProfiles200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ListProfiles200ResponseData from a JSON string
list_profiles200_response_data_instance = ListProfiles200ResponseData.from_json(json)
# print the JSON string representation of the object
print(ListProfiles200ResponseData.to_json())

# convert the object into a dict
list_profiles200_response_data_dict = list_profiles200_response_data_instance.to_dict()
# create an instance of ListProfiles200ResponseData from a dict
list_profiles200_response_data_from_dict = ListProfiles200ResponseData.from_dict(list_profiles200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


