# ListYouTubeChannels200ResponseAnyOfDataChannelsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**title** | **str** |  | 
**description** | **str** |  | [optional] 
**custom_url** | **str** |  | [optional] 
**thumbnail_url** | **str** |  | [optional] 
**uploads_playlist_id** | **str** |  | [optional] 
**subscriber_count** | **int** |  | [optional] 
**video_count** | **int** |  | [optional] 
**view_count** | **int** |  | [optional] 
**selected** | **bool** |  | [optional] 
**can_upload** | **bool** |  | [optional] 
**missing_permissions** | **List[str]** |  | [optional] 

## Example

```python
from kavenio.models.list_you_tube_channels200_response_any_of_data_channels_inner import ListYouTubeChannels200ResponseAnyOfDataChannelsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListYouTubeChannels200ResponseAnyOfDataChannelsInner from a JSON string
list_you_tube_channels200_response_any_of_data_channels_inner_instance = ListYouTubeChannels200ResponseAnyOfDataChannelsInner.from_json(json)
# print the JSON string representation of the object
print(ListYouTubeChannels200ResponseAnyOfDataChannelsInner.to_json())

# convert the object into a dict
list_you_tube_channels200_response_any_of_data_channels_inner_dict = list_you_tube_channels200_response_any_of_data_channels_inner_instance.to_dict()
# create an instance of ListYouTubeChannels200ResponseAnyOfDataChannelsInner from a dict
list_you_tube_channels200_response_any_of_data_channels_inner_from_dict = ListYouTubeChannels200ResponseAnyOfDataChannelsInner.from_dict(list_you_tube_channels200_response_any_of_data_channels_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


