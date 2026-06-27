# ListPosts200ResponseAnyOfDataPagination


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | **int** |  | 
**limit** | **int** |  | 
**total** | **int** |  | 
**has_more** | **bool** |  | 

## Example

```python
from kavenio.models.list_posts200_response_any_of_data_pagination import ListPosts200ResponseAnyOfDataPagination

# TODO update the JSON string below
json = "{}"
# create an instance of ListPosts200ResponseAnyOfDataPagination from a JSON string
list_posts200_response_any_of_data_pagination_instance = ListPosts200ResponseAnyOfDataPagination.from_json(json)
# print the JSON string representation of the object
print(ListPosts200ResponseAnyOfDataPagination.to_json())

# convert the object into a dict
list_posts200_response_any_of_data_pagination_dict = list_posts200_response_any_of_data_pagination_instance.to_dict()
# create an instance of ListPosts200ResponseAnyOfDataPagination from a dict
list_posts200_response_any_of_data_pagination_from_dict = ListPosts200ResponseAnyOfDataPagination.from_dict(list_posts200_response_any_of_data_pagination_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


