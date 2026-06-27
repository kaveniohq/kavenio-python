# ListYouTubePlaylists200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**channel_id** | **str** |  | 
**playlists** | [**List[ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner]**](ListYouTubePlaylists200ResponseAnyOfDataPlaylistsInner.md) |  | 
**fetched_at** | **str** |  | [optional] 

## Example

```python
from kavenio.models.list_you_tube_playlists200_response_any_of_data import ListYouTubePlaylists200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of ListYouTubePlaylists200ResponseAnyOfData from a JSON string
list_you_tube_playlists200_response_any_of_data_instance = ListYouTubePlaylists200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(ListYouTubePlaylists200ResponseAnyOfData.to_json())

# convert the object into a dict
list_you_tube_playlists200_response_any_of_data_dict = list_you_tube_playlists200_response_any_of_data_instance.to_dict()
# create an instance of ListYouTubePlaylists200ResponseAnyOfData from a dict
list_you_tube_playlists200_response_any_of_data_from_dict = ListYouTubePlaylists200ResponseAnyOfData.from_dict(list_you_tube_playlists200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


