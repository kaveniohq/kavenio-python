# kavenio.AccountsApi

All URIs are relative to *https://api.kavenio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**check_account_health**](AccountsApi.md#check_account_health) | **POST** /v1/accounts/{accountId}/health | Check account health
[**disconnect_account**](AccountsApi.md#disconnect_account) | **POST** /v1/accounts/{accountId}/disconnect | Disconnect an account
[**get_account**](AccountsApi.md#get_account) | **GET** /v1/accounts/{accountId} | Get a connected account
[**list_accounts**](AccountsApi.md#list_accounts) | **GET** /v1/accounts | List connected accounts
[**move_account**](AccountsApi.md#move_account) | **POST** /v1/accounts/{accountId}/move | Move a connected account
[**refresh_tik_tok_creator_info**](AccountsApi.md#refresh_tik_tok_creator_info) | **POST** /v1/accounts/{accountId}/tiktok/creator-info | Refresh TikTok creator info
[**replace_account**](AccountsApi.md#replace_account) | **PUT** /v1/accounts/{accountId} | Replace account fields
[**update_account**](AccountsApi.md#update_account) | **PATCH** /v1/accounts/{accountId} | Update a connected account


# **check_account_health**
> CheckAccountHealth200Response check_account_health(account_id)

Check account health

Refreshes account health and readiness information for a connected account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.check_account_health200_response import CheckAccountHealth200Response
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
    api_instance = kavenio.AccountsApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # Check account health
        api_response = await api_instance.check_account_health(account_id)
        print("The response of AccountsApi->check_account_health:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountsApi->check_account_health: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**CheckAccountHealth200Response**](CheckAccountHealth200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Account health returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Path parameter validation failed. |  -  |
**500** | Account health check failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **disconnect_account**
> DisconnectAccount200Response disconnect_account(account_id)

Disconnect an account

Disconnects a connected account and returns the resulting account state.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.disconnect_account200_response import DisconnectAccount200Response
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
    api_instance = kavenio.AccountsApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # Disconnect an account
        api_response = await api_instance.disconnect_account(account_id)
        print("The response of AccountsApi->disconnect_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountsApi->disconnect_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**DisconnectAccount200Response**](DisconnectAccount200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connected account disconnected. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**409** | Connected account cannot be disconnected. |  -  |
**422** | Path parameter validation failed. |  -  |
**500** | Connected account disconnect failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_account**
> GetAccount200Response get_account(account_id)

Get a connected account

Returns one connected account by ID.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.get_account200_response import GetAccount200Response
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
    api_instance = kavenio.AccountsApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # Get a connected account
        api_response = await api_instance.get_account(account_id)
        print("The response of AccountsApi->get_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountsApi->get_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**GetAccount200Response**](GetAccount200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connected account returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Path parameter validation failed. |  -  |
**500** | Connected account lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_accounts**
> ListAccounts200Response list_accounts(profile_id=profile_id, platform=platform, status=status, limit=limit, cursor=cursor)

List connected accounts

Returns connected social accounts for the authenticated organization.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_accounts200_response import ListAccounts200Response
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
    api_instance = kavenio.AccountsApi(api_client)
    profile_id = 'profile_id_example' # str |  (optional)
    platform = 'platform_example' # str |  (optional)
    status = 'status_example' # str |  (optional)
    limit = 56 # int |  (optional)
    cursor = 'cursor_example' # str |  (optional)

    try:
        # List connected accounts
        api_response = await api_instance.list_accounts(profile_id=profile_id, platform=platform, status=status, limit=limit, cursor=cursor)
        print("The response of AccountsApi->list_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountsApi->list_accounts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | [optional] 
 **platform** | **str**|  | [optional] 
 **status** | **str**|  | [optional] 
 **limit** | **int**|  | [optional] 
 **cursor** | **str**|  | [optional] 

### Return type

[**ListAccounts200Response**](ListAccounts200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connected accounts returned. |  -  |
**401** | Authentication failed. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Connected account lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **move_account**
> GetAccount200Response move_account(account_id, move_account_request)

Move a connected account

Moves a connected account to another profile.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.get_account200_response import GetAccount200Response
from kavenio.models.move_account_request import MoveAccountRequest
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
    api_instance = kavenio.AccountsApi(api_client)
    account_id = 'account_id_example' # str | 
    move_account_request = {"profileId":"aaaaaaaaaaaaaaaa"} # MoveAccountRequest | 

    try:
        # Move a connected account
        api_response = await api_instance.move_account(account_id, move_account_request)
        print("The response of AccountsApi->move_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountsApi->move_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 
 **move_account_request** | [**MoveAccountRequest**](MoveAccountRequest.md)|  | 

### Return type

[**GetAccount200Response**](GetAccount200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connected account moved. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account or profile not found. |  -  |
**409** | Connected account cannot be moved. |  -  |
**422** | Request validation failed. |  -  |
**500** | Connected account move failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **refresh_tik_tok_creator_info**
> RefreshTikTokCreatorInfo200Response refresh_tik_tok_creator_info(account_id)

Refresh TikTok creator info

Refreshes TikTok creator information and posting readiness for a connected account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.refresh_tik_tok_creator_info200_response import RefreshTikTokCreatorInfo200Response
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
    api_instance = kavenio.AccountsApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # Refresh TikTok creator info
        api_response = await api_instance.refresh_tik_tok_creator_info(account_id)
        print("The response of AccountsApi->refresh_tik_tok_creator_info:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountsApi->refresh_tik_tok_creator_info: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**RefreshTikTokCreatorInfo200Response**](RefreshTikTokCreatorInfo200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | TikTok creator information returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Path parameter validation failed. |  -  |
**500** | TikTok creator information refresh failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **replace_account**
> GetAccount200Response replace_account(account_id, replace_account_request)

Replace account fields

Updates editable connected account fields. Public metadata updates must not include provider credential fields.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.get_account200_response import GetAccount200Response
from kavenio.models.replace_account_request import ReplaceAccountRequest
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
    api_instance = kavenio.AccountsApi(api_client)
    account_id = 'account_id_example' # str | 
    replace_account_request = {"displayName":"Retail LinkedIn","enabled":true,"metadata":{"label":"primary"}} # ReplaceAccountRequest | 

    try:
        # Replace account fields
        api_response = await api_instance.replace_account(account_id, replace_account_request)
        print("The response of AccountsApi->replace_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountsApi->replace_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 
 **replace_account_request** | [**ReplaceAccountRequest**](ReplaceAccountRequest.md)|  | 

### Return type

[**GetAccount200Response**](GetAccount200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connected account updated. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**409** | Connected account cannot be updated. |  -  |
**422** | Request validation failed. |  -  |
**500** | Connected account update failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_account**
> GetAccount200Response update_account(account_id, replace_account_request)

Update a connected account

Partially updates editable connected account fields. Public metadata updates must not include provider credential fields.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.get_account200_response import GetAccount200Response
from kavenio.models.replace_account_request import ReplaceAccountRequest
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
    api_instance = kavenio.AccountsApi(api_client)
    account_id = 'account_id_example' # str | 
    replace_account_request = {"enabled":false} # ReplaceAccountRequest | 

    try:
        # Update a connected account
        api_response = await api_instance.update_account(account_id, replace_account_request)
        print("The response of AccountsApi->update_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccountsApi->update_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 
 **replace_account_request** | [**ReplaceAccountRequest**](ReplaceAccountRequest.md)|  | 

### Return type

[**GetAccount200Response**](GetAccount200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connected account updated. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**409** | Connected account cannot be updated. |  -  |
**422** | Request validation failed. |  -  |
**500** | Connected account update failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

