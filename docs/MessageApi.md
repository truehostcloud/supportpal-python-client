# supportpal_client.MessageApi

All URIs are relative to *https://yourdomain.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_message**](MessageApi.md#get_message) | **GET** /ticket/message/{id} | Get message by ID
[**list_messages**](MessageApi.md#list_messages) | **GET** /ticket/message | List messages for a ticket


# **get_message**
> MessageResponse get_message(id)

Get message by ID

### Example

* Basic Authentication (BasicAuth):

```python
import supportpal_client
from supportpal_client.models.message_response import MessageResponse
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
    api_instance = supportpal_client.MessageApi(api_client)
    id = 56 # int | 

    try:
        # Get message by ID
        api_response = api_instance.get_message(id)
        print("The response of MessageApi->get_message:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageApi->get_message: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**MessageResponse**](MessageResponse.md)

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

# **list_messages**
> MessageListResponse list_messages(ticket_id, type=type, by=by, include_draft=include_draft, start=start, limit=limit, order_column=order_column, order_direction=order_direction)

List messages for a ticket

### Example

* Basic Authentication (BasicAuth):

```python
import supportpal_client
from supportpal_client.models.message_list_response import MessageListResponse
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
    api_instance = supportpal_client.MessageApi(api_client)
    ticket_id = 56 # int | Ticket ID to fetch messages for
    type = 56 # int | Filter by message type: 0 = message, 1 = internal note (optional)
    by = 56 # int | Filter by author type: 0 = operator, 1 = user (customer) (optional)
    include_draft = 0 # int | Whether to include draft messages (optional) (default to 0)
    start = 1 # int |  (optional) (default to 1)
    limit = 50 # int |  (optional) (default to 50)
    order_column = 'id' # str |  (optional) (default to 'id')
    order_direction = asc # str |  (optional) (default to asc)

    try:
        # List messages for a ticket
        api_response = api_instance.list_messages(ticket_id, type=type, by=by, include_draft=include_draft, start=start, limit=limit, order_column=order_column, order_direction=order_direction)
        print("The response of MessageApi->list_messages:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MessageApi->list_messages: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticket_id** | **int**| Ticket ID to fetch messages for | 
 **type** | **int**| Filter by message type: 0 &#x3D; message, 1 &#x3D; internal note | [optional] 
 **by** | **int**| Filter by author type: 0 &#x3D; operator, 1 &#x3D; user (customer) | [optional] 
 **include_draft** | **int**| Whether to include draft messages | [optional] [default to 0]
 **start** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 50]
 **order_column** | **str**|  | [optional] [default to &#39;id&#39;]
 **order_direction** | **str**|  | [optional] [default to asc]

### Return type

[**MessageListResponse**](MessageListResponse.md)

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

