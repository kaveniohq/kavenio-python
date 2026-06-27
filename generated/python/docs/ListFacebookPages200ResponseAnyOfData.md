# ListFacebookPages200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**pages** | [**List[ListFacebookPages200ResponseAnyOfDataPagesInner]**](ListFacebookPages200ResponseAnyOfDataPagesInner.md) |  | 
**selected_page_id** | **str** |  | [optional] 
**fetched_at** | **str** |  | [optional] 
**readiness** | [**ListFacebookPages200ResponseAnyOfDataReadiness**](ListFacebookPages200ResponseAnyOfDataReadiness.md) |  | [optional] 

## Example

```python
from kavenio.models.list_facebook_pages200_response_any_of_data import ListFacebookPages200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of ListFacebookPages200ResponseAnyOfData from a JSON string
list_facebook_pages200_response_any_of_data_instance = ListFacebookPages200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(ListFacebookPages200ResponseAnyOfData.to_json())

# convert the object into a dict
list_facebook_pages200_response_any_of_data_dict = list_facebook_pages200_response_any_of_data_instance.to_dict()
# create an instance of ListFacebookPages200ResponseAnyOfData from a dict
list_facebook_pages200_response_any_of_data_from_dict = ListFacebookPages200ResponseAnyOfData.from_dict(list_facebook_pages200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


