# UpdateQueueSlotSchedule200ResponseAnyOf


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListQueueSlots200ResponseAnyOfDataQueuesInner**](ListQueueSlots200ResponseAnyOfDataQueuesInner.md) |  | 

## Example

```python
from kavenio.models.update_queue_slot_schedule200_response_any_of import UpdateQueueSlotSchedule200ResponseAnyOf

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateQueueSlotSchedule200ResponseAnyOf from a JSON string
update_queue_slot_schedule200_response_any_of_instance = UpdateQueueSlotSchedule200ResponseAnyOf.from_json(json)
# print the JSON string representation of the object
print(UpdateQueueSlotSchedule200ResponseAnyOf.to_json())

# convert the object into a dict
update_queue_slot_schedule200_response_any_of_dict = update_queue_slot_schedule200_response_any_of_instance.to_dict()
# create an instance of UpdateQueueSlotSchedule200ResponseAnyOf from a dict
update_queue_slot_schedule200_response_any_of_from_dict = UpdateQueueSlotSchedule200ResponseAnyOf.from_dict(update_queue_slot_schedule200_response_any_of_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


