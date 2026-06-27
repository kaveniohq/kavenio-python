# ValidatePostLength200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ValidatePostLength200ResponseAnyOfData**](ValidatePostLength200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.validate_post_length200_response import ValidatePostLength200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ValidatePostLength200Response from a JSON string
validate_post_length200_response_instance = ValidatePostLength200Response.from_json(json)
# print the JSON string representation of the object
print(ValidatePostLength200Response.to_json())

# convert the object into a dict
validate_post_length200_response_dict = validate_post_length200_response_instance.to_dict()
# create an instance of ValidatePostLength200Response from a dict
validate_post_length200_response_from_dict = ValidatePostLength200Response.from_dict(validate_post_length200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


