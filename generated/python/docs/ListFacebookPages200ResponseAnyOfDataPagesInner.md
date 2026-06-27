# ListFacebookPages200ResponseAnyOfDataPagesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**name** | **str** |  | 
**username** | **str** |  | [optional] 
**category** | **str** |  | [optional] 
**tasks** | **List[str]** |  | [optional] 
**page_url** | **str** |  | [optional] 
**picture_url** | **str** |  | [optional] 
**connected_instagram_account_id** | **str** |  | [optional] 
**connected_instagram_username** | **str** |  | [optional] 
**connected_instagram_name** | **str** |  | [optional] 
**connected_instagram_account_type** | **str** |  | [optional] 
**connected_instagram_profile_picture_url** | **str** |  | [optional] 
**selected** | **bool** |  | [optional] 
**can_publish** | **bool** |  | [optional] 
**missing_permissions** | **List[str]** |  | [optional] 

## Example

```python
from kavenio.models.list_facebook_pages200_response_any_of_data_pages_inner import ListFacebookPages200ResponseAnyOfDataPagesInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListFacebookPages200ResponseAnyOfDataPagesInner from a JSON string
list_facebook_pages200_response_any_of_data_pages_inner_instance = ListFacebookPages200ResponseAnyOfDataPagesInner.from_json(json)
# print the JSON string representation of the object
print(ListFacebookPages200ResponseAnyOfDataPagesInner.to_json())

# convert the object into a dict
list_facebook_pages200_response_any_of_data_pages_inner_dict = list_facebook_pages200_response_any_of_data_pages_inner_instance.to_dict()
# create an instance of ListFacebookPages200ResponseAnyOfDataPagesInner from a dict
list_facebook_pages200_response_any_of_data_pages_inner_from_dict = ListFacebookPages200ResponseAnyOfDataPagesInner.from_dict(list_facebook_pages200_response_any_of_data_pages_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


