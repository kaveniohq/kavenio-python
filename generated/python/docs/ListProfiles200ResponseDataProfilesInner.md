# ListProfiles200ResponseDataProfilesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**organization_id** | **str** |  | 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**color** | **str** |  | [optional] 
**is_default** | **bool** |  | 
**created_by** | **str** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from kavenio.models.list_profiles200_response_data_profiles_inner import ListProfiles200ResponseDataProfilesInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListProfiles200ResponseDataProfilesInner from a JSON string
list_profiles200_response_data_profiles_inner_instance = ListProfiles200ResponseDataProfilesInner.from_json(json)
# print the JSON string representation of the object
print(ListProfiles200ResponseDataProfilesInner.to_json())

# convert the object into a dict
list_profiles200_response_data_profiles_inner_dict = list_profiles200_response_data_profiles_inner_instance.to_dict()
# create an instance of ListProfiles200ResponseDataProfilesInner from a dict
list_profiles200_response_data_profiles_inner_from_dict = ListProfiles200ResponseDataProfilesInner.from_dict(list_profiles200_response_data_profiles_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


