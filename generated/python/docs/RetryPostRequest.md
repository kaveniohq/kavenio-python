# RetryPostRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**target_ids** | **List[Optional[str]]** |  | [optional] 

## Example

```python
from kavenio.models.retry_post_request import RetryPostRequest

# TODO update the JSON string below
json = "{}"
# create an instance of RetryPostRequest from a JSON string
retry_post_request_instance = RetryPostRequest.from_json(json)
# print the JSON string representation of the object
print(RetryPostRequest.to_json())

# convert the object into a dict
retry_post_request_dict = retry_post_request_instance.to_dict()
# create an instance of RetryPostRequest from a dict
retry_post_request_from_dict = RetryPostRequest.from_dict(retry_post_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


