# PreviewQueueSlots200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**PreviewQueueSlots200ResponseAnyOfData**](PreviewQueueSlots200ResponseAnyOfData.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.preview_queue_slots200_response import PreviewQueueSlots200Response

# TODO update the JSON string below
json = "{}"
# create an instance of PreviewQueueSlots200Response from a JSON string
preview_queue_slots200_response_instance = PreviewQueueSlots200Response.from_json(json)
# print the JSON string representation of the object
print(PreviewQueueSlots200Response.to_json())

# convert the object into a dict
preview_queue_slots200_response_dict = preview_queue_slots200_response_instance.to_dict()
# create an instance of PreviewQueueSlots200Response from a dict
preview_queue_slots200_response_from_dict = PreviewQueueSlots200Response.from_dict(preview_queue_slots200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


