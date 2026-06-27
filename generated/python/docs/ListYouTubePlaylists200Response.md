# ListYouTubePlaylists200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListYouTubePlaylists200ResponseAnyOfData**](ListYouTubePlaylists200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.list_you_tube_playlists200_response import ListYouTubePlaylists200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListYouTubePlaylists200Response from a JSON string
list_you_tube_playlists200_response_instance = ListYouTubePlaylists200Response.from_json(json)
# print the JSON string representation of the object
print(ListYouTubePlaylists200Response.to_json())

# convert the object into a dict
list_you_tube_playlists200_response_dict = list_you_tube_playlists200_response_instance.to_dict()
# create an instance of ListYouTubePlaylists200Response from a dict
list_you_tube_playlists200_response_from_dict = ListYouTubePlaylists200Response.from_dict(list_you_tube_playlists200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


