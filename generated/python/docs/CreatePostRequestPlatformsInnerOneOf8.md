# CreatePostRequestPlatformsInnerOneOf8


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | [optional] 
**custom_content** | **str** |  | [optional] 
**custom_media** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**platform** | **str** |  | 
**platform_specific_data** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf8**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf8.md) |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of8 import CreatePostRequestPlatformsInnerOneOf8

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOf8 from a JSON string
create_post_request_platforms_inner_one_of8_instance = CreatePostRequestPlatformsInnerOneOf8.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOf8.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of8_dict = create_post_request_platforms_inner_one_of8_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOf8 from a dict
create_post_request_platforms_inner_one_of8_from_dict = CreatePostRequestPlatformsInnerOneOf8.from_dict(create_post_request_platforms_inner_one_of8_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


