# ListConnectProviders200ResponseAnyOfDataProvidersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform** | **str** |  | 
**label** | **str** |  | 
**connect_mode** | **str** |  | 
**configured** | **bool** |  | 
**effective_credential** | [**ListConnectProviders200ResponseAnyOfDataProvidersInnerEffectiveCredential**](ListConnectProviders200ResponseAnyOfDataProvidersInnerEffectiveCredential.md) |  | [optional] 

## Example

```python
from kavenio.models.list_connect_providers200_response_any_of_data_providers_inner import ListConnectProviders200ResponseAnyOfDataProvidersInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListConnectProviders200ResponseAnyOfDataProvidersInner from a JSON string
list_connect_providers200_response_any_of_data_providers_inner_instance = ListConnectProviders200ResponseAnyOfDataProvidersInner.from_json(json)
# print the JSON string representation of the object
print(ListConnectProviders200ResponseAnyOfDataProvidersInner.to_json())

# convert the object into a dict
list_connect_providers200_response_any_of_data_providers_inner_dict = list_connect_providers200_response_any_of_data_providers_inner_instance.to_dict()
# create an instance of ListConnectProviders200ResponseAnyOfDataProvidersInner from a dict
list_connect_providers200_response_any_of_data_providers_inner_from_dict = ListConnectProviders200ResponseAnyOfDataProvidersInner.from_dict(list_connect_providers200_response_any_of_data_providers_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


