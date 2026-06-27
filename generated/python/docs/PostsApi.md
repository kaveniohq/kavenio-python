# kavenio.PostsApi

All URIs are relative to *https://api.kavenio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulk_upload_posts**](PostsApi.md#bulk_upload_posts) | **POST** /v1/posts/bulk-upload | Bulk upload posts
[**create_post**](PostsApi.md#create_post) | **POST** /v1/posts | Create a post
[**delete_post**](PostsApi.md#delete_post) | **DELETE** /v1/posts/{postId} | Delete a post
[**edit_published_post**](PostsApi.md#edit_published_post) | **POST** /v1/posts/{postId}/edit | Edit a published post
[**get_post**](PostsApi.md#get_post) | **GET** /v1/posts/{postId} | Get a post
[**list_posts**](PostsApi.md#list_posts) | **GET** /v1/posts | List posts
[**replace_post**](PostsApi.md#replace_post) | **PUT** /v1/posts/{postId} | Replace post fields
[**retry_post**](PostsApi.md#retry_post) | **POST** /v1/posts/{postId}/retry | Retry post publishing
[**unpublish_post**](PostsApi.md#unpublish_post) | **POST** /v1/posts/{postId}/unpublish | Unpublish a post
[**update_post**](PostsApi.md#update_post) | **PATCH** /v1/posts/{postId} | Update a post


# **bulk_upload_posts**
> BulkUploadPosts201Response bulk_upload_posts(bulk_upload_posts_request)

Bulk upload posts

Creates posts from CSV content and returns per-row creation or validation results.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.bulk_upload_posts201_response import BulkUploadPosts201Response
from kavenio.models.bulk_upload_posts_request import BulkUploadPostsRequest
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
    api_instance = kavenio.PostsApi(api_client)
    bulk_upload_posts_request = {"csv":"title,content,scheduledFor\nLaunch,Post body,2026-06-25T15:00:00.000Z","defaults":{"profileId":"aaaaaaaaaaaaaaaa","timezone":"UTC"}} # BulkUploadPostsRequest | 

    try:
        # Bulk upload posts
        api_response = await api_instance.bulk_upload_posts(bulk_upload_posts_request)
        print("The response of PostsApi->bulk_upload_posts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->bulk_upload_posts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulk_upload_posts_request** | [**BulkUploadPostsRequest**](BulkUploadPostsRequest.md)|  | 

### Return type

[**BulkUploadPosts201Response**](BulkUploadPosts201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Bulk upload processed. |  -  |
**401** | Authentication failed. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Bulk upload failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_post**
> CreatePost201Response create_post(create_post_request)

Create a post

Creates a draft, scheduled post, queue-backed post, or immediate publish request depending on the payload fields.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_post201_response import CreatePost201Response
from kavenio.models.create_post_request import CreatePostRequest
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
    api_instance = kavenio.PostsApi(api_client)
    create_post_request = {"profileId":"aaaaaaaaaaaaaaaa","title":"Launch announcement","content":"We are launching the new campaign today.","platforms":[{"platform":"linkedin","accountId":"bbbbbbbbbbbbbbbb"}],"scheduledFor":"2026-06-25T15:00:00.000Z","timezone":"UTC","tags":["launch"]} # CreatePostRequest | 

    try:
        # Create a post
        api_response = await api_instance.create_post(create_post_request)
        print("The response of PostsApi->create_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->create_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_post_request** | [**CreatePostRequest**](CreatePostRequest.md)|  | 

### Return type

[**CreatePost201Response**](CreatePost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Post created. |  -  |
**401** | Authentication failed. |  -  |
**409** | Post request conflicts with current state. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Post creation failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_post**
> DeletePost200Response delete_post(post_id)

Delete a post

Deletes a post by ID and returns the deletion count.

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
    api_instance = kavenio.PostsApi(api_client)
    post_id = 'post_id_example' # str | 

    try:
        # Delete a post
        api_response = await api_instance.delete_post(post_id)
        print("The response of PostsApi->delete_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->delete_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_id** | **str**|  | 

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
**200** | Post deleted. |  -  |
**401** | Authentication failed. |  -  |
**404** | Post not found. |  -  |
**409** | Post cannot be deleted in its current state. |  -  |
**422** | Path parameter validation failed. |  -  |
**500** | Post deletion failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_published_post**
> CreatePost201Response edit_published_post(post_id, edit_published_post_request)

Edit a published post

Applies supported lifecycle edits to published platform targets and returns the resulting post state.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_post201_response import CreatePost201Response
from kavenio.models.edit_published_post_request import EditPublishedPostRequest
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
    api_instance = kavenio.PostsApi(api_client)
    post_id = 'post_id_example' # str | 
    edit_published_post_request = {"targetIds":["gggggggggggggggg"],"content":"Updated published content.","visibility":"public"} # EditPublishedPostRequest | 

    try:
        # Edit a published post
        api_response = await api_instance.edit_published_post(post_id, edit_published_post_request)
        print("The response of PostsApi->edit_published_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->edit_published_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_id** | **str**|  | 
 **edit_published_post_request** | [**EditPublishedPostRequest**](EditPublishedPostRequest.md)|  | 

### Return type

[**CreatePost201Response**](CreatePost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Published post edit processed. |  -  |
**401** | Authentication failed. |  -  |
**404** | Post not found. |  -  |
**409** | Post cannot be edited in its current state. |  -  |
**422** | Request validation failed. |  -  |
**500** | Published post edit failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_post**
> CreatePost201Response get_post(post_id)

Get a post

Returns a post by ID, including platform target state.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_post201_response import CreatePost201Response
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
    api_instance = kavenio.PostsApi(api_client)
    post_id = 'post_id_example' # str | 

    try:
        # Get a post
        api_response = await api_instance.get_post(post_id)
        print("The response of PostsApi->get_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->get_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_id** | **str**|  | 

### Return type

[**CreatePost201Response**](CreatePost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Post returned. |  -  |
**401** | Authentication failed. |  -  |
**404** | Post not found. |  -  |
**422** | Path parameter validation failed. |  -  |
**500** | Post lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_posts**
> ListPosts200Response list_posts(profile_id=profile_id, account_id=account_id, platform=platform, status=status, search=search, from_date=from_date, to_date=to_date, page=page, limit=limit)

List posts

Returns posts for the authenticated organization, optionally filtered by profile, account, platform, status, search text, or date range.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.list_posts200_response import ListPosts200Response
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
    api_instance = kavenio.PostsApi(api_client)
    profile_id = 'profile_id_example' # str |  (optional)
    account_id = 'account_id_example' # str |  (optional)
    platform = 'platform_example' # str |  (optional)
    status = 'status_example' # str |  (optional)
    search = 'search_example' # str |  (optional)
    from_date = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    to_date = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    page = 56 # int |  (optional)
    limit = 56 # int |  (optional)

    try:
        # List posts
        api_response = await api_instance.list_posts(profile_id=profile_id, account_id=account_id, platform=platform, status=status, search=search, from_date=from_date, to_date=to_date, page=page, limit=limit)
        print("The response of PostsApi->list_posts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->list_posts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **profile_id** | **str**|  | [optional] 
 **account_id** | **str**|  | [optional] 
 **platform** | **str**|  | [optional] 
 **status** | **str**|  | [optional] 
 **search** | **str**|  | [optional] 
 **from_date** | **datetime**|  | [optional] 
 **to_date** | **datetime**|  | [optional] 
 **page** | **int**|  | [optional] 
 **limit** | **int**|  | [optional] 

### Return type

[**ListPosts200Response**](ListPosts200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Posts returned. |  -  |
**401** | Authentication failed. |  -  |
**422** | Query parameter validation failed. |  -  |
**500** | Post lookup failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **replace_post**
> CreatePost201Response replace_post(post_id, replace_post_request)

Replace post fields

Updates editable fields on an existing post and returns the resulting post state.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_post201_response import CreatePost201Response
from kavenio.models.replace_post_request import ReplacePostRequest
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
    api_instance = kavenio.PostsApi(api_client)
    post_id = 'post_id_example' # str | 
    replace_post_request = {"title":"Updated launch announcement","content":"Updated post body.","scheduledFor":"2026-06-25T16:00:00.000Z","timezone":"UTC"} # ReplacePostRequest | 

    try:
        # Replace post fields
        api_response = await api_instance.replace_post(post_id, replace_post_request)
        print("The response of PostsApi->replace_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->replace_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_id** | **str**|  | 
 **replace_post_request** | [**ReplacePostRequest**](ReplacePostRequest.md)|  | 

### Return type

[**CreatePost201Response**](CreatePost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Post updated. |  -  |
**401** | Authentication failed. |  -  |
**404** | Post not found. |  -  |
**409** | Post cannot be updated in its current state. |  -  |
**422** | Request validation failed. |  -  |
**500** | Post update failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **retry_post**
> CreatePost201Response retry_post(post_id, retry_post_request)

Retry post publishing

Retries failed platform targets for a post, optionally limited to specific target IDs.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_post201_response import CreatePost201Response
from kavenio.models.retry_post_request import RetryPostRequest
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
    api_instance = kavenio.PostsApi(api_client)
    post_id = 'post_id_example' # str | 
    retry_post_request = {"targetIds":["gggggggggggggggg"]} # RetryPostRequest | 

    try:
        # Retry post publishing
        api_response = await api_instance.retry_post(post_id, retry_post_request)
        print("The response of PostsApi->retry_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->retry_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_id** | **str**|  | 
 **retry_post_request** | [**RetryPostRequest**](RetryPostRequest.md)|  | 

### Return type

[**CreatePost201Response**](CreatePost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Post retry started. |  -  |
**401** | Authentication failed. |  -  |
**404** | Post not found. |  -  |
**409** | Post cannot be retried in its current state. |  -  |
**422** | Request validation failed. |  -  |
**500** | Post retry failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **unpublish_post**
> CreatePost201Response unpublish_post(post_id, unpublish_post_request)

Unpublish a post

Starts unpublishing for published platform targets, optionally limited to specific target IDs.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_post201_response import CreatePost201Response
from kavenio.models.unpublish_post_request import UnpublishPostRequest
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
    api_instance = kavenio.PostsApi(api_client)
    post_id = 'post_id_example' # str | 
    unpublish_post_request = {"targetIds":["gggggggggggggggg"]} # UnpublishPostRequest | 

    try:
        # Unpublish a post
        api_response = await api_instance.unpublish_post(post_id, unpublish_post_request)
        print("The response of PostsApi->unpublish_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->unpublish_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_id** | **str**|  | 
 **unpublish_post_request** | [**UnpublishPostRequest**](UnpublishPostRequest.md)|  | 

### Return type

[**CreatePost201Response**](CreatePost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Post unpublish started. |  -  |
**401** | Authentication failed. |  -  |
**404** | Post not found. |  -  |
**409** | Post cannot be unpublished in its current state. |  -  |
**422** | Request validation failed. |  -  |
**500** | Post unpublish failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_post**
> CreatePost201Response update_post(post_id, replace_post_request)

Update a post

Partially updates editable fields on an existing post and returns the resulting post state.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_post201_response import CreatePost201Response
from kavenio.models.replace_post_request import ReplacePostRequest
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
    api_instance = kavenio.PostsApi(api_client)
    post_id = 'post_id_example' # str | 
    replace_post_request = {"content":"Updated post body."} # ReplacePostRequest | 

    try:
        # Update a post
        api_response = await api_instance.update_post(post_id, replace_post_request)
        print("The response of PostsApi->update_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PostsApi->update_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **post_id** | **str**|  | 
 **replace_post_request** | [**ReplacePostRequest**](ReplacePostRequest.md)|  | 

### Return type

[**CreatePost201Response**](CreatePost201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Post updated. |  -  |
**401** | Authentication failed. |  -  |
**404** | Post not found. |  -  |
**409** | Post cannot be updated in its current state. |  -  |
**422** | Request validation failed. |  -  |
**500** | Post update failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

