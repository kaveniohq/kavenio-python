# UpdateQueueSlotScheduleRequestSlotsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**day_of_week** | **int** |  | 
**time** | **str** |  | 
**timezone** | **str** |  | 
**active** | **bool** |  | [optional] 

## Example

```python
from kavenio.models.update_queue_slot_schedule_request_slots_inner import UpdateQueueSlotScheduleRequestSlotsInner

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateQueueSlotScheduleRequestSlotsInner from a JSON string
update_queue_slot_schedule_request_slots_inner_instance = UpdateQueueSlotScheduleRequestSlotsInner.from_json(json)
# print the JSON string representation of the object
print(UpdateQueueSlotScheduleRequestSlotsInner.to_json())

# convert the object into a dict
update_queue_slot_schedule_request_slots_inner_dict = update_queue_slot_schedule_request_slots_inner_instance.to_dict()
# create an instance of UpdateQueueSlotScheduleRequestSlotsInner from a dict
update_queue_slot_schedule_request_slots_inner_from_dict = UpdateQueueSlotScheduleRequestSlotsInner.from_dict(update_queue_slot_schedule_request_slots_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


