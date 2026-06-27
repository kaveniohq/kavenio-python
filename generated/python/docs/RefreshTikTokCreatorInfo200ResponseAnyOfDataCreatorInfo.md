# RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**creator_username** | **str** |  | [optional] 
**display_name** | **str** |  | [optional] 
**avatar_url** | **str** |  | [optional] 
**privacy_levels** | **List[str]** |  | 
**comment_allowed** | **bool** |  | [optional] 
**duet_allowed** | **bool** |  | [optional] 
**stitch_allowed** | **bool** |  | [optional] 
**max_video_duration_seconds** | **int** |  | [optional] 
**max_caption_length** | **int** |  | [optional] 
**can_post** | **bool** |  | 
**fetched_at** | **str** |  | [optional] 
**expires_at** | **str** |  | [optional] 
**warnings** | **List[str]** |  | [optional] 

## Example

```python
from kavenio.models.refresh_tik_tok_creator_info200_response_any_of_data_creator_info import RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo

# TODO update the JSON string below
json = "{}"
# create an instance of RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo from a JSON string
refresh_tik_tok_creator_info200_response_any_of_data_creator_info_instance = RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo.from_json(json)
# print the JSON string representation of the object
print(RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo.to_json())

# convert the object into a dict
refresh_tik_tok_creator_info200_response_any_of_data_creator_info_dict = refresh_tik_tok_creator_info200_response_any_of_data_creator_info_instance.to_dict()
# create an instance of RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo from a dict
refresh_tik_tok_creator_info200_response_any_of_data_creator_info_from_dict = RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo.from_dict(refresh_tik_tok_creator_info200_response_any_of_data_creator_info_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


