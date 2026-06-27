# kavenio.ConnectApi

All URIs are relative to *https://api.kavenio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**begin_connect**](ConnectApi.md#begin_connect) | **POST** /v1/connect/begin | Begin OAuth connect
[**complete_connect**](ConnectApi.md#complete_connect) | **POST** /v1/connect/complete | Complete OAuth connect
[**complete_hosted_connect_callback**](ConnectApi.md#complete_hosted_connect_callback) | **GET** /v1/connect/callback | Complete hosted OAuth callback
[**complete_token_connect**](ConnectApi.md#complete_token_connect) | **POST** /v1/connect/token | Complete token connect
[**connect_bluesky_credentials**](ConnectApi.md#connect_bluesky_credentials) | **POST** /v1/connect/bluesky/credentials | Connect Bluesky credentials
[**connect_telegram_credentials**](ConnectApi.md#connect_telegram_credentials) | **POST** /v1/connect/telegram/credentials | Connect Telegram credentials
[**list_connect_providers**](ConnectApi.md#list_connect_providers) | **GET** /v1/connect/providers | List connect providers
[**list_facebook_pages**](ConnectApi.md#list_facebook_pages) | **GET** /v1/connect/facebook/pages | List Facebook Pages
[**list_google_business_connect_locations**](ConnectApi.md#list_google_business_connect_locations) | **GET** /v1/connect/googlebusiness/locations | List Google Business connect locations
[**list_instagram_accounts**](ConnectApi.md#list_instagram_accounts) | **GET** /v1/connect/instagram/accounts | List Instagram accounts
[**list_linked_in_organizations**](ConnectApi.md#list_linked_in_organizations) | **GET** /v1/connect/linkedin/organizations | List LinkedIn organizations
[**list_pinterest_boards**](ConnectApi.md#list_pinterest_boards) | **GET** /v1/connect/pinterest/boards | List Pinterest boards
[**list_reddit_flairs**](ConnectApi.md#list_reddit_flairs) | **GET** /v1/connect/reddit/flairs | List Reddit flairs
[**list_reddit_subreddits**](ConnectApi.md#list_reddit_subreddits) | **GET** /v1/connect/reddit/subreddits | List Reddit subreddits
[**list_you_tube_channels**](ConnectApi.md#list_you_tube_channels) | **GET** /v1/connect/youtube/channels | List YouTube channels
[**list_you_tube_playlists**](ConnectApi.md#list_you_tube_playlists) | **GET** /v1/connect/youtube/playlists | List YouTube playlists
[**select_facebook_page**](ConnectApi.md#select_facebook_page) | **POST** /v1/connect/facebook/select-page | Select Facebook Page
[**select_google_business_location**](ConnectApi.md#select_google_business_location) | **POST** /v1/connect/googlebusiness/select-location | Select Google Business location
[**select_instagram_account**](ConnectApi.md#select_instagram_account) | **POST** /v1/connect/instagram/select-account | Select Instagram account
[**select_linked_in_organization**](ConnectApi.md#select_linked_in_organization) | **POST** /v1/connect/linkedin/select-organization | Select LinkedIn organization
[**select_pinterest_board**](ConnectApi.md#select_pinterest_board) | **POST** /v1/connect/pinterest/select-board | Select Pinterest board
[**select_you_tube_channel**](ConnectApi.md#select_you_tube_channel) | **POST** /v1/connect/youtube/select-channel | Select YouTube channel


# **begin_connect**
> BeginConnect200Response begin_connect(begin_connect_request)

Begin OAuth connect

Creates an OAuth connect session and returns the provider authorization URL.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.begin_connect200_response import BeginConnect200Response
from kavenio.models.begin_connect_request import BeginConnectRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    begin_connect_request = {"profileId":"aaaaaaaaaaaaaaaa","platform":"linkedin","returnTo":"/accounts"} # BeginConnectRequest | 

    try:
        # Begin OAuth connect
        api_response = await api_instance.begin_connect(begin_connect_request)
        print("The response of ConnectApi->begin_connect:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->begin_connect: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **begin_connect_request** | [**BeginConnectRequest**](BeginConnectRequest.md)|  | 

### Return type

[**BeginConnect200Response**](BeginConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connect session created. |  -  |
**401** | Authentication failed. |  -  |
**409** | Provider cannot be connected in the current state. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Connect session creation failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **complete_connect**
> CompleteConnect200Response complete_connect(complete_connect_request)

Complete OAuth connect

Completes an OAuth connect session using the provider authorization code.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.complete_connect_request import CompleteConnectRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    complete_connect_request = {"state":"state_example","code":"code_example"} # CompleteConnectRequest | 

    try:
        # Complete OAuth connect
        api_response = await api_instance.complete_connect(complete_connect_request)
        print("The response of ConnectApi->complete_connect:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->complete_connect: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **complete_connect_request** | [**CompleteConnectRequest**](CompleteConnectRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connect session completed. |  -  |
**401** | Authentication failed. |  -  |
**409** | Connect session cannot be completed. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Connect completion failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **complete_hosted_connect_callback**
> complete_hosted_connect_callback(state=state, code=code, error=error)

Complete hosted OAuth callback

Handles provider OAuth redirects for hosted connect flows and redirects back to the Kavenio app with the connection result.

### Example


```python
import kavenio
from kavenio.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.kavenio.com
# See configuration.py for a list of all supported configuration parameters.
configuration = kavenio.Configuration(
    host = "https://api.kavenio.com"
)


# Enter a context with an instance of the API client
async with kavenio.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = kavenio.ConnectApi(api_client)
    state = 'state_example' # str |  (optional)
    code = 'code_example' # str |  (optional)
    error = 'error_example' # str |  (optional)

    try:
        # Complete hosted OAuth callback
        await api_instance.complete_hosted_connect_callback(state=state, code=code, error=error)
    except Exception as e:
        print("Exception when calling ConnectApi->complete_hosted_connect_callback: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **state** | **str**|  | [optional] 
 **code** | **str**|  | [optional] 
 **error** | **str**|  | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**302** | Redirects to the configured Kavenio app completion URL with connection status query parameters. |  -  |
**500** | Hosted connect callback failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **complete_token_connect**
> CompleteConnect200Response complete_token_connect(complete_token_connect_request)

Complete token connect

Connects a provider that requires user-supplied token credentials. Raw tokens are accepted only in the request and are never returned.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.complete_token_connect_request import CompleteTokenConnectRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    complete_token_connect_request = {"profileId":"aaaaaaaaaaaaaaaa","platform":"xads","oauthToken":"oauth_token_redacted","oauthTokenSecret":"oauth_token_secret_redacted","providerAccountId":"provider_account_example","displayName":"Example X Ads account"} # CompleteTokenConnectRequest | 

    try:
        # Complete token connect
        api_response = await api_instance.complete_token_connect(complete_token_connect_request)
        print("The response of ConnectApi->complete_token_connect:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->complete_token_connect: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **complete_token_connect_request** | [**CompleteTokenConnectRequest**](CompleteTokenConnectRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Token connect completed. |  -  |
**401** | Authentication failed. |  -  |
**409** | Provider cannot be connected in the current state. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Token connect failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **connect_bluesky_credentials**
> CompleteConnect200Response connect_bluesky_credentials(connect_bluesky_credentials_request)

Connect Bluesky credentials

Connects a Bluesky account using an identifier and app password. The app password is accepted only in the request and is never returned.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.connect_bluesky_credentials_request import ConnectBlueskyCredentialsRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    connect_bluesky_credentials_request = {"profileId":"aaaaaaaaaaaaaaaa","identifier":"handle.example.com","appPassword":"bluesky_app_password_redacted"} # ConnectBlueskyCredentialsRequest | 

    try:
        # Connect Bluesky credentials
        api_response = await api_instance.connect_bluesky_credentials(connect_bluesky_credentials_request)
        print("The response of ConnectApi->connect_bluesky_credentials:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->connect_bluesky_credentials: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connect_bluesky_credentials_request** | [**ConnectBlueskyCredentialsRequest**](ConnectBlueskyCredentialsRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Bluesky account connected. |  -  |
**401** | Authentication failed. |  -  |
**409** | Bluesky account cannot be connected. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Bluesky credential connect failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **connect_telegram_credentials**
> CompleteConnect200Response connect_telegram_credentials(connect_telegram_credentials_request)

Connect Telegram credentials

Connects a Telegram bot or chat using supplied credentials. The bot token is accepted only in the request and is never returned.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.connect_telegram_credentials_request import ConnectTelegramCredentialsRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    connect_telegram_credentials_request = {"profileId":"aaaaaaaaaaaaaaaa","botToken":"telegram_bot_token_redacted","chatId":"@example_channel","displayName":"Example channel"} # ConnectTelegramCredentialsRequest | 

    try:
        # Connect Telegram credentials
        api_response = await api_instance.connect_telegram_credentials(connect_telegram_credentials_request)
        print("The response of ConnectApi->connect_telegram_credentials:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->connect_telegram_credentials: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **connect_telegram_credentials_request** | [**ConnectTelegramCredentialsRequest**](ConnectTelegramCredentialsRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Telegram account connected. |  -  |
**401** | Authentication failed. |  -  |
**409** | Telegram account cannot be connected. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Telegram credential connect failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_connect_providers**
> ListConnectProviders200Response list_connect_providers()

List connect providers

Returns social and ads providers available to the authenticated user.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_connect_providers200_response import ListConnectProviders200Response
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
    api_instance = kavenio.ConnectApi(api_client)

    try:
        # List connect providers
        api_response = await api_instance.list_connect_providers()
        print("The response of ConnectApi->list_connect_providers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_connect_providers: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ListConnectProviders200Response**](ListConnectProviders200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Connect providers returned. |  -  |
**401** | Authentication failed. |  -  |
**500** | Connect provider lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_facebook_pages**
> ListFacebookPages200Response list_facebook_pages(account_id)

List Facebook Pages

Returns Facebook Pages available from a connected Facebook account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_facebook_pages200_response import ListFacebookPages200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # List Facebook Pages
        api_response = await api_instance.list_facebook_pages(account_id)
        print("The response of ConnectApi->list_facebook_pages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_facebook_pages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**ListFacebookPages200Response**](ListFacebookPages200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Facebook Pages returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Facebook Page lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_google_business_connect_locations**
> ListGoogleBusinessConnectLocations200Response list_google_business_connect_locations(account_id, page_size=page_size, page_token=page_token, search=search, filter=filter)

List Google Business connect locations

Returns Google Business locations available during account connection.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_google_business_connect_locations200_response import ListGoogleBusinessConnectLocations200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 
    page_size = 56 # int |  (optional)
    page_token = 'page_token_example' # str |  (optional)
    search = 'search_example' # str |  (optional)
    filter = 'filter_example' # str |  (optional)

    try:
        # List Google Business connect locations
        api_response = await api_instance.list_google_business_connect_locations(account_id, page_size=page_size, page_token=page_token, search=search, filter=filter)
        print("The response of ConnectApi->list_google_business_connect_locations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_google_business_connect_locations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 
 **page_size** | **int**|  | [optional] 
 **page_token** | **str**|  | [optional] 
 **search** | **str**|  | [optional] 
 **filter** | **str**|  | [optional] 

### Return type

[**ListGoogleBusinessConnectLocations200Response**](ListGoogleBusinessConnectLocations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Google Business locations returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Google Business location lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_instagram_accounts**
> ListInstagramAccounts200Response list_instagram_accounts(account_id)

List Instagram accounts

Returns Instagram business or creator accounts available from a connected account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_instagram_accounts200_response import ListInstagramAccounts200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # List Instagram accounts
        api_response = await api_instance.list_instagram_accounts(account_id)
        print("The response of ConnectApi->list_instagram_accounts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_instagram_accounts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**ListInstagramAccounts200Response**](ListInstagramAccounts200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Instagram accounts returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Instagram account lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_linked_in_organizations**
> ListLinkedInOrganizations200Response list_linked_in_organizations(account_id)

List LinkedIn organizations

Returns LinkedIn organizations available from a connected LinkedIn account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_linked_in_organizations200_response import ListLinkedInOrganizations200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # List LinkedIn organizations
        api_response = await api_instance.list_linked_in_organizations(account_id)
        print("The response of ConnectApi->list_linked_in_organizations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_linked_in_organizations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**ListLinkedInOrganizations200Response**](ListLinkedInOrganizations200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | LinkedIn organizations returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | LinkedIn organization lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_pinterest_boards**
> ListPinterestBoards200Response list_pinterest_boards(account_id)

List Pinterest boards

Returns Pinterest boards available from a connected Pinterest account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_pinterest_boards200_response import ListPinterestBoards200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # List Pinterest boards
        api_response = await api_instance.list_pinterest_boards(account_id)
        print("The response of ConnectApi->list_pinterest_boards:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_pinterest_boards: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**ListPinterestBoards200Response**](ListPinterestBoards200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Pinterest boards returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Pinterest board lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_reddit_flairs**
> ListRedditFlairs200Response list_reddit_flairs(account_id, subreddit)

List Reddit flairs

Returns post flair choices for a connected Reddit account and subreddit.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_reddit_flairs200_response import ListRedditFlairs200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 
    subreddit = 'subreddit_example' # str | 

    try:
        # List Reddit flairs
        api_response = await api_instance.list_reddit_flairs(account_id, subreddit)
        print("The response of ConnectApi->list_reddit_flairs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_reddit_flairs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 
 **subreddit** | **str**|  | 

### Return type

[**ListRedditFlairs200Response**](ListRedditFlairs200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Reddit flairs returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account or subreddit not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Reddit flair lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_reddit_subreddits**
> ListRedditSubreddits200Response list_reddit_subreddits(account_id)

List Reddit subreddits

Returns Reddit subreddits available from a connected Reddit account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_reddit_subreddits200_response import ListRedditSubreddits200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # List Reddit subreddits
        api_response = await api_instance.list_reddit_subreddits(account_id)
        print("The response of ConnectApi->list_reddit_subreddits:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_reddit_subreddits: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**ListRedditSubreddits200Response**](ListRedditSubreddits200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Reddit subreddits returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Reddit subreddit lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_you_tube_channels**
> ListYouTubeChannels200Response list_you_tube_channels(account_id)

List YouTube channels

Returns YouTube channels available from a connected YouTube account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_you_tube_channels200_response import ListYouTubeChannels200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # List YouTube channels
        api_response = await api_instance.list_you_tube_channels(account_id)
        print("The response of ConnectApi->list_you_tube_channels:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_you_tube_channels: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**ListYouTubeChannels200Response**](ListYouTubeChannels200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | YouTube channels returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | YouTube channel lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_you_tube_playlists**
> ListYouTubePlaylists200Response list_you_tube_playlists(account_id)

List YouTube playlists

Returns YouTube playlists available from a connected YouTube account.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_you_tube_playlists200_response import ListYouTubePlaylists200Response
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
    api_instance = kavenio.ConnectApi(api_client)
    account_id = 'account_id_example' # str | 

    try:
        # List YouTube playlists
        api_response = await api_instance.list_you_tube_playlists(account_id)
        print("The response of ConnectApi->list_you_tube_playlists:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->list_you_tube_playlists: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **account_id** | **str**|  | 

### Return type

[**ListYouTubePlaylists200Response**](ListYouTubePlaylists200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | YouTube playlists returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account not found. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | YouTube playlist lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **select_facebook_page**
> CompleteConnect200Response select_facebook_page(select_facebook_page_request)

Select Facebook Page

Selects a Facebook Page destination and attaches it to a profile.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.select_facebook_page_request import SelectFacebookPageRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    select_facebook_page_request = {"accountId":"bbbbbbbbbbbbbbbb","profileId":"aaaaaaaaaaaaaaaa","pageId":"page_example"} # SelectFacebookPageRequest | 

    try:
        # Select Facebook Page
        api_response = await api_instance.select_facebook_page(select_facebook_page_request)
        print("The response of ConnectApi->select_facebook_page:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->select_facebook_page: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **select_facebook_page_request** | [**SelectFacebookPageRequest**](SelectFacebookPageRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Facebook Page selected. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account or Page not found. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Facebook Page selection failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **select_google_business_location**
> CompleteConnect200Response select_google_business_location(select_google_business_location_request)

Select Google Business location

Selects a Google Business location destination and attaches it to a profile.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.select_google_business_location_request import SelectGoogleBusinessLocationRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    select_google_business_location_request = {"accountId":"bbbbbbbbbbbbbbbb","profileId":"aaaaaaaaaaaaaaaa","locationId":"locations/123"} # SelectGoogleBusinessLocationRequest | 

    try:
        # Select Google Business location
        api_response = await api_instance.select_google_business_location(select_google_business_location_request)
        print("The response of ConnectApi->select_google_business_location:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->select_google_business_location: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **select_google_business_location_request** | [**SelectGoogleBusinessLocationRequest**](SelectGoogleBusinessLocationRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Google Business location selected. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account or location not found. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Google Business location selection failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **select_instagram_account**
> CompleteConnect200Response select_instagram_account(select_instagram_account_request)

Select Instagram account

Selects an Instagram account destination and attaches it to a profile.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.select_instagram_account_request import SelectInstagramAccountRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    select_instagram_account_request = {"accountId":"bbbbbbbbbbbbbbbb","profileId":"aaaaaaaaaaaaaaaa","instagramAccountId":"ig_example"} # SelectInstagramAccountRequest | 

    try:
        # Select Instagram account
        api_response = await api_instance.select_instagram_account(select_instagram_account_request)
        print("The response of ConnectApi->select_instagram_account:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->select_instagram_account: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **select_instagram_account_request** | [**SelectInstagramAccountRequest**](SelectInstagramAccountRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Instagram account selected. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account or Instagram account not found. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Instagram account selection failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **select_linked_in_organization**
> CompleteConnect200Response select_linked_in_organization(select_linked_in_organization_request)

Select LinkedIn organization

Selects a LinkedIn organization destination and attaches it to a profile.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.select_linked_in_organization_request import SelectLinkedInOrganizationRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    select_linked_in_organization_request = {"accountId":"bbbbbbbbbbbbbbbb","profileId":"aaaaaaaaaaaaaaaa","organizationUrn":"urn:li:organization:123","displayName":"Example Company"} # SelectLinkedInOrganizationRequest | 

    try:
        # Select LinkedIn organization
        api_response = await api_instance.select_linked_in_organization(select_linked_in_organization_request)
        print("The response of ConnectApi->select_linked_in_organization:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->select_linked_in_organization: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **select_linked_in_organization_request** | [**SelectLinkedInOrganizationRequest**](SelectLinkedInOrganizationRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | LinkedIn organization selected. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account or organization not found. |  -  |
**422** | Request body validation failed. |  -  |
**500** | LinkedIn organization selection failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **select_pinterest_board**
> CompleteConnect200Response select_pinterest_board(select_pinterest_board_request)

Select Pinterest board

Selects a Pinterest board destination and attaches it to a profile.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.select_pinterest_board_request import SelectPinterestBoardRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    select_pinterest_board_request = {"accountId":"bbbbbbbbbbbbbbbb","profileId":"aaaaaaaaaaaaaaaa","boardId":"board_example"} # SelectPinterestBoardRequest | 

    try:
        # Select Pinterest board
        api_response = await api_instance.select_pinterest_board(select_pinterest_board_request)
        print("The response of ConnectApi->select_pinterest_board:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->select_pinterest_board: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **select_pinterest_board_request** | [**SelectPinterestBoardRequest**](SelectPinterestBoardRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Pinterest board selected. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account or board not found. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Pinterest board selection failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **select_you_tube_channel**
> CompleteConnect200Response select_you_tube_channel(select_you_tube_channel_request)

Select YouTube channel

Selects a YouTube channel destination and attaches it to a profile.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.complete_connect200_response import CompleteConnect200Response
from kavenio.models.select_you_tube_channel_request import SelectYouTubeChannelRequest
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
    api_instance = kavenio.ConnectApi(api_client)
    select_you_tube_channel_request = {"accountId":"bbbbbbbbbbbbbbbb","profileId":"aaaaaaaaaaaaaaaa","channelId":"channel_example"} # SelectYouTubeChannelRequest | 

    try:
        # Select YouTube channel
        api_response = await api_instance.select_you_tube_channel(select_you_tube_channel_request)
        print("The response of ConnectApi->select_you_tube_channel:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ConnectApi->select_you_tube_channel: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **select_you_tube_channel_request** | [**SelectYouTubeChannelRequest**](SelectYouTubeChannelRequest.md)|  | 

### Return type

[**CompleteConnect200Response**](CompleteConnect200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | YouTube channel selected. |  -  |
**401** | Authentication failed. |  -  |
**404** | Connected account or channel not found. |  -  |
**422** | Request body validation failed. |  -  |
**500** | YouTube channel selection failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

