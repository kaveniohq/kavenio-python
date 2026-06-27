# CreatePostRequestPlatformsInnerOneOf3


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | [optional] 
**custom_content** | **str** |  | [optional] 
**custom_media** | [**List[CreatePostRequestMediaItemsInner]**](CreatePostRequestMediaItemsInner.md) |  | [optional] 
**scheduled_for** | **datetime** |  | [optional] 
**platform** | **str** |  | 
**platform_specific_data** | [**CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData**](CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData.md) |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of3 import CreatePostRequestPlatformsInnerOneOf3

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOf3 from a JSON string
create_post_request_platforms_inner_one_of3_instance = CreatePostRequestPlatformsInnerOneOf3.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOf3.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of3_dict = create_post_request_platforms_inner_one_of3_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOf3 from a dict
create_post_request_platforms_inner_one_of3_from_dict = CreatePostRequestPlatformsInnerOneOf3.from_dict(create_post_request_platforms_inner_one_of3_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


