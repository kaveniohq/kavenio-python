# kavenio.QueueApi

All URIs are relative to *https://api.kavenio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_queue_slot_schedule**](QueueApi.md#create_queue_slot_schedule) | **POST** /v1/queue/slots | Create a queue schedule
[**delete_queue_slot_schedule**](QueueApi.md#delete_queue_slot_schedule) | **DELETE** /v1/queue/slots | Delete a queue schedule
[**get_next_queue_slot**](QueueApi.md#get_next_queue_slot) | **GET** /v1/queue/next-slot | Get next queue slot
[**list_queue_slots**](QueueApi.md#list_queue_slots) | **GET** /v1/queue/slots | List queue schedules
[**preview_queue_slots**](QueueApi.md#preview_queue_slots) | **GET** /v1/queue/preview | Preview queue slots
[**update_queue_slot_schedule**](QueueApi.md#update_queue_slot_schedule) | **PUT** /v1/queue/slots | Update a queue schedule


# **create_queue_slot_schedule**
> UpdateQueueSlotSchedule200Response create_queue_slot_schedule(create_queue_slot_schedule_request)

Create a queue schedule

Creates a reusable posting queue schedule for a profile.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_queue_slot_schedule_request import CreateQueueSlotScheduleRequest
from kavenio.models.update_queue_slot_schedule200_response import UpdateQueueSlotSchedule200Response
from kavenio.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.kavenio.com
# See configuration.py for a list of all supported configuration parameters.
configuration = kavenio.Configuration(
    host = "https://api.kavenio.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (Clerk session or OAuth token): bearerAuth
configuration = kavenio.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
async with kavenio.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kavenio.QueueApi(api_client)
    create_queue_slot_schedule_request = {"profileId":"aaaaaaaaaaaaaaaa","name":"Weekday mornings","timezone":"UTC","active":true,"slots":[{"dayOfWeek":1,"time":"09:00","timezone":"UTC"}]} # CreateQueueSlotScheduleRequest | 

    try:
        # Create a queue schedule
        api_response = await api_instance.create_queue_slot_schedule(create_queue_slot_schedule_request)
        print("The response of QueueApi->create_queue_slot_schedule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueueApi->create_queue_slot_schedule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_queue_slot_schedule_request** | [**CreateQueueSlotScheduleRequest**](CreateQueueSlotScheduleRequest.md)|  | 

### Return type

[**UpdateQueueSlotSchedule200Response**](UpdateQueueSlotSchedule200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Queue schedule created. |  -  |
**401** | Authentication failed. |  -  |
**409** | Queue schedule conflicts with current state. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Queue creation failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_queue_slot_schedule**
> DeletePost200Response delete_queue_slot_schedule(profile_id, queue_id)

Delete a queue schedule

Deletes a reusable posting queue schedule by profile and queue ID.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.delete_post200_response import DeletePost200Response
from kavenio.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.kavenio.com
# See configuration.py for a list of all supported configuration parameters.
configuration = kavenio.Configuration(
    host = "https://api.kavenio.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (Clerk session or OAuth token): bearerAuth
configuration = kavenio.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
async with kavenio.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kavenio.QueueApi(api_client)
    profile_id = 'profile_id_example' # str | 
    queue_id = 'queue_id_example' # str | 

    try:
        # Delete a queue schedule
        api_response = await api_instance.delete_queue_slot_schedule(profile_id, queue_id)
        print("The response of QueueApi->delete_queue_slot_schedule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueueApi->delete_queue_slot_schedule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 
 **queue_id** | **str**|  | 

### Return type

[**DeletePost200Response**](DeletePost200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Queue schedule deleted. |  -  |
**401** | Authentication failed. |  -  |
**404** | Queue schedule not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Queue deletion failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_next_queue_slot**
> PreviewQueueSlots200Response get_next_queue_slot(profile_id, queue_id=queue_id, after=after)

Get next queue slot

Returns the next scheduled posting slot for a profile queue. The response uses the queue preview shape with at most one slot.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.preview_queue_slots200_response import PreviewQueueSlots200Response
from kavenio.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.kavenio.com
# See configuration.py for a list of all supported configuration parameters.
configuration = kavenio.Configuration(
    host = "https://api.kavenio.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (Clerk session or OAuth token): bearerAuth
configuration = kavenio.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
async with kavenio.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kavenio.QueueApi(api_client)
    profile_id = 'profile_id_example' # str | 
    queue_id = 'queue_id_example' # str |  (optional)
    after = '2013-10-20T19:20:30+01:00' # datetime |  (optional)

    try:
        # Get next queue slot
        api_response = await api_instance.get_next_queue_slot(profile_id, queue_id=queue_id, after=after)
        print("The response of QueueApi->get_next_queue_slot:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueueApi->get_next_queue_slot: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 
 **queue_id** | **str**|  | [optional] 
 **after** | **datetime**|  | [optional] 

### Return type

[**PreviewQueueSlots200Response**](PreviewQueueSlots200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Next queue slot returned. |  -  |
**401** | Authentication failed. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Next queue slot lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_queue_slots**
> ListQueueSlots200Response list_queue_slots(profile_id, queue_id=queue_id, all=all)

List queue schedules

Returns queue schedules for a profile, optionally filtered to one queue.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_queue_slots200_response import ListQueueSlots200Response
from kavenio.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.kavenio.com
# See configuration.py for a list of all supported configuration parameters.
configuration = kavenio.Configuration(
    host = "https://api.kavenio.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (Clerk session or OAuth token): bearerAuth
configuration = kavenio.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
async with kavenio.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kavenio.QueueApi(api_client)
    profile_id = 'profile_id_example' # str | 
    queue_id = 'queue_id_example' # str |  (optional)
    all = 'all_example' # str |  (optional)

    try:
        # List queue schedules
        api_response = await api_instance.list_queue_slots(profile_id, queue_id=queue_id, all=all)
        print("The response of QueueApi->list_queue_slots:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueueApi->list_queue_slots: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 
 **queue_id** | **str**|  | [optional] 
 **all** | **str**|  | [optional] 

### Return type

[**ListQueueSlots200Response**](ListQueueSlots200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Queue schedules returned. |  -  |
**401** | Authentication failed. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Queue lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **preview_queue_slots**
> PreviewQueueSlots200Response preview_queue_slots(profile_id, queue_id=queue_id, count=count, after=after)

Preview queue slots

Returns upcoming scheduled times for a profile queue without creating posts.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.preview_queue_slots200_response import PreviewQueueSlots200Response
from kavenio.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.kavenio.com
# See configuration.py for a list of all supported configuration parameters.
configuration = kavenio.Configuration(
    host = "https://api.kavenio.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (Clerk session or OAuth token): bearerAuth
configuration = kavenio.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
async with kavenio.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kavenio.QueueApi(api_client)
    profile_id = 'profile_id_example' # str | 
    queue_id = 'queue_id_example' # str |  (optional)
    count = 56 # int |  (optional)
    after = '2013-10-20T19:20:30+01:00' # datetime |  (optional)

    try:
        # Preview queue slots
        api_response = await api_instance.preview_queue_slots(profile_id, queue_id=queue_id, count=count, after=after)
        print("The response of QueueApi->preview_queue_slots:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueueApi->preview_queue_slots: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 
 **queue_id** | **str**|  | [optional] 
 **count** | **int**|  | [optional] 
 **after** | **datetime**|  | [optional] 

### Return type

[**PreviewQueueSlots200Response**](PreviewQueueSlots200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Queue preview returned. |  -  |
**401** | Authentication failed. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Queue preview failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_queue_slot_schedule**
> UpdateQueueSlotSchedule200Response update_queue_slot_schedule(update_queue_slot_schedule_request)

Update a queue schedule

Updates a reusable posting queue schedule and returns the resulting schedule.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.update_queue_slot_schedule200_response import UpdateQueueSlotSchedule200Response
from kavenio.models.update_queue_slot_schedule_request import UpdateQueueSlotScheduleRequest
from kavenio.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.kavenio.com
# See configuration.py for a list of all supported configuration parameters.
configuration = kavenio.Configuration(
    host = "https://api.kavenio.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (Clerk session or OAuth token): bearerAuth
configuration = kavenio.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
async with kavenio.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kavenio.QueueApi(api_client)
    update_queue_slot_schedule_request = {"profileId":"aaaaaaaaaaaaaaaa","queueId":"ffffffffffffffff","name":"Weekday afternoons","slots":[{"dayOfWeek":2,"time":"14:00","timezone":"UTC"}]} # UpdateQueueSlotScheduleRequest | 

    try:
        # Update a queue schedule
        api_response = await api_instance.update_queue_slot_schedule(update_queue_slot_schedule_request)
        print("The response of QueueApi->update_queue_slot_schedule:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueueApi->update_queue_slot_schedule: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **update_queue_slot_schedule_request** | [**UpdateQueueSlotScheduleRequest**](UpdateQueueSlotScheduleRequest.md)|  | 

### Return type

[**UpdateQueueSlotSchedule200Response**](UpdateQueueSlotSchedule200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Queue schedule updated. |  -  |
**401** | Authentication failed. |  -  |
**404** | Queue schedule not found. |  -  |
**409** | Queue schedule conflicts with current state. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Queue update failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

