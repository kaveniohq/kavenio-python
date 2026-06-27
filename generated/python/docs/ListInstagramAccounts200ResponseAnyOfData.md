# ListInstagramAccounts200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**accounts** | [**List[ListInstagramAccounts200ResponseAnyOfDataAccountsInner]**](ListInstagramAccounts200ResponseAnyOfDataAccountsInner.md) |  | 
**selected_instagram_account_id** | **str** |  | [optional] 
**fetched_at** | **str** |  | [optional] 
**readiness** | [**ListFacebookPages200ResponseAnyOfDataReadiness**](ListFacebookPages200ResponseAnyOfDataReadiness.md) |  | [optional] 

## Example

```python
from kavenio.models.list_instagram_accounts200_response_any_of_data import ListInstagramAccounts200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of ListInstagramAccounts200ResponseAnyOfData from a JSON string
list_instagram_accounts200_response_any_of_data_instance = ListInstagramAccounts200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(ListInstagramAccounts200ResponseAnyOfData.to_json())

# convert the object into a dict
list_instagram_accounts200_response_any_of_data_dict = list_instagram_accounts200_response_any_of_data_instance.to_dict()
# create an instance of ListInstagramAccounts200ResponseAnyOfData from a dict
list_instagram_accounts200_response_any_of_data_from_dict = ListInstagramAccounts200ResponseAnyOfData.from_dict(list_instagram_accounts200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


