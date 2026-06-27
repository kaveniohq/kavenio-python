# EditPublishedPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**target_ids** | **List[str]** |  | [optional] 
**title** | **str** |  | [optional] 
**content** | **str** |  | [optional] 
**tags** | **List[str]** |  | [optional] 
**category** | **str** |  | [optional] 
**made_for_kids** | **bool** |  | [optional] 
**contains_synthetic_media** | **bool** |  | [optional] 
**visibility** | **str** |  | [optional] 

## Example

```python
from kavenio.models.edit_published_post_request import EditPublishedPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EditPublishedPostRequest from a JSON string
edit_published_post_request_instance = EditPublishedPostRequest.from_json(json)
# print the JSON string representation of the object
print(EditPublishedPostRequest.to_json())

# convert the object into a dict
edit_published_post_request_dict = edit_published_post_request_instance.to_dict()
# create an instance of EditPublishedPostRequest from a dict
edit_published_post_request_from_dict = EditPublishedPostRequest.from_dict(edit_published_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


