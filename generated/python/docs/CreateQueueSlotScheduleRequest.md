# CreateQueueSlotScheduleRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**profile_id** | **str** |  | 
**name** | **str** |  | 
**timezone** | **str** |  | 
**active** | **bool** |  | [optional] 
**is_default** | **bool** |  | [optional] 
**slots** | [**List[UpdateQueueSlotScheduleRequestSlotsInner]**](UpdateQueueSlotScheduleRequestSlotsInner.md) |  | [optional] [default to []]

## Example

```python
from kavenio.models.create_queue_slot_schedule_request import CreateQueueSlotScheduleRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateQueueSlotScheduleRequest from a JSON string
create_queue_slot_schedule_request_instance = CreateQueueSlotScheduleRequest.from_json(json)
# print the JSON string representation of the object
print(CreateQueueSlotScheduleRequest.to_json())

# convert the object into a dict
create_queue_slot_schedule_request_dict = create_queue_slot_schedule_request_instance.to_dict()
# create an instance of CreateQueueSlotScheduleRequest from a dict
create_queue_slot_schedule_request_from_dict = CreateQueueSlotScheduleRequest.from_dict(create_queue_slot_schedule_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


