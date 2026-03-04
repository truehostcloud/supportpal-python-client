# supportpal_client.FeedbackApi

All URIs are relative to *https://yourdomain.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_feedback**](FeedbackApi.md#get_feedback) | **GET** /ticket/feedback/{id} | Get feedback by ID
[**list_feedback**](FeedbackApi.md#list_feedback) | **GET** /ticket/feedback | List ticket feedback


# **get_feedback**
> FeedbackListResponse get_feedback(id)

Get feedback by ID

### Example

* Basic Authentication (BasicAuth):

```python
import supportpal_client
from supportpal_client.models.feedback_list_response import FeedbackListResponse
from supportpal_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://yourdomain.com/api
# See configuration.py for a list of all supported configuration parameters.
configuration = supportpal_client.Configuration(
    host = "https://yourdomain.com/api"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: BasicAuth
configuration = supportpal_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with supportpal_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = supportpal_client.FeedbackApi(api_client)
    id = 56 # int | 

    try:
        # Get feedback by ID
        api_response = api_instance.get_feedback(id)
        print("The response of FeedbackApi->get_feedback:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FeedbackApi->get_feedback: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**FeedbackListResponse**](FeedbackListResponse.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response. Note: returns an array in data even for a single resource. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_feedback**
> FeedbackListResponse list_feedback(ticket_id=ticket_id, rating=rating, start=start, limit=limit)

List ticket feedback

### Example

* Basic Authentication (BasicAuth):

```python
import supportpal_client
from supportpal_client.models.feedback_list_response import FeedbackListResponse
from supportpal_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://yourdomain.com/api
# See configuration.py for a list of all supported configuration parameters.
configuration = supportpal_client.Configuration(
    host = "https://yourdomain.com/api"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: BasicAuth
configuration = supportpal_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with supportpal_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = supportpal_client.FeedbackApi(api_client)
    ticket_id = 56 # int | Only show feedback for the given ticket ID (optional)
    rating = 56 # int | Filter by rating: 0 = bad, 1 = good, 2 = neutral (optional)
    start = 1 # int |  (optional) (default to 1)
    limit = 50 # int |  (optional) (default to 50)

    try:
        # List ticket feedback
        api_response = api_instance.list_feedback(ticket_id=ticket_id, rating=rating, start=start, limit=limit)
        print("The response of FeedbackApi->list_feedback:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FeedbackApi->list_feedback: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticket_id** | **int**| Only show feedback for the given ticket ID | [optional] 
 **rating** | **int**| Filter by rating: 0 &#x3D; bad, 1 &#x3D; good, 2 &#x3D; neutral | [optional] 
 **start** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 50]

### Return type

[**FeedbackListResponse**](FeedbackListResponse.md)

### Authorization

[BasicAuth](../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

