# CreatePostRequestPlatformsInnerOneOfPlatformSpecificData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**reply_to_tweet_id** | **str** |  | [optional] 
**quote_tweet_id** | **str** |  | [optional] 
**media_ids** | **List[str]** |  | [optional] 
**reply_settings** | **str** |  | [optional] 
**thread_items** | [**List[CreatePostRequestPlatformsInnerOneOfPlatformSpecificDataThreadItemsInner]**](CreatePostRequestPlatformsInnerOneOfPlatformSpecificDataThreadItemsInner.md) |  | [optional] 
**poll** | [**CreatePostRequestPlatformsInnerOneOfPlatformSpecificDataPoll**](CreatePostRequestPlatformsInnerOneOfPlatformSpecificDataPoll.md) |  | [optional] 
**long_video** | **bool** |  | [optional] 
**paid_partnership** | **bool** |  | [optional] 
**made_with_ai** | **bool** |  | [optional] 
**first_comment** | **str** |  | [optional] 
**sensitive_media** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOfSensitiveMedia**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOfSensitiveMedia.md) |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of_platform_specific_data import CreatePostRequestPlatformsInnerOneOfPlatformSpecificData

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOfPlatformSpecificData from a JSON string
create_post_request_platforms_inner_one_of_platform_specific_data_instance = CreatePostRequestPlatformsInnerOneOfPlatformSpecificData.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOfPlatformSpecificData.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of_platform_specific_data_dict = create_post_request_platforms_inner_one_of_platform_specific_data_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOfPlatformSpecificData from a dict
create_post_request_platforms_inner_one_of_platform_specific_data_from_dict = CreatePostRequestPlatformsInnerOneOfPlatformSpecificData.from_dict(create_post_request_platforms_inner_one_of_platform_specific_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


