# ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**account_id** | **str** |  | [optional] 
**account_name** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**resource_name** | **str** |  | [optional] 
**title** | **str** |  | [optional] 
**address** | **str** |  | [optional] 
**category** | **str** |  | [optional] 
**store_code** | **str** |  | [optional] 
**place_id** | **str** |  | [optional] 
**maps_uri** | **str** |  | [optional] 
**review_url** | **str** |  | [optional] 
**website_uri** | **str** |  | [optional] 
**phone_number** | **str** |  | [optional] 
**is_verified** | **bool** |  | [optional] 
**selected** | **bool** |  | [optional] 
**can_publish** | **bool** |  | [optional] 
**missing_permissions** | **List[str]** |  | [optional] 

## Example

```python
from kavenio.models.list_google_business_connect_locations200_response_any_of_data_locations_inner import ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner from a JSON string
list_google_business_connect_locations200_response_any_of_data_locations_inner_instance = ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner.from_json(json)
# print the JSON string representation of the object
print(ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner.to_json())

# convert the object into a dict
list_google_business_connect_locations200_response_any_of_data_locations_inner_dict = list_google_business_connect_locations200_response_any_of_data_locations_inner_instance.to_dict()
# create an instance of ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner from a dict
list_google_business_connect_locations200_response_any_of_data_locations_inner_from_dict = ListGoogleBusinessConnectLocations200ResponseAnyOfDataLocationsInner.from_dict(list_google_business_connect_locations200_response_any_of_data_locations_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


