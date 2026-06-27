# BeginConnectRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | 
**platform** | **str** |  | 
**callback_url** | **str** |  | [optional] 
**return_to** | **str** |  | [optional] 
**mastodon_instance** | **str** |  | [optional] 

## Example

```python
from kavenio.models.begin_connect_request import BeginConnectRequest

# TODO update the JSON string below
json = "{}"
# create an instance of BeginConnectRequest from a JSON string
begin_connect_request_instance = BeginConnectRequest.from_json(json)
# print the JSON string representation of the object
print(BeginConnectRequest.to_json())

# convert the object into a dict
begin_connect_request_dict = begin_connect_request_instance.to_dict()
# create an instance of BeginConnectRequest from a dict
begin_connect_request_from_dict = BeginConnectRequest.from_dict(begin_connect_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


