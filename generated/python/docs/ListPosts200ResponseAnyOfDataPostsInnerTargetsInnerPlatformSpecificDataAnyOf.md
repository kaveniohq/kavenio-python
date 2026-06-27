# ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reply_to_tweet_id** | **str** |  | [optional] 
**quote_tweet_id** | **str** |  | [optional] 
**media_ids** | **List[str]** |  | [optional] 
**reply_settings** | **str** |  | [optional] 
**thread_items** | [**List[ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOfThreadItemsInner]**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOfThreadItemsInner.md) |  | [optional] 
**poll** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOfPoll**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOfPoll.md) |  | [optional] 
**long_video** | **bool** |  | [optional] 
**paid_partnership** | **bool** |  | [optional] 
**made_with_ai** | **bool** |  | [optional] 
**first_comment** | **str** |  | [optional] 
**sensitive_media** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOfSensitiveMedia**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOfSensitiveMedia.md) |  | [optional] 

## Example

```python
from kavenio.models.list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of import ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf

# TODO update the JSON string below
json = "{}"
# create an instance of ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf from a JSON string
list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of_instance = ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf.from_json(json)
# print the JSON string representation of the object
print(ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf.to_json())

# convert the object into a dict
list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of_dict = list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of_instance.to_dict()
# create an instance of ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf from a dict
list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of_from_dict = ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf.from_dict(list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


