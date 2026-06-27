# CompleteConnect200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**CompleteConnect200ResponseAnyOfData**](CompleteConnect200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.complete_connect200_response import CompleteConnect200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CompleteConnect200Response from a JSON string
complete_connect200_response_instance = CompleteConnect200Response.from_json(json)
# print the JSON string representation of the object
print(CompleteConnect200Response.to_json())

# convert the object into a dict
complete_connect200_response_dict = complete_connect200_response_instance.to_dict()
# create an instance of CompleteConnect200Response from a dict
complete_connect200_response_from_dict = CompleteConnect200Response.from_dict(complete_connect200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


