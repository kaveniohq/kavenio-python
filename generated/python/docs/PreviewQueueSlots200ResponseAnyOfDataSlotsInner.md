# PreviewQueueSlots200ResponseAnyOfDataSlotsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**queue_id** | **str** |  | 
**profile_id** | **str** |  | 
**day_of_week** | **int** |  | 
**time** | **str** |  | 
**timezone** | **str** |  | 
**scheduled_for** | **datetime** |  | 

## Example

```python
from kavenio.models.preview_queue_slots200_response_any_of_data_slots_inner import PreviewQueueSlots200ResponseAnyOfDataSlotsInner

# TODO update the JSON string below
json = "{}"
# create an instance of PreviewQueueSlots200ResponseAnyOfDataSlotsInner from a JSON string
preview_queue_slots200_response_any_of_data_slots_inner_instance = PreviewQueueSlots200ResponseAnyOfDataSlotsInner.from_json(json)
# print the JSON string representation of the object
print(PreviewQueueSlots200ResponseAnyOfDataSlotsInner.to_json())

# convert the object into a dict
preview_queue_slots200_response_any_of_data_slots_inner_dict = preview_queue_slots200_response_any_of_data_slots_inner_instance.to_dict()
# create an instance of PreviewQueueSlots200ResponseAnyOfDataSlotsInner from a dict
preview_queue_slots200_response_any_of_data_slots_inner_from_dict = PreviewQueueSlots200ResponseAnyOfDataSlotsInner.from_dict(preview_queue_slots200_response_any_of_data_slots_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


