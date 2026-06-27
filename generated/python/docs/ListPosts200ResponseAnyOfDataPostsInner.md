# ListPosts200ResponseAnyOfDataPostsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**organization_id** | **str** |  | 
**profile_id** | **str** |  | [optional] 
**created_by** | **str** |  | 
**title** | **str** |  | [optional] 
**content** | **str** |  | [optional] 
**status** | **str** |  | 
**scheduled_for** | **datetime** |  | [optional] 
**published_at** | **datetime** |  | [optional] 
**timezone** | **str** |  | [optional] 
**media_items** | [**List[ListPosts200ResponseAnyOfDataPostsInnerMediaItemsInner]**](ListPosts200ResponseAnyOfDataPostsInnerMediaItemsInner.md) |  | 
**tags** | **List[str]** |  | 
**hashtags** | **List[str]** |  | 
**mentions** | **List[str]** |  | 
**metadata** | **Dict[str, object]** |  | 
**crossposting_enabled** | **bool** |  | 
**queued_from_profile** | **str** |  | [optional] 
**queue_id** | **str** |  | [optional] 
**recycling** | [**ListPosts200ResponseAnyOfDataPostsInnerRecycling**](ListPosts200ResponseAnyOfDataPostsInnerRecycling.md) |  | [optional] 
**targets** | [**List[ListPosts200ResponseAnyOfDataPostsInnerTargetsInner]**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInner.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 

## Example

```python
from kavenio.models.list_posts200_response_any_of_data_posts_inner import ListPosts200ResponseAnyOfDataPostsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListPosts200ResponseAnyOfDataPostsInner from a JSON string
list_posts200_response_any_of_data_posts_inner_instance = ListPosts200ResponseAnyOfDataPostsInner.from_json(json)
# print the JSON string representation of the object
print(ListPosts200ResponseAnyOfDataPostsInner.to_json())

# convert the object into a dict
list_posts200_response_any_of_data_posts_inner_dict = list_posts200_response_any_of_data_posts_inner_instance.to_dict()
# create an instance of ListPosts200ResponseAnyOfDataPostsInner from a dict
list_posts200_response_any_of_data_posts_inner_from_dict = ListPosts200ResponseAnyOfDataPostsInner.from_dict(list_posts200_response_any_of_data_posts_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


