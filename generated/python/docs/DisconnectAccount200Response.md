# DisconnectAccount200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**DisconnectAccount200ResponseAnyOfData**](DisconnectAccount200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.disconnect_account200_response import DisconnectAccount200Response

# TODO update the JSON string below
json = "{}"
# create an instance of DisconnectAccount200Response from a JSON string
disconnect_account200_response_instance = DisconnectAccount200Response.from_json(json)
# print the JSON string representation of the object
print(DisconnectAccount200Response.to_json())

# convert the object into a dict
disconnect_account200_response_dict = disconnect_account200_response_instance.to_dict()
# create an instance of DisconnectAccount200Response from a dict
disconnect_account200_response_from_dict = DisconnectAccount200Response.from_dict(disconnect_account200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


