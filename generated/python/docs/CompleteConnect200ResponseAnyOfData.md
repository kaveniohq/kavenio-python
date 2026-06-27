# CompleteConnect200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**platform** | **str** |  | 
**provider_account_id** | **str** |  | 
**display_name** | **str** |  | [optional] 
**attached_to_profile_id** | **str** |  | 
**return_to** | **str** |  | [optional] 

## Example

```python
from kavenio.models.complete_connect200_response_any_of_data import CompleteConnect200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of CompleteConnect200ResponseAnyOfData from a JSON string
complete_connect200_response_any_of_data_instance = CompleteConnect200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(CompleteConnect200ResponseAnyOfData.to_json())

# convert the object into a dict
complete_connect200_response_any_of_data_dict = complete_connect200_response_any_of_data_instance.to_dict()
# create an instance of CompleteConnect200ResponseAnyOfData from a dict
complete_connect200_response_any_of_data_from_dict = CompleteConnect200ResponseAnyOfData.from_dict(complete_connect200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


