# SelectInstagramAccountRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**profile_id** | **str** |  | [optional] 
**instagram_account_id** | **str** |  | 
**connected_facebook_page_id** | **str** |  | [optional] 

## Example

```python
from kavenio.models.select_instagram_account_request import SelectInstagramAccountRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SelectInstagramAccountRequest from a JSON string
select_instagram_account_request_instance = SelectInstagramAccountRequest.from_json(json)
# print the JSON string representation of the object
print(SelectInstagramAccountRequest.to_json())

# convert the object into a dict
select_instagram_account_request_dict = select_instagram_account_request_instance.to_dict()
# create an instance of SelectInstagramAccountRequest from a dict
select_instagram_account_request_from_dict = SelectInstagramAccountRequest.from_dict(select_instagram_account_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


