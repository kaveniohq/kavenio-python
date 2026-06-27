# CheckAccountHealth200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account** | [**ListAccounts200ResponseAnyOfDataAccountsInner**](ListAccounts200ResponseAnyOfDataAccountsInner.md) |  | 
**healthy** | **bool** |  | 
**checked_at** | **str** |  | 
**issues** | [**List[ListFacebookPages200ResponseAnyOfDataReadinessIssuesInner]**](ListFacebookPages200ResponseAnyOfDataReadinessIssuesInner.md) |  | 
**readiness** | [**ListFacebookPages200ResponseAnyOfDataReadiness**](ListFacebookPages200ResponseAnyOfDataReadiness.md) |  | [optional] 

## Example

```python
from kavenio.models.check_account_health200_response_any_of_data import CheckAccountHealth200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of CheckAccountHealth200ResponseAnyOfData from a JSON string
check_account_health200_response_any_of_data_instance = CheckAccountHealth200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(CheckAccountHealth200ResponseAnyOfData.to_json())

# convert the object into a dict
check_account_health200_response_any_of_data_dict = check_account_health200_response_any_of_data_instance.to_dict()
# create an instance of CheckAccountHealth200ResponseAnyOfData from a dict
check_account_health200_response_any_of_data_from_dict = CheckAccountHealth200ResponseAnyOfData.from_dict(check_account_health200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


