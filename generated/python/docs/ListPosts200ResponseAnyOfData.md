# ListPosts200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**posts** | [**List[ListPosts200ResponseAnyOfDataPostsInner]**](ListPosts200ResponseAnyOfDataPostsInner.md) |  | 
**pagination** | [**ListPosts200ResponseAnyOfDataPagination**](ListPosts200ResponseAnyOfDataPagination.md) |  | 

## Example

```python
from kavenio.models.list_posts200_response_any_of_data import ListPosts200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of ListPosts200ResponseAnyOfData from a JSON string
list_posts200_response_any_of_data_instance = ListPosts200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(ListPosts200ResponseAnyOfData.to_json())

# convert the object into a dict
list_posts200_response_any_of_data_dict = list_posts200_response_any_of_data_instance.to_dict()
# create an instance of ListPosts200ResponseAnyOfData from a dict
list_posts200_response_any_of_data_from_dict = ListPosts200ResponseAnyOfData.from_dict(list_posts200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


