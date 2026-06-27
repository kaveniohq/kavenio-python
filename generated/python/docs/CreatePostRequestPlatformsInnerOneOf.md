# CreatePostRequestPlatformsInnerOneOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | [optional] 
**custom_content** | **str** |  | [optional] 
**custom_media** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**platform** | **str** |  | 
**platform_specific_data** | [**CreatePostRequestPlatformsInnerOneOfPlatformSpecificData**](CreatePostRequestPlatformsInnerOneOfPlatformSpecificData.md) |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of import CreatePostRequestPlatformsInnerOneOf

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOf from a JSON string
create_post_request_platforms_inner_one_of_instance = CreatePostRequestPlatformsInnerOneOf.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOf.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of_dict = create_post_request_platforms_inner_one_of_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOf from a dict
create_post_request_platforms_inner_one_of_from_dict = CreatePostRequestPlatformsInnerOneOf.from_dict(create_post_request_platforms_inner_one_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


