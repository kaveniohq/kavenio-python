# ValidateMedia200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**valid** | **bool** |  | 
**url** | **str** |  | 
**error** | **str** |  | [optional] 
**content_type** | **str** |  | [optional] 
**size** | **int** |  | [optional] 
**size_formatted** | **str** |  | [optional] 
**type** | **str** |  | 
**platform_limits** | [**Dict[str, ValidateMedia200ResponseDataPlatformLimitsValue]**](ValidateMedia200ResponseDataPlatformLimitsValue.md) |  | [optional] 

## Example

```python
from kavenio.models.validate_media200_response_data import ValidateMedia200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ValidateMedia200ResponseData from a JSON string
validate_media200_response_data_instance = ValidateMedia200ResponseData.from_json(json)
# print the JSON string representation of the object
print(ValidateMedia200ResponseData.to_json())

# convert the object into a dict
validate_media200_response_data_dict = validate_media200_response_data_instance.to_dict()
# create an instance of ValidateMedia200ResponseData from a dict
validate_media200_response_data_from_dict = ValidateMedia200ResponseData.from_dict(validate_media200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


