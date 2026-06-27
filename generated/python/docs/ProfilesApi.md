# kavenio.ProfilesApi

All URIs are relative to *https://api.kavenio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_profile**](ProfilesApi.md#create_profile) | **POST** /v1/profiles | Create a profile
[**delete_profile**](ProfilesApi.md#delete_profile) | **DELETE** /v1/profiles/{profileId} | Delete a profile
[**get_profile**](ProfilesApi.md#get_profile) | **GET** /v1/profiles/{profileId} | Get a profile
[**list_profiles**](ProfilesApi.md#list_profiles) | **GET** /v1/profiles | List profiles
[**replace_profile**](ProfilesApi.md#replace_profile) | **PUT** /v1/profiles/{profileId} | Replace profile fields
[**update_profile**](ProfilesApi.md#update_profile) | **PATCH** /v1/profiles/{profileId} | Update a profile


# **create_profile**
> CreateProfile201Response create_profile(create_profile_request)

Create a profile

Creates a customer-owned profile grouping.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_profile201_response import CreateProfile201Response
from kavenio.models.create_profile_request import CreateProfileRequest
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
    api_instance = kavenio.ProfilesApi(api_client)
    create_profile_request = {"name":"Retail campaigns","description":"Campaigns managed by the retail team.","color":"#2563eb","isDefault":false} # CreateProfileRequest | 

    try:
        # Create a profile
        api_response = await api_instance.create_profile(create_profile_request)
        print("The response of ProfilesApi->create_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->create_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_profile_request** | [**CreateProfileRequest**](CreateProfileRequest.md)|  | 

### Return type

[**CreateProfile201Response**](CreateProfile201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Profile created. |  -  |
**401** | Authentication failed. |  -  |
**409** | A profile with this name already exists. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Profile creation failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_profile**
> DeleteProfile200Response delete_profile(profile_id)

Delete a profile

Deletes a customer-owned profile grouping.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.delete_profile200_response import DeleteProfile200Response
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
    api_instance = kavenio.ProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 

    try:
        # Delete a profile
        api_response = await api_instance.delete_profile(profile_id)
        print("The response of ProfilesApi->delete_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->delete_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 

### Return type

[**DeleteProfile200Response**](DeleteProfile200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Profile deleted. |  -  |
**401** | Authentication failed. |  -  |
**404** | Profile not found. |  -  |
**409** | Profile cannot be deleted in its current state. |  -  |
**422** | Path parameter validation failed. |  -  |
**500** | Profile deletion failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_profile**
> CreateProfile201Response get_profile(profile_id)

Get a profile

Returns one profile by ID.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_profile201_response import CreateProfile201Response
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
    api_instance = kavenio.ProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 

    try:
        # Get a profile
        api_response = await api_instance.get_profile(profile_id)
        print("The response of ProfilesApi->get_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->get_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 

### Return type

[**CreateProfile201Response**](CreateProfile201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Profile returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Profile not found. |  -  |
**422** | Path parameter validation failed. |  -  |
**500** | Profile lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_profiles**
> ListProfiles200Response list_profiles()

List profiles

Returns the profiles available to the authenticated organization.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_profiles200_response import ListProfiles200Response
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
    api_instance = kavenio.ProfilesApi(api_client)

    try:
        # List profiles
        api_response = await api_instance.list_profiles()
        print("The response of ProfilesApi->list_profiles:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->list_profiles: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ListProfiles200Response**](ListProfiles200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Profiles returned. |  -  |
**401** | Authentication failed. |  -  |
**500** | Profile lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **replace_profile**
> CreateProfile201Response replace_profile(profile_id, replace_profile_request)

Replace profile fields

Updates profile fields for an existing customer-owned grouping.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_profile201_response import CreateProfile201Response
from kavenio.models.replace_profile_request import ReplaceProfileRequest
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
    api_instance = kavenio.ProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 
    replace_profile_request = {"name":"Retail campaigns","description":"Updated profile description.","color":"#0f766e","isDefault":true} # ReplaceProfileRequest | 

    try:
        # Replace profile fields
        api_response = await api_instance.replace_profile(profile_id, replace_profile_request)
        print("The response of ProfilesApi->replace_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->replace_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 
 **replace_profile_request** | [**ReplaceProfileRequest**](ReplaceProfileRequest.md)|  | 

### Return type

[**CreateProfile201Response**](CreateProfile201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Profile updated. |  -  |
**401** | Authentication failed. |  -  |
**404** | Profile not found. |  -  |
**409** | A profile with this name already exists. |  -  |
**422** | Request validation failed. |  -  |
**500** | Profile update failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_profile**
> CreateProfile201Response update_profile(profile_id, replace_profile_request)

Update a profile

Partially updates profile fields for an existing customer-owned grouping.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_profile201_response import CreateProfile201Response
from kavenio.models.replace_profile_request import ReplaceProfileRequest
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
    api_instance = kavenio.ProfilesApi(api_client)
    profile_id = 'profile_id_example' # str | 
    replace_profile_request = {"description":null,"isDefault":true} # ReplaceProfileRequest | 

    try:
        # Update a profile
        api_response = await api_instance.update_profile(profile_id, replace_profile_request)
        print("The response of ProfilesApi->update_profile:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProfilesApi->update_profile: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | 
 **replace_profile_request** | [**ReplaceProfileRequest**](ReplaceProfileRequest.md)|  | 

### Return type

[**CreateProfile201Response**](CreateProfile201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Profile updated. |  -  |
**401** | Authentication failed. |  -  |
**404** | Profile not found. |  -  |
**409** | A profile with this name already exists. |  -  |
**422** | Request validation failed. |  -  |
**500** | Profile update failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

