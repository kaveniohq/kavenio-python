# ListYouTubeChannels200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**channels** | [**List[ListYouTubeChannels200ResponseAnyOfDataChannelsInner]**](ListYouTubeChannels200ResponseAnyOfDataChannelsInner.md) |  | 
**selected_channel_id** | **str** |  | [optional] 
**fetched_at** | **str** |  | [optional] 
**readiness** | [**ListFacebookPages200ResponseAnyOfDataReadiness**](ListFacebookPages200ResponseAnyOfDataReadiness.md) |  | [optional] 

## Example

```python
from kavenio.models.list_you_tube_channels200_response_any_of_data import ListYouTubeChannels200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of ListYouTubeChannels200ResponseAnyOfData from a JSON string
list_you_tube_channels200_response_any_of_data_instance = ListYouTubeChannels200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(ListYouTubeChannels200ResponseAnyOfData.to_json())

# convert the object into a dict
list_you_tube_channels200_response_any_of_data_dict = list_you_tube_channels200_response_any_of_data_instance.to_dict()
# create an instance of ListYouTubeChannels200ResponseAnyOfData from a dict
list_you_tube_channels200_response_any_of_data_from_dict = ListYouTubeChannels200ResponseAnyOfData.from_dict(list_you_tube_channels200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


