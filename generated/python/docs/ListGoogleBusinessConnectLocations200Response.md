# ListGoogleBusinessConnectLocations200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListGoogleBusinessConnectLocations200ResponseAnyOfData**](ListGoogleBusinessConnectLocations200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.list_google_business_connect_locations200_response import ListGoogleBusinessConnectLocations200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListGoogleBusinessConnectLocations200Response from a JSON string
list_google_business_connect_locations200_response_instance = ListGoogleBusinessConnectLocations200Response.from_json(json)
# print the JSON string representation of the object
print(ListGoogleBusinessConnectLocations200Response.to_json())

# convert the object into a dict
list_google_business_connect_locations200_response_dict = list_google_business_connect_locations200_response_instance.to_dict()
# create an instance of ListGoogleBusinessConnectLocations200Response from a dict
list_google_business_connect_locations200_response_from_dict = ListGoogleBusinessConnectLocations200Response.from_dict(list_google_business_connect_locations200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


