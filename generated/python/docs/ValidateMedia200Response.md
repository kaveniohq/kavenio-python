# ValidateMedia200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ValidateMedia200ResponseData**](ValidateMedia200ResponseData.md) |  | 

## Example

```python
from kavenio.models.validate_media200_response import ValidateMedia200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ValidateMedia200Response from a JSON string
validate_media200_response_instance = ValidateMedia200Response.from_json(json)
# print the JSON string representation of the object
print(ValidateMedia200Response.to_json())

# convert the object into a dict
validate_media200_response_dict = validate_media200_response_instance.to_dict()
# create an instance of ValidateMedia200Response from a dict
validate_media200_response_from_dict = ValidateMedia200Response.from_dict(validate_media200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


