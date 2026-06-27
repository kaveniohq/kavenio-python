# CreatePostRequestPlatformsInnerOneOf1


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | [optional] 
**custom_content** | **str** |  | [optional] 
**custom_media** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**platform** | **str** |  | 
**platform_specific_data** | [**ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf1**](ListPosts200ResponseAnyOfDataPostsInnerTargetsInnerPlatformSpecificDataAnyOf1.md) |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of1 import CreatePostRequestPlatformsInnerOneOf1

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOf1 from a JSON string
create_post_request_platforms_inner_one_of1_instance = CreatePostRequestPlatformsInnerOneOf1.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOf1.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of1_dict = create_post_request_platforms_inner_one_of1_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOf1 from a dict
create_post_request_platforms_inner_one_of1_from_dict = CreatePostRequestPlatformsInnerOneOf1.from_dict(create_post_request_platforms_inner_one_of1_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


