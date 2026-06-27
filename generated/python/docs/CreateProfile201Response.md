# CreateProfile201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**CreateProfile201ResponseData**](CreateProfile201ResponseData.md) |  | 

## Example

```python
from kavenio.models.create_profile201_response import CreateProfile201Response

# TODO update the JSON string below
json = "{}"
# create an instance of CreateProfile201Response from a JSON string
create_profile201_response_instance = CreateProfile201Response.from_json(json)
# print the JSON string representation of the object
print(CreateProfile201Response.to_json())

# convert the object into a dict
create_profile201_response_dict = create_profile201_response_instance.to_dict()
# create an instance of CreateProfile201Response from a dict
create_profile201_response_from_dict = CreateProfile201Response.from_dict(create_profile201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


