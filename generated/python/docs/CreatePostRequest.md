# CreatePostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**content** | **str** |  | [optional] 
**media_items** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**platforms** | [**List[CreatePostRequestPlatformsInner]**](CreatePostRequestPlatformsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**publish_now** | **bool** |  | [optional] 
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
from kavenio.models.create_post_request import CreatePostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequest from a JSON string
create_post_request_instance = CreatePostRequest.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequest.to_json())

# convert the object into a dict
create_post_request_dict = create_post_request_instance.to_dict()
# create an instance of CreatePostRequest from a dict
create_post_request_from_dict = CreatePostRequest.from_dict(create_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


