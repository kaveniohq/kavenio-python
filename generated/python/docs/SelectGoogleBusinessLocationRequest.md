# SelectGoogleBusinessLocationRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**profile_id** | **str** |  | [optional] 
**location_id** | **str** |  | 

## Example

```python
from kavenio.models.select_google_business_location_request import SelectGoogleBusinessLocationRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SelectGoogleBusinessLocationRequest from a JSON string
select_google_business_location_request_instance = SelectGoogleBusinessLocationRequest.from_json(json)
# print the JSON string representation of the object
print(SelectGoogleBusinessLocationRequest.to_json())

# convert the object into a dict
select_google_business_location_request_dict = select_google_business_location_request_instance.to_dict()
# create an instance of SelectGoogleBusinessLocationRequest from a dict
select_google_business_location_request_from_dict = SelectGoogleBusinessLocationRequest.from_dict(select_google_business_location_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


