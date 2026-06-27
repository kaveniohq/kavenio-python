# UpdateQueueSlotSchedule200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ok** | **bool** |  | 
**data** | [**ListQueueSlots200ResponseAnyOfDataQueuesInner**](ListQueueSlots200ResponseAnyOfDataQueuesInner.md) |  | 
**error** | [**ListProfiles401ResponseError**](ListProfiles401ResponseError.md) |  | 

## Example

```python
from kavenio.models.update_queue_slot_schedule200_response import UpdateQueueSlotSchedule200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UpdateQueueSlotSchedule200Response from a JSON string
update_queue_slot_schedule200_response_instance = UpdateQueueSlotSchedule200Response.from_json(json)
# print the JSON string representation of the object
print(UpdateQueueSlotSchedule200Response.to_json())

# convert the object into a dict
update_queue_slot_schedule200_response_dict = update_queue_slot_schedule200_response_instance.to_dict()
# create an instance of UpdateQueueSlotSchedule200Response from a dict
update_queue_slot_schedule200_response_from_dict = UpdateQueueSlotSchedule200Response.from_dict(update_queue_slot_schedule200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


