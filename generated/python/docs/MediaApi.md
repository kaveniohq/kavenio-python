# kavenio.MediaApi

All URIs are relative to *https://api.kavenio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_media_presign**](MediaApi.md#create_media_presign) | **POST** /v1/media/presign | Create a media presign URL
[**upload_media_batch**](MediaApi.md#upload_media_batch) | **POST** /v1/media/upload | Upload media
[**validate_media**](MediaApi.md#validate_media) | **POST** /v1/tools/validate/media | Validate media


# **create_media_presign**
> CreateMediaPresign200Response create_media_presign(create_media_presign_request)

Create a media presign URL

Creates a short-lived upload URL and public media URL for direct upload workflows.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.create_media_presign200_response import CreateMediaPresign200Response
from kavenio.models.create_media_presign_request import CreateMediaPresignRequest
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
    api_instance = kavenio.MediaApi(api_client)
    create_media_presign_request = {"filename":"campaign-video.mp4","contentType":"video/mp4","size":10485760} # CreateMediaPresignRequest | 

    try:
        # Create a media presign URL
        api_response = await api_instance.create_media_presign(create_media_presign_request)
        print("The response of MediaApi->create_media_presign:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MediaApi->create_media_presign: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_media_presign_request** | [**CreateMediaPresignRequest**](CreateMediaPresignRequest.md)|  | 

### Return type

[**CreateMediaPresign200Response**](CreateMediaPresign200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Presign URL created. |  -  |
**401** | Authentication failed. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Media presign failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **upload_media_batch**
> UploadMediaBatch200Response upload_media_batch(upload_media_batch_request)

Upload media

Uploads one or more base64-encoded media items and returns public URLs.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.upload_media_batch200_response import UploadMediaBatch200Response
from kavenio.models.upload_media_batch_request import UploadMediaBatchRequest
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
    api_instance = kavenio.MediaApi(api_client)
    upload_media_batch_request = {"items":[{"fileName":"campaign-image.png","contentType":"image/png","base64Data":"iVBORw0KGgoAAAANSUhEUgAAAAEAAAAB..."}]} # UploadMediaBatchRequest | 

    try:
        # Upload media
        api_response = await api_instance.upload_media_batch(upload_media_batch_request)
        print("The response of MediaApi->upload_media_batch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MediaApi->upload_media_batch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **upload_media_batch_request** | [**UploadMediaBatchRequest**](UploadMediaBatchRequest.md)|  | 

### Return type

[**UploadMediaBatch200Response**](UploadMediaBatch200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Media uploaded. |  -  |
**401** | Authentication failed. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Media upload failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validate_media**
> ValidateMedia200Response validate_media(validate_media_request)

Validate media

Validates a public media URL and returns content type, size, type, and platform limit information when available.

### Example

* Bearer (Clerk session or OAuth token) Authentication (bearerAuth):

```python
import kavenio
from kavenio.models.validate_media200_response import ValidateMedia200Response
from kavenio.models.validate_media_request import ValidateMediaRequest
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
    api_instance = kavenio.MediaApi(api_client)
    validate_media_request = {"url":"https://cdn.example.com/campaign-image.png"} # ValidateMediaRequest | 

    try:
        # Validate media
        api_response = await api_instance.validate_media(validate_media_request)
        print("The response of MediaApi->validate_media:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MediaApi->validate_media: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **validate_media_request** | [**ValidateMediaRequest**](ValidateMediaRequest.md)|  | 

### Return type

[**ValidateMedia200Response**](ValidateMedia200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Media validation result returned. |  -  |
**401** | Authentication failed. |  -  |
**422** | Request body validation failed. |  -  |
**500** | Media validation failed. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

