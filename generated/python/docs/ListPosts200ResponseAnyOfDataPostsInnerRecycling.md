# ListPosts200ResponseAnyOfDataPostsInnerRecycling


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**enabled** | **bool** |  | [optional] 
**interval** | **str** |  | [optional] 
**frequency** | **str** |  | [optional] 
**every** | **int** |  | [optional] 
**max_occurrences** | **int** |  | [optional] 
**ends_at** | **datetime** |  | [optional] 
**expires_at** | **datetime** |  | [optional] 
**until** | **datetime** |  | [optional] 
**end_date** | **datetime** |  | [optional] 
**preserve_queue** | **bool** |  | [optional] 
**allow_duplicate_for_recycling** | **bool** |  | [optional] 

## Example

```python
from kavenio.models.list_posts200_response_any_of_data_posts_inner_recycling import ListPosts200ResponseAnyOfDataPostsInnerRecycling

# TODO update the JSON string below
json = "{}"
# create an instance of ListPosts200ResponseAnyOfDataPostsInnerRecycling from a JSON string
list_posts200_response_any_of_data_posts_inner_recycling_instance = ListPosts200ResponseAnyOfDataPostsInnerRecycling.from_json(json)
# print the JSON string representation of the object
print(ListPosts200ResponseAnyOfDataPostsInnerRecycling.to_json())

# convert the object into a dict
list_posts200_response_any_of_data_posts_inner_recycling_dict = list_posts200_response_any_of_data_posts_inner_recycling_instance.to_dict()
# create an instance of ListPosts200ResponseAnyOfDataPostsInnerRecycling from a dict
list_posts200_response_any_of_data_posts_inner_recycling_from_dict = ListPosts200ResponseAnyOfDataPostsInnerRecycling.from_dict(list_posts200_response_any_of_data_posts_inner_recycling_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


