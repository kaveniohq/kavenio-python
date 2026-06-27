# CheckAccountHealth200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**CheckAccountHealth200ResponseAnyOfData**](CheckAccountHealth200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.check_account_health200_response import CheckAccountHealth200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CheckAccountHealth200Response from a JSON string
check_account_health200_response_instance = CheckAccountHealth200Response.from_json(json)
# print the JSON string representation of the object
print(CheckAccountHealth200Response.to_json())

# convert the object into a dict
check_account_health200_response_dict = check_account_health200_response_instance.to_dict()
# create an instance of CheckAccountHealth200Response from a dict
check_account_health200_response_from_dict = CheckAccountHealth200Response.from_dict(check_account_health200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


