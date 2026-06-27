# CreatePostRequestPlatformsInnerOneOf10


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | [optional] 
**custom_content** | **str** |  | [optional] 
**custom_media** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**platform** | **str** |  | 
**platform_specific_data** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf10**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf10.md) |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of10 import CreatePostRequestPlatformsInnerOneOf10

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOf10 from a JSON string
create_post_request_platforms_inner_one_of10_instance = CreatePostRequestPlatformsInnerOneOf10.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOf10.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of10_dict = create_post_request_platforms_inner_one_of10_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOf10 from a dict
create_post_request_platforms_inner_one_of10_from_dict = CreatePostRequestPlatformsInnerOneOf10.from_dict(create_post_request_platforms_inner_one_of10_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


