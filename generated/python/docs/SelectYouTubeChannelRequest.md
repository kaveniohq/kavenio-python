# SelectYouTubeChannelRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**profile_id** | **str** |  | [optional] 
**channel_id** | **str** |  | 

## Example

```python
from kavenio.models.select_you_tube_channel_request import SelectYouTubeChannelRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SelectYouTubeChannelRequest from a JSON string
select_you_tube_channel_request_instance = SelectYouTubeChannelRequest.from_json(json)
# print the JSON string representation of the object
print(SelectYouTubeChannelRequest.to_json())

# convert the object into a dict
select_you_tube_channel_request_dict = select_you_tube_channel_request_instance.to_dict()
# create an instance of SelectYouTubeChannelRequest from a dict
select_you_tube_channel_request_from_dict = SelectYouTubeChannelRequest.from_dict(select_you_tube_channel_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


