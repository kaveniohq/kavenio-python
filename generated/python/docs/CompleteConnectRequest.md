# CompleteConnectRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform** | **str** |  | [optional] 
**state** | **str** |  | 
**code** | **str** |  | 
**callback_url** | **str** |  | [optional] 

## Example

```python
from kavenio.models.complete_connect_request import CompleteConnectRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CompleteConnectRequest from a JSON string
complete_connect_request_instance = CompleteConnectRequest.from_json(json)
# print the JSON string representation of the object
print(CompleteConnectRequest.to_json())

# convert the object into a dict
complete_connect_request_dict = complete_connect_request_instance.to_dict()
# create an instance of CompleteConnectRequest from a dict
complete_connect_request_from_dict = CompleteConnectRequest.from_dict(complete_connect_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


