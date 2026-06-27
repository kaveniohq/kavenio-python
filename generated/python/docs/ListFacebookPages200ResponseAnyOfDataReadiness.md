# ListFacebookPages200ResponseAnyOfDataReadiness


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**platform** | **str** |  | 
**ready** | **bool** |  | 
**status** | **str** |  | 
**checked_at** | **str** |  | [optional] 
**reconnect_recommended** | **bool** |  | [optional] 
**selected_destination_id** | **str** |  | [optional] 
**selected_destination_name** | **str** |  | [optional] 
**missing_scopes** | **List[str]** |  | [optional] 
**missing_permissions** | **List[str]** |  | [optional] 
**missing_destinations** | **List[str]** |  | [optional] 
**issues** | [**List[ListFacebookPages200ResponseAnyOfDataReadinessIssuesInner]**](ListFacebookPages200ResponseAnyOfDataReadinessIssuesInner.md) |  | [optional] 
**capabilities** | [**List[ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner]**](ListFacebookPages200ResponseAnyOfDataReadinessCapabilitiesInner.md) |  | [optional] 

## Example

```python
from kavenio.models.list_facebook_pages200_response_any_of_data_readiness import ListFacebookPages200ResponseAnyOfDataReadiness

# TODO update the JSON string below
json = "{}"
# create an instance of ListFacebookPages200ResponseAnyOfDataReadiness from a JSON string
list_facebook_pages200_response_any_of_data_readiness_instance = ListFacebookPages200ResponseAnyOfDataReadiness.from_json(json)
# print the JSON string representation of the object
print(ListFacebookPages200ResponseAnyOfDataReadiness.to_json())

# convert the object into a dict
list_facebook_pages200_response_any_of_data_readiness_dict = list_facebook_pages200_response_any_of_data_readiness_instance.to_dict()
# create an instance of ListFacebookPages200ResponseAnyOfDataReadiness from a dict
list_facebook_pages200_response_any_of_data_readiness_from_dict = ListFacebookPages200ResponseAnyOfDataReadiness.from_dict(list_facebook_pages200_response_any_of_data_readiness_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


