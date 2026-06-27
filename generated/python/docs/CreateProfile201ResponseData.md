# CreateProfile201ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**organization_id** | **str** |  | 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**color** | **str** |  | [optional] 
**is_default** | **bool** |  | 
**created_by** | **str** |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from kavenio.models.create_profile201_response_data import CreateProfile201ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of CreateProfile201ResponseData from a JSON string
create_profile201_response_data_instance = CreateProfile201ResponseData.from_json(json)
# print the JSON string representation of the object
print(CreateProfile201ResponseData.to_json())

# convert the object into a dict
create_profile201_response_data_dict = create_profile201_response_data_instance.to_dict()
# create an instance of CreateProfile201ResponseData from a dict
create_profile201_response_data_from_dict = CreateProfile201ResponseData.from_dict(create_profile201_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


