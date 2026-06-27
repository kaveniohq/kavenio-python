# ListRedditSubreddits200ResponseAnyOfDataSubredditsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**display_name** | **str** |  | 
**title** | **str** |  | [optional] 
**over18** | **bool** |  | [optional] 
**user_is_banned** | **bool** |  | [optional] 
**user_is_muted** | **bool** |  | [optional] 

## Example

```python
from kavenio.models.list_reddit_subreddits200_response_any_of_data_subreddits_inner import ListRedditSubreddits200ResponseAnyOfDataSubredditsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListRedditSubreddits200ResponseAnyOfDataSubredditsInner from a JSON string
list_reddit_subreddits200_response_any_of_data_subreddits_inner_instance = ListRedditSubreddits200ResponseAnyOfDataSubredditsInner.from_json(json)
# print the JSON string representation of the object
print(ListRedditSubreddits200ResponseAnyOfDataSubredditsInner.to_json())

# convert the object into a dict
list_reddit_subreddits200_response_any_of_data_subreddits_inner_dict = list_reddit_subreddits200_response_any_of_data_subreddits_inner_instance.to_dict()
# create an instance of ListRedditSubreddits200ResponseAnyOfDataSubredditsInner from a dict
list_reddit_subreddits200_response_any_of_data_subreddits_inner_from_dict = ListRedditSubreddits200ResponseAnyOfDataSubredditsInner.from_dict(list_reddit_subreddits200_response_any_of_data_subreddits_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


