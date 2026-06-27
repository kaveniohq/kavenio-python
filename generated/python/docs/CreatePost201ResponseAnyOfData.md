# CreatePost201ResponseAnyOfData


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
**recycling** | [**CreatePostRequestRecycling**](CreatePostRequestRecycling.md) |  | [optional] 
**targets** | [**List[ListPosts200ResponseAnyOfDataPostsInnerTargetsInner]**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInner.md) |  | 
**created_at** | **datetime** |  | 
**updated_at** | **datetime** |  | 

## Example

```python
from kavenio.models.create_post201_response_any_of_data import CreatePost201ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePost201ResponseAnyOfData from a JSON string
create_post201_response_any_of_data_instance = CreatePost201ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(CreatePost201ResponseAnyOfData.to_json())

# convert the object into a dict
create_post201_response_any_of_data_dict = create_post201_response_any_of_data_instance.to_dict()
# create an instance of CreatePost201ResponseAnyOfData from a dict
create_post201_response_any_of_data_from_dict = CreatePost201ResponseAnyOfData.from_dict(create_post201_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


