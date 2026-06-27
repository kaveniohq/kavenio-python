# CreatePostRequestRecycling


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
from kavenio.models.create_post_request_recycling import CreatePostRequestRecycling

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestRecycling from a JSON string
create_post_request_recycling_instance = CreatePostRequestRecycling.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestRecycling.to_json())

# convert the object into a dict
create_post_request_recycling_dict = create_post_request_recycling_instance.to_dict()
# create an instance of CreatePostRequestRecycling from a dict
create_post_request_recycling_from_dict = CreatePostRequestRecycling.from_dict(create_post_request_recycling_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


