# CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**thread_items** | [**List[CreatePostRequestPlatformsInnerOneOfPlatformSpecificDataThreadItemsInner]**](CreatePostRequestPlatformsInnerOneOfPlatformSpecificDataThreadItemsInner.md) |  | [optional] 
**external_url** | **str** |  | [optional] 
**external_title** | **str** |  | [optional] 
**external_description** | **str** |  | [optional] 
**external_thumb_url** | **str** |  | [optional] 
**disable_link_preview** | **bool** |  | [optional] 

## Example

```python
from kavenio.models.create_post_request_platforms_inner_one_of3_platform_specific_data import CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData

# TODO update the JSON string below
json = "{}"
# create an instance of CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData from a JSON string
create_post_request_platforms_inner_one_of3_platform_specific_data_instance = CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData.from_json(json)
# print the JSON string representation of the object
print(CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData.to_json())

# convert the object into a dict
create_post_request_platforms_inner_one_of3_platform_specific_data_dict = create_post_request_platforms_inner_one_of3_platform_specific_data_instance.to_dict()
# create an instance of CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData from a dict
create_post_request_platforms_inner_one_of3_platform_specific_data_from_dict = CreatePostRequestPlatformsInnerOneOf3PlatformSpecificData.from_dict(create_post_request_platforms_inner_one_of3_platform_specific_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


