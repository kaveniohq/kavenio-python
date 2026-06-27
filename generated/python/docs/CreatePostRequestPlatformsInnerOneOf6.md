# CreatePostRequestPlatformsInnerOneOf6


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | [optional] 
**custom_content** | **str** |  | [optional] 
**custom_media** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**platform** | **str** |  | 
**platform_specific_data** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf6**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf6.md) |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of6 import CreatePostRequestPlatformsInnerOneOf6

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOf6 from a JSON string
create_post_request_platforms_inner_one_of6_instance = CreatePostRequestPlatformsInnerOneOf6.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOf6.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of6_dict = create_post_request_platforms_inner_one_of6_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOf6 from a dict
create_post_request_platforms_inner_one_of6_from_dict = CreatePostRequestPlatformsInnerOneOf6.from_dict(create_post_request_platforms_inner_one_of6_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


