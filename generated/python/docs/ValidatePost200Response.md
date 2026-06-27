# ValidatePost200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ValidatePost200ResponseAnyOfData**](ValidatePost200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.validate_post200_response import ValidatePost200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ValidatePost200Response from a JSON string
validate_post200_response_instance = ValidatePost200Response.from_json(json)
# print the JSON string representation of the object
print(ValidatePost200Response.to_json())

# convert the object into a dict
validate_post200_response_dict = validate_post200_response_instance.to_dict()
# create an instance of ValidatePost200Response from a dict
validate_post200_response_from_dict = ValidatePost200Response.from_dict(validate_post200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


