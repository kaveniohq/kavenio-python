# CreatePostRequestMediaItemsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | 
**url** | **str** |  | 
**title** | **str** |  | [optional] 
**alt_text** | **str** |  | [optional] 
**filename** | **str** |  | [optional] 
**size** | **int** |  | [optional] 
**mime_type** | **str** |  | [optional] 
**thumbnail** | **str** |  | [optional] 
**duration_ms** | **int** |  | [optional] 
**duration_seconds** | **float** |  | [optional] 
**width** | **int** |  | [optional] 
**height** | **int** |  | [optional] 
**frame_rate** | **float** |  | [optional] 
**frame_count** | **int** |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_media_items_inner import CreatePostRequestMediaItemsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestMediaItemsInner from a JSON string
create_post_request_media_items_inner_instance = CreatePostRequestMediaItemsInner.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestMediaItemsInner.to_json())

# convert the object into a dict
create_post_request_media_items_inner_dict = create_post_request_media_items_inner_instance.to_dict()
# create an instance of CreatePostRequestMediaItemsInner from a dict
create_post_request_media_items_inner_from_dict = CreatePostRequestMediaItemsInner.from_dict(create_post_request_media_items_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


