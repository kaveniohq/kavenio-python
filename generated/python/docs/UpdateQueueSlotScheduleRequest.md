# UpdateQueueSlotScheduleRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | 
**queue_id** | **str** |  | 
**name** | **str** |  | [optional] 
**timezone** | **str** |  | [optional] 
**active** | **bool** |  | [optional] 
**is_default** | **bool** |  | [optional] 
**slots** | [**List[UpdateQueueSlotScheduleRequestSlotsInner]**](UpdateQueueSlotScheduleRequestSlotsInner.md) |  | [optional] 

## Example

```python
from kavenio.models.update_queue_slot_schedule_request import UpdateQueueSlotScheduleRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateQueueSlotScheduleRequest from a JSON string
update_queue_slot_schedule_request_instance = UpdateQueueSlotScheduleRequest.from_json(json)
# print the JSON string representation of the object
print(UpdateQueueSlotScheduleRequest.to_json())

# convert the object into a dict
update_queue_slot_schedule_request_dict = update_queue_slot_schedule_request_instance.to_dict()
# create an instance of UpdateQueueSlotScheduleRequest from a dict
update_queue_slot_schedule_request_from_dict = UpdateQueueSlotScheduleRequest.from_dict(update_queue_slot_schedule_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


