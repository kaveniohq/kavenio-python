# ListInstagramAccounts200ResponseAnyOfDataAccountsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**username** | **str** |  | 
**display_name** | **str** |  | [optional] 
**account_type** | **str** |  | 
**connected_facebook_page_id** | **str** |  | [optional] 
**connected_facebook_page_name** | **str** |  | [optional] 
**profile_picture_url** | **str** |  | [optional] 
**selected** | **bool** |  | [optional] 
**can_publish** | **bool** |  | [optional] 
**missing_permissions** | **List[str]** |  | [optional] 

## Example

```python
from kavenio.models.list_instagram_accounts200_response_any_of_data_accounts_inner import ListInstagramAccounts200ResponseAnyOfDataAccountsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListInstagramAccounts200ResponseAnyOfDataAccountsInner from a JSON string
list_instagram_accounts200_response_any_of_data_accounts_inner_instance = ListInstagramAccounts200ResponseAnyOfDataAccountsInner.from_json(json)
# print the JSON string representation of the object
print(ListInstagramAccounts200ResponseAnyOfDataAccountsInner.to_json())

# convert the object into a dict
list_instagram_accounts200_response_any_of_data_accounts_inner_dict = list_instagram_accounts200_response_any_of_data_accounts_inner_instance.to_dict()
# create an instance of ListInstagramAccounts200ResponseAnyOfDataAccountsInner from a dict
list_instagram_accounts200_response_any_of_data_accounts_inner_from_dict = ListInstagramAccounts200ResponseAnyOfDataAccountsInner.from_dict(list_instagram_accounts200_response_any_of_data_accounts_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


