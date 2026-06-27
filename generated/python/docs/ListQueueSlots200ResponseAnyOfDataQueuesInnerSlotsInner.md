# ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**queue_id** | **str** |  | [optional] 
**day_of_week** | **int** |  | 
**time** | **str** |  | 
**timezone** | **str** |  | 
**active** | **bool** |  | [optional] 

## Example

```python
from kavenio.models.list_queue_slots200_response_any_of_data_queues_inner_slots_inner import ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner from a JSON string
list_queue_slots200_response_any_of_data_queues_inner_slots_inner_instance = ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner.from_json(json)
# print the JSON string representation of the object
print(ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner.to_json())

# convert the object into a dict
list_queue_slots200_response_any_of_data_queues_inner_slots_inner_dict = list_queue_slots200_response_any_of_data_queues_inner_slots_inner_instance.to_dict()
# create an instance of ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner from a dict
list_queue_slots200_response_any_of_data_queues_inner_slots_inner_from_dict = ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner.from_dict(list_queue_slots200_response_any_of_data_queues_inner_slots_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


