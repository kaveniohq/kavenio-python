# ListAccounts200ResponseAnyOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListAccounts200ResponseAnyOfData**](ListAccounts200ResponseAnyOfData.md) |  | 

## Example

```python
from kavenio.models.list_accounts200_response_any_of import ListAccounts200ResponseAnyOf

# TODO update the JSON string below
json = "{}"
# create an instance of ListAccounts200ResponseAnyOf from a JSON string
list_accounts200_response_any_of_instance = ListAccounts200ResponseAnyOf.from_json(json)
# print the JSON string representation of the object
print(ListAccounts200ResponseAnyOf.to_json())

# convert the object into a dict
list_accounts200_response_any_of_dict = list_accounts200_response_any_of_instance.to_dict()
# create an instance of ListAccounts200ResponseAnyOf from a dict
list_accounts200_response_any_of_from_dict = ListAccounts200ResponseAnyOf.from_dict(list_accounts200_response_any_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


