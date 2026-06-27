# ListAccounts200ResponseAnyOfDataAccountsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**organization_id** | **str** |  | 
**profile_id** | **str** |  | 
**platform** | **str** |  | 
**provider_account_id** | **str** |  | 
**username** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**profile_picture** | **str** |  | [optional] 
**profile_url** | **str** |  | [optional] 
**parent_account_id** | **str** |  | [optional] 
**enabled** | **bool** |  | 
**is_active** | **bool** |  | 
**status** | **str** |  | 
**token_expires_at** | **str** |  | [optional] 
**scopes** | **List[str]** |  | 
**permissions** | **List[str]** |  | 
**metadata** | **Dict[str, object]** |  | 
**readiness** | [**ListFacebookPages200ResponseAnyOfDataReadiness**](ListFacebookPages200ResponseAnyOfDataReadiness.md) |  | [optional] 
**ad_accounts_cache_expires_at** | **str** |  | [optional] 
**last_error** | **str** |  | [optional] 
**last_health_checked_at** | **str** |  | [optional] 
**created_by** | **str** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from kavenio.models.list_accounts200_response_any_of_data_accounts_inner import ListAccounts200ResponseAnyOfDataAccountsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListAccounts200ResponseAnyOfDataAccountsInner from a JSON string
list_accounts200_response_any_of_data_accounts_inner_instance = ListAccounts200ResponseAnyOfDataAccountsInner.from_json(json)
# print the JSON string representation of the object
print(ListAccounts200ResponseAnyOfDataAccountsInner.to_json())

# convert the object into a dict
list_accounts200_response_any_of_data_accounts_inner_dict = list_accounts200_response_any_of_data_accounts_inner_instance.to_dict()
# create an instance of ListAccounts200ResponseAnyOfDataAccountsInner from a dict
list_accounts200_response_any_of_data_accounts_inner_from_dict = ListAccounts200ResponseAnyOfDataAccountsInner.from_dict(list_accounts200_response_any_of_data_accounts_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


