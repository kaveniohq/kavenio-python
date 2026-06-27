# MoveAccountRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | 

## Example

```python
from kavenio.models.move_account_request import MoveAccountRequest

# TODO update the JSON string below
json = "{}"
# create an instance of MoveAccountRequest from a JSON string
move_account_request_instance = MoveAccountRequest.from_json(json)
# print the JSON string representation of the object
print(MoveAccountRequest.to_json())

# convert the object into a dict
move_account_request_dict = move_account_request_instance.to_dict()
# create an instance of MoveAccountRequest from a dict
move_account_request_from_dict = MoveAccountRequest.from_dict(move_account_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


