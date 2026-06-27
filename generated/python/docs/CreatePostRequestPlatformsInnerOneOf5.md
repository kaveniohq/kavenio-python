# CreatePostRequestPlatformsInnerOneOf5


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | [optional] 
**custom_content** | **str** |  | [optional] 
**custom_media** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**platform** | **str** |  | 
**platform_specific_data** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf5**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf5.md) |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of5 import CreatePostRequestPlatformsInnerOneOf5

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOf5 from a JSON string
create_post_request_platforms_inner_one_of5_instance = CreatePostRequestPlatformsInnerOneOf5.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOf5.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of5_dict = create_post_request_platforms_inner_one_of5_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOf5 from a dict
create_post_request_platforms_inner_one_of5_from_dict = CreatePostRequestPlatformsInnerOneOf5.from_dict(create_post_request_platforms_inner_one_of5_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


