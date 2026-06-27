# ListRedditSubreddits200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListRedditSubreddits200ResponseAnyOfData**](ListRedditSubreddits200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.list_reddit_subreddits200_response import ListRedditSubreddits200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListRedditSubreddits200Response from a JSON string
list_reddit_subreddits200_response_instance = ListRedditSubreddits200Response.from_json(json)
# print the JSON string representation of the object
print(ListRedditSubreddits200Response.to_json())

# convert the object into a dict
list_reddit_subreddits200_response_dict = list_reddit_subreddits200_response_instance.to_dict()
# create an instance of ListRedditSubreddits200Response from a dict
list_reddit_subreddits200_response_from_dict = ListRedditSubreddits200Response.from_dict(list_reddit_subreddits200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


