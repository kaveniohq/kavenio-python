# ListQueueSlots200ResponseAnyOfDataQueuesInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**profile_id** | **str** |  | 
**name** | **str** |  | 
**timezone** | **str** |  | 
**active** | **bool** |  | 
**is_default** | **bool** |  | 
**slots** | [**List[ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner]**](ListQueueSlots200ResponseAnyOfDataQueuesInnerSlotsInner.md) |  | 
**created_at** | **str** |  | 
**updated_at** | **str** |  | 

## Example

```python
from kavenio.models.list_queue_slots200_response_any_of_data_queues_inner import ListQueueSlots200ResponseAnyOfDataQueuesInner

# TODO update the JSON string below
json = "{}"
# create an instance of ListQueueSlots200ResponseAnyOfDataQueuesInner from a JSON string
list_queue_slots200_response_any_of_data_queues_inner_instance = ListQueueSlots200ResponseAnyOfDataQueuesInner.from_json(json)
# print the JSON string representation of the object
print(ListQueueSlots200ResponseAnyOfDataQueuesInner.to_json())

# convert the object into a dict
list_queue_slots200_response_any_of_data_queues_inner_dict = list_queue_slots200_response_any_of_data_queues_inner_instance.to_dict()
# create an instance of ListQueueSlots200ResponseAnyOfDataQueuesInner from a dict
list_queue_slots200_response_any_of_data_queues_inner_from_dict = ListQueueSlots200ResponseAnyOfDataQueuesInner.from_dict(list_queue_slots200_response_any_of_data_queues_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


