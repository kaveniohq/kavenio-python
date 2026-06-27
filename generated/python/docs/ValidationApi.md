# kavenio.ValidationApi

All URIs are relative to *https://api.kavenio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**validate_post**](ValidationApi.md#validate_post) | **POST** /v1/tools/validate/post | Validate a post
[**validate_post_length**](ValidationApi.md#validate_post_length) | **POST** /v1/tools/validate/post-length | Validate post length


# **validate_post**
> ValidatePost200Response validate_post(create_post_request)

Validate a post

Validates a post payload against platform and scheduling rules without creating a post.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_post_request import CreatePostRequest
from kavenio.models.validate_post200_response import ValidatePost200Response
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
    api_instance = kavenio.ValidationApi(api_client)
    create_post_request = {"profileId":"aaaaaaaaaaaaaaaa","content":"Validation-only post body.","platforms":[{"platform":"linkedin","accountId":"bbbbbbbbbbbbbbbb"}]} # CreatePostRequest | 

    try:
        # Validate a post
        api_response = await api_instance.validate_post(create_post_request)
        print("The response of ValidationApi->validate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationApi->validate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_post_request** | [**CreatePostRequest**](CreatePostRequest.md)|  | 

### Return type

[**ValidatePost200Response**](ValidatePost200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Post validation result returned. |  -  |
**401** | Authentication failed. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Post validation failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_post_length**
> ValidatePostLength200Response validate_post_length(validate_post_length_request)

Validate post length

Returns character counts and per-platform length validity for the supplied text.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.validate_post_length200_response import ValidatePostLength200Response
from kavenio.models.validate_post_length_request import ValidatePostLengthRequest
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
    api_instance = kavenio.ValidationApi(api_client)
    validate_post_length_request = {"text":"Short post text for platform length validation."} # ValidatePostLengthRequest | 

    try:
        # Validate post length
        api_response = await api_instance.validate_post_length(validate_post_length_request)
        print("The response of ValidationApi->validate_post_length:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationApi->validate_post_length: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **validate_post_length_request** | [**ValidatePostLengthRequest**](ValidatePostLengthRequest.md)|  | 

### Return type

[**ValidatePostLength200Response**](ValidatePostLength200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Post length validation result returned. |  -  |
**401** | Authentication failed. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Post length validation failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

