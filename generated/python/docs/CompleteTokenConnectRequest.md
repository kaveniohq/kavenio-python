# CompleteTokenConnectRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | 
**platform** | **str** |  | 
**oauth_token** | **str** |  | 
**oauth_token_secret** | **str** |  | 
**provider_account_id** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 

## Example

```python
from kavenio.models.complete_token_connect_request import CompleteTokenConnectRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CompleteTokenConnectRequest from a JSON string
complete_token_connect_request_instance = CompleteTokenConnectRequest.from_json(json)
# print the JSON string representation of the object
print(CompleteTokenConnectRequest.to_json())

# convert the object into a dict
complete_token_connect_request_dict = complete_token_connect_request_instance.to_dict()
# create an instance of CompleteTokenConnectRequest from a dict
complete_token_connect_request_from_dict = CompleteTokenConnectRequest.from_dict(complete_token_connect_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


