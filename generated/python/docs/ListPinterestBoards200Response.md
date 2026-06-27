# ListPinterestBoards200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListPinterestBoards200ResponseAnyOfData**](ListPinterestBoards200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.list_pinterest_boards200_response import ListPinterestBoards200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ListPinterestBoards200Response from a JSON string
list_pinterest_boards200_response_instance = ListPinterestBoards200Response.from_json(json)
# print the JSON string representation of the object
print(ListPinterestBoards200Response.to_json())

# convert the object into a dict
list_pinterest_boards200_response_dict = list_pinterest_boards200_response_instance.to_dict()
# create an instance of ListPinterestBoards200Response from a dict
list_pinterest_boards200_response_from_dict = ListPinterestBoards200Response.from_dict(list_pinterest_boards200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


