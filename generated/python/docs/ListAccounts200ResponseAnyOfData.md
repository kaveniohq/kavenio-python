# ListAccounts200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accounts** | [**List[ListAccounts200ResponseAnyOfDataAccountsInner]**](ListAccounts200ResponseAnyOfDataAccountsInner.md) |  | 
**next_cursor** | **str** |  | [optional] 

## Example

```python
from kavenio.models.list_accounts200_response_any_of_data import ListAccounts200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of ListAccounts200ResponseAnyOfData from a JSON string
list_accounts200_response_any_of_data_instance = ListAccounts200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(ListAccounts200ResponseAnyOfData.to_json())

# convert the object into a dict
list_accounts200_response_any_of_data_dict = list_accounts200_response_any_of_data_instance.to_dict()
# create an instance of ListAccounts200ResponseAnyOfData from a dict
list_accounts200_response_any_of_data_from_dict = ListAccounts200ResponseAnyOfData.from_dict(list_accounts200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


