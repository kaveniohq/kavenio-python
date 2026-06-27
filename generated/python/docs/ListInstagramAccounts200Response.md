# ListInstagramAccounts200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListInstagramAccounts200ResponseAnyOfData**](ListInstagramAccounts200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.list_instagram_accounts200_response import ListInstagramAccounts200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListInstagramAccounts200Response from a JSON string
list_instagram_accounts200_response_instance = ListInstagramAccounts200Response.from_json(json)
# print the JSON string representation of the object
print(ListInstagramAccounts200Response.to_json())

# convert the object into a dict
list_instagram_accounts200_response_dict = list_instagram_accounts200_response_instance.to_dict()
# create an instance of ListInstagramAccounts200Response from a dict
list_instagram_accounts200_response_from_dict = ListInstagramAccounts200Response.from_dict(list_instagram_accounts200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


