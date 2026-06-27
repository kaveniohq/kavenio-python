# RefreshTikTokCreatorInfo200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**RefreshTikTokCreatorInfo200ResponseAnyOfData**](RefreshTikTokCreatorInfo200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.refresh_tik_tok_creator_info200_response import RefreshTikTokCreatorInfo200Response

# TODO update the JSON string below
json = "{}"
# create an instance of RefreshTikTokCreatorInfo200Response from a JSON string
refresh_tik_tok_creator_info200_response_instance = RefreshTikTokCreatorInfo200Response.from_json(json)
# print the JSON string representation of the object
print(RefreshTikTokCreatorInfo200Response.to_json())

# convert the object into a dict
refresh_tik_tok_creator_info200_response_dict = refresh_tik_tok_creator_info200_response_instance.to_dict()
# create an instance of RefreshTikTokCreatorInfo200Response from a dict
refresh_tik_tok_creator_info200_response_from_dict = RefreshTikTokCreatorInfo200Response.from_dict(refresh_tik_tok_creator_info200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


