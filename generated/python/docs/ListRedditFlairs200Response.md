# ListRedditFlairs200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListRedditFlairs200ResponseAnyOfData**](ListRedditFlairs200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.list_reddit_flairs200_response import ListRedditFlairs200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListRedditFlairs200Response from a JSON string
list_reddit_flairs200_response_instance = ListRedditFlairs200Response.from_json(json)
# print the JSON string representation of the object
print(ListRedditFlairs200Response.to_json())

# convert the object into a dict
list_reddit_flairs200_response_dict = list_reddit_flairs200_response_instance.to_dict()
# create an instance of ListRedditFlairs200Response from a dict
list_reddit_flairs200_response_from_dict = ListRedditFlairs200Response.from_dict(list_reddit_flairs200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


