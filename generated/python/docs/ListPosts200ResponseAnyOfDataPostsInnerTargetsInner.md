# ListPosts200ResponseAnyOfDataPostsInnerTargetsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**post_id** | **str** |  | 
**platform** | **str** |  | 
**account_id** | **str** |  | [optional] 
**status** | **str** |  | 
**custom_content** | **str** |  | [optional] 
**custom_media** | [**List[ListPosts200ResponseAnyOfDataPostsInnerMediaItemsInner]**](ListPosts200ResponseAnyOfDataPostsInnerMediaItemsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**platform_specific_data** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificData**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificData.md) |  | [optional] 
**platform_post_id** | **str** |  | [optional] 
**native_url** | **str** |  | [optional] 
**error** | **str** |  | [optional] 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 

## Example

```python
from kavenio.models.list_posts200_response_any_of_data_posts_inner_targets_inner import ListPosts200ResponseAnyOfDataPostsInnerTargetsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListPosts200ResponseAnyOfDataPostsInnerTargetsInner from a JSON string
list_posts200_response_any_of_data_posts_inner_targets_inner_instance = ListPosts200ResponseAnyOfDataPostsInnerTargetsInner.from_json(json)
# print the JSON string representation of the object
print(ListPosts200ResponseAnyOfDataPostsInnerTargetsInner.to_json())

# convert the object into a dict
list_posts200_response_any_of_data_posts_inner_targets_inner_dict = list_posts200_response_any_of_data_posts_inner_targets_inner_instance.to_dict()
# create an instance of ListPosts200ResponseAnyOfDataPostsInnerTargetsInner from a dict
list_posts200_response_any_of_data_posts_inner_targets_inner_from_dict = ListPosts200ResponseAnyOfDataPostsInnerTargetsInner.from_dict(list_posts200_response_any_of_data_posts_inner_targets_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


