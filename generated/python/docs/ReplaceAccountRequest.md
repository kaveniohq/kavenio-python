# ReplaceAccountRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**display_name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 
**metadata** | **Dict[str, object]** |  | [optional] 

## Example

```python
from kavenio.models.replace_account_request import ReplaceAccountRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReplaceAccountRequest from a JSON string
replace_account_request_instance = ReplaceAccountRequest.from_json(json)
# print the JSON string representation of the object
print(ReplaceAccountRequest.to_json())

# convert the object into a dict
replace_account_request_dict = replace_account_request_instance.to_dict()
# create an instance of ReplaceAccountRequest from a dict
replace_account_request_from_dict = ReplaceAccountRequest.from_dict(replace_account_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


