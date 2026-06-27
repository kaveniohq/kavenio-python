# ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page_id** | **str** |  | [optional] 
**content_type** | **str** |  | [optional] 
**first_comment** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**reel_title** | **str** |  | [optional] 
**link** | **str** |  | [optional] 
**carousel_link** | **str** |  | [optional] 
**carousel_cards** | [**List[ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7CarouselCardsInner]**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7CarouselCardsInner.md) |  | [optional] 
**unpublished_content_type** | **str** |  | [optional] 
**draft** | **bool** |  | [optional] 
**scheduled_publish_time** | **datetime** |  | [optional] 
**geo_restriction** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7GeoRestriction**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7GeoRestriction.md) |  | [optional] 
**geo_restrictions** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7GeoRestriction**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7GeoRestriction.md) |  | [optional] 
**multi_page_targets** | **List[str]** |  | [optional] 

## Example

```python
from kavenio.models.list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of7 import ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7

# TODO update the JSON string below
json = "{}"
# create an instance of ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7 from a JSON string
list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of7_instance = ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7.from_json(json)
# print the JSON string representation of the object
print(ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7.to_json())

# convert the object into a dict
list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of7_dict = list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of7_instance.to_dict()
# create an instance of ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7 from a dict
list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of7_from_dict = ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf7.from_dict(list_posts200_response_any_of_data_posts_inner_targets_inner_platform_specific_data_any_of7_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


