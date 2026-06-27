# ValidatePost200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**valid** | **bool** |  | 
**message** | **str** |  | [optional] 
**errors** | [**List[ValidatePost200ResponseAnyOfDataErrorsInner]**](ValidatePost200ResponseAnyOfDataErrorsInner.md) |  | [optional] 
**warnings** | [**List[ValidatePost200ResponseAnyOfDataWarningsInner]**](ValidatePost200ResponseAnyOfDataWarningsInner.md) |  | [optional] 

## Example

```python
from kavenio.models.validate_post200_response_any_of_data import ValidatePost200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of ValidatePost200ResponseAnyOfData from a JSON string
validate_post200_response_any_of_data_instance = ValidatePost200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(ValidatePost200ResponseAnyOfData.to_json())

# convert the object into a dict
validate_post200_response_any_of_data_dict = validate_post200_response_any_of_data_instance.to_dict()
# create an instance of ValidatePost200ResponseAnyOfData from a dict
validate_post200_response_any_of_data_from_dict = ValidatePost200ResponseAnyOfData.from_dict(validate_post200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


