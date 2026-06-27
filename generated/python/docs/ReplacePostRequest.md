# ReplacePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**content** | **str** |  | [optional] 
**media_items** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**platforms** | [**List[CreatePostRequestPlatformsInner]**](CreatePostRequestPlatformsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**is_draft** | **bool** |  | [optional] 
**timezone** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] 
**hashtags** | **List[str]** |  | [optional] 
**mentions** | **List[str]** |  | [optional] 
**crossposting_enabled** | **bool** |  | [optional] 
**facebook_settings** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7.md) |  | [optional] 
**tiktok_settings** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf10**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf10.md) |  | [optional] 
**metadata** | **Dict[str, object]** |  | [optional] 
**recycling** | [**CreatePostRequestRecycling**](CreatePostRequestRecycling.md) |  | [optional] 
**queued_from_profile** | **str** |  | [optional] 
**queue_id** | **str** |  | [optional] 

## Example

```python
from kavenio.models.replace_post_request import ReplacePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ReplacePostRequest from a JSON string
replace_post_request_instance = ReplacePostRequest.from_json(json)
# print the JSON string representation of the object
print(ReplacePostRequest.to_json())

# convert the object into a dict
replace_post_request_dict = replace_post_request_instance.to_dict()
# create an instance of ReplacePostRequest from a dict
replace_post_request_from_dict = ReplacePostRequest.from_dict(replace_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


