# ListGoogleBusinessConnectLocations200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**locations** | [**List[ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner]**](ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner.md) |  | 
**selected_location_id** | **str** |  | [optional] 
**next_page_token** | **str** |  | [optional] 
**has_more** | **bool** |  | [optional] 
**fetched_at** | **str** |  | [optional] 

## Example

```python
from kavenio.models.list_google_business_connect_locations200_response_any_of_data import ListGoogleBusinessConnectLocations200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of ListGoogleBusinessConnectLocations200ResponseAnyOfData from a JSON string
list_google_business_connect_locations200_response_any_of_data_instance = ListGoogleBusinessConnectLocations200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(ListGoogleBusinessConnectLocations200ResponseAnyOfData.to_json())

# convert the object into a dict
list_google_business_connect_locations200_response_any_of_data_dict = list_google_business_connect_locations200_response_any_of_data_instance.to_dict()
# create an instance of ListGoogleBusinessConnectLocations200ResponseAnyOfData from a dict
list_google_business_connect_locations200_response_any_of_data_from_dict = ListGoogleBusinessConnectLocations200ResponseAnyOfData.from_dict(list_google_business_connect_locations200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


