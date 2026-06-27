# RefreshTikTokCreatorInfo200ResponseAnyOfData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**account_id** | **str** |  | 
**creator_info** | [**RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo**](RefreshTikTokCreatorInfo200ResponseAnyOfDataCreatorInfo.md) |  | 
**readiness** | [**ListFacebookPages200ResponseAnyOfDataReadiness**](ListFacebookPages200ResponseAnyOfDataReadiness.md) |  | [optional] 

## Example

```python
from kavenio.models.refresh_tik_tok_creator_info200_response_any_of_data import RefreshTikTokCreatorInfo200ResponseAnyOfData

# TODO update the JSON string below
json = "{}"
# create an instance of RefreshTikTokCreatorInfo200ResponseAnyOfData from a JSON string
refresh_tik_tok_creator_info200_response_any_of_data_instance = RefreshTikTokCreatorInfo200ResponseAnyOfData.from_json(json)
# print the JSON string representation of the object
print(RefreshTikTokCreatorInfo200ResponseAnyOfData.to_json())

# convert the object into a dict
refresh_tik_tok_creator_info200_response_any_of_data_dict = refresh_tik_tok_creator_info200_response_any_of_data_instance.to_dict()
# create an instance of RefreshTikTokCreatorInfo200ResponseAnyOfData from a dict
refresh_tik_tok_creator_info200_response_any_of_data_from_dict = RefreshTikTokCreatorInfo200ResponseAnyOfData.from_dict(refresh_tik_tok_creator_info200_response_any_of_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


