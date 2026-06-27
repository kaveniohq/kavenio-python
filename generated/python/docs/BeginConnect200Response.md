# BeginConnect200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**BeginConnect200ResponseAnyOfData**](BeginConnect200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.begin_connect200_response import BeginConnect200Response

# TODO update the JSON string below
json = "{}"
# create an instance of BeginConnect200Response from a JSON string
begin_connect200_response_instance = BeginConnect200Response.from_json(json)
# print the JSON string representation of the object
print(BeginConnect200Response.to_json())

# convert the object into a dict
begin_connect200_response_dict = begin_connect200_response_instance.to_dict()
# create an instance of BeginConnect200Response from a dict
begin_connect200_response_from_dict = BeginConnect200Response.from_dict(begin_connect200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


