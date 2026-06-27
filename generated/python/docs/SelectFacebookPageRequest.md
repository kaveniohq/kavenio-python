# SelectFacebookPageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**profile_id** | **str** |  | [optional] 
**page_id** | **str** |  | 

## Example

```python
from kavenio.models.select_facebook_page_request import SelectFacebookPageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SelectFacebookPageRequest from a JSON string
select_facebook_page_request_instance = SelectFacebookPageRequest.from_json(json)
# print the JSON string representation of the object
print(SelectFacebookPageRequest.to_json())

# convert the object into a dict
select_facebook_page_request_dict = select_facebook_page_request_instance.to_dict()
# create an instance of SelectFacebookPageRequest from a dict
select_facebook_page_request_from_dict = SelectFacebookPageRequest.from_dict(select_facebook_page_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


