# UnpublishPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**target_ids** | **List[str]** |  | [optional] 

## Example

```python
from kavenio.models.unpublish_post_request import UnpublishPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UnpublishPostRequest from a JSON string
unpublish_post_request_instance = UnpublishPostRequest.from_json(json)
# print the JSON string representation of the object
print(UnpublishPostRequest.to_json())

# convert the object into a dict
unpublish_post_request_dict = unpublish_post_request_instance.to_dict()
# create an instance of UnpublishPostRequest from a dict
unpublish_post_request_from_dict = UnpublishPostRequest.from_dict(unpublish_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


