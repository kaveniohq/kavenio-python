# ListFacebookPages200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListFacebookPages200ResponseAnyOfData**](ListFacebookPages200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.list_facebook_pages200_response import ListFacebookPages200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListFacebookPages200Response from a JSON string
list_facebook_pages200_response_instance = ListFacebookPages200Response.from_json(json)
# print the JSON string representation of the object
print(ListFacebookPages200Response.to_json())

# convert the object into a dict
list_facebook_pages200_response_dict = list_facebook_pages200_response_instance.to_dict()
# create an instance of ListFacebookPages200Response from a dict
list_facebook_pages200_response_from_dict = ListFacebookPages200Response.from_dict(list_facebook_pages200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


