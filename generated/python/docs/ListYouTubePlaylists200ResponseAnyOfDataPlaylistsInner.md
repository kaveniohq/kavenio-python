# ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**channel_id** | **str** |  | 
**title** | **str** |  | 
**description** | **str** |  | [optional] 
**privacy_status** | **str** |  | [optional] 
**thumbnail_url** | **str** |  | [optional] 
**item_count** | **int** |  | [optional] 

## Example

```python
from kavenio.models.list_you_tube_playlists200_response_any_of_data_playlists_inner import ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner from a JSON string
list_you_tube_playlists200_response_any_of_data_playlists_inner_instance = ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner.from_json(json)
# print the JSON string representation of the object
print(ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner.to_json())

# convert the object into a dict
list_you_tube_playlists200_response_any_of_data_playlists_inner_dict = list_you_tube_playlists200_response_any_of_data_playlists_inner_instance.to_dict()
# create an instance of ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner from a dict
list_you_tube_playlists200_response_any_of_data_playlists_inner_from_dict = ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner.from_dict(list_you_tube_playlists200_response_any_of_data_playlists_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


