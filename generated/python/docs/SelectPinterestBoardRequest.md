# SelectPinterestBoardRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**profile_id** | **str** |  | 
**board_id** | **str** |  | 

## Example

```python
from kavenio.models.select_pinterest_board_request import SelectPinterestBoardRequest

# TODO update the JSON string below
json = "{}"
# create an instance of SelectPinterestBoardRequest from a JSON string
select_pinterest_board_request_instance = SelectPinterestBoardRequest.from_json(json)
# print the JSON string representation of the object
print(SelectPinterestBoardRequest.to_json())

# convert the object into a dict
select_pinterest_board_request_dict = select_pinterest_board_request_instance.to_dict()
# create an instance of SelectPinterestBoardRequest from a dict
select_pinterest_board_request_from_dict = SelectPinterestBoardRequest.from_dict(select_pinterest_board_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


