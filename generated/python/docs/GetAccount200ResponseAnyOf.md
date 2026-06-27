# GetAccount200ResponseAnyOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListAccounts200ResponseAnyOfDataAccountsInner**](ListAccounts200ResponseAnyOfDataAccountsInner.md) |  | 

## Example

```python
from kavenio.models.get_account200_response_any_of import GetAccount200ResponseAnyOf

# TODO update the JSON string below
json = "{}"
# create an instance of GetAccount200ResponseAnyOf from a JSON string
get_account200_response_any_of_instance = GetAccount200ResponseAnyOf.from_json(json)
# print the JSON string representation of the object
print(GetAccount200ResponseAnyOf.to_json())

# convert the object into a dict
get_account200_response_any_of_dict = get_account200_response_any_of_instance.to_dict()
# create an instance of GetAccount200ResponseAnyOf from a dict
get_account200_response_any_of_from_dict = GetAccount200ResponseAnyOf.from_dict(get_account200_response_any_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


