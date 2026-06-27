# ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**key** | **str** |  | 
**supported** | **bool** |  | 
**status** | **str** |  | [optional] 
**reason** | **str** |  | [optional] 
**required_scopes** | **List[str]** |  | [optional] 
**required_permissions** | **List[str]** |  | [optional] 

## Example

```python
from kavenio.models.list_facebook_pages200_response_any_of_data_readiness_capabilities_inner import ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner from a JSON string
list_facebook_pages200_response_any_of_data_readiness_capabilities_inner_instance = ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner.from_json(json)
# print the JSON string representation of the object
print(ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner.to_json())

# convert the object into a dict
list_facebook_pages200_response_any_of_data_readiness_capabilities_inner_dict = list_facebook_pages200_response_any_of_data_readiness_capabilities_inner_instance.to_dict()
# create an instance of ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner from a dict
list_facebook_pages200_response_any_of_data_readiness_capabilities_inner_from_dict = ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner.from_dict(list_facebook_pages200_response_any_of_data_readiness_capabilities_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


