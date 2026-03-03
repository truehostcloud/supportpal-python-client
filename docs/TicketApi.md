# supportpal_api_client.TicketApi

All URIs are relative to *https://yourdomain.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_ticket**](TicketApi.md#get_ticket) | **GET** /ticket/ticket/{id} | Get ticket by ID
[**list_tickets**](TicketApi.md#list_tickets) | **GET** /ticket/ticket | List tickets


# **get_ticket**
> TicketResponse get_ticket(id)

Get ticket by ID

### Example

* Basic Authentication (BasicAuth):

```python
import supportpal_api_client
from supportpal_api_client.models.ticket_response import TicketResponse
from supportpal_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://yourdomain.com/api
# See configuration.py for a list of all supported configuration parameters.
configuration = supportpal_api_client.Configuration(
    host = "https://yourdomain.com/api"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: BasicAuth
configuration = supportpal_api_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with supportpal_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = supportpal_api_client.TicketApi(api_client)
    id = 56 # int | 

    try:
        # Get ticket by ID
        api_response = api_instance.get_ticket(id)
        print("The response of TicketApi->get_ticket:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TicketApi->get_ticket: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**TicketResponse**](TicketResponse.md)

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

# **list_tickets**
> TicketListResponse list_tickets(department=department, status=status, assigned=assigned, start=start, limit=limit, order_column=order_column, order_direction=order_direction, created_at_min=created_at_min, created_at_max=created_at_max, updated_at_min=updated_at_min, updated_at_max=updated_at_max)

List tickets

### Example

* Basic Authentication (BasicAuth):

```python
import supportpal_api_client
from supportpal_api_client.models.ticket_list_response import TicketListResponse
from supportpal_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://yourdomain.com/api
# See configuration.py for a list of all supported configuration parameters.
configuration = supportpal_api_client.Configuration(
    host = "https://yourdomain.com/api"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: BasicAuth
configuration = supportpal_api_client.Configuration(
    username = os.environ["USERNAME"],
    password = os.environ["PASSWORD"]
)

# Enter a context with an instance of the API client
with supportpal_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = supportpal_api_client.TicketApi(api_client)
    department = 'department_example' # str | Filter by department ID(s), comma delimited e.g. 1,2,3 (optional)
    status = 'status_example' # str | Filter by status ID(s), comma delimited e.g. 1,2,3 (optional)
    assigned = 'assigned_example' # str | Filter by assigned operator ID(s), use -1 for unassigned tickets (optional)
    start = 1 # int | The first result offset (1-indexed) (optional) (default to 1)
    limit = 50 # int | The number of results to fetch per page (optional) (default to 50)
    order_column = 'id' # str |  (optional) (default to 'id')
    order_direction = asc # str |  (optional) (default to asc)
    created_at_min = 56 # int | Filter tickets created since this UNIX timestamp (optional)
    created_at_max = 56 # int | Filter tickets created before this UNIX timestamp (optional)
    updated_at_min = 56 # int | Filter tickets updated since this UNIX timestamp (optional)
    updated_at_max = 56 # int | Filter tickets updated before this UNIX timestamp (optional)

    try:
        # List tickets
        api_response = api_instance.list_tickets(department=department, status=status, assigned=assigned, start=start, limit=limit, order_column=order_column, order_direction=order_direction, created_at_min=created_at_min, created_at_max=created_at_max, updated_at_min=updated_at_min, updated_at_max=updated_at_max)
        print("The response of TicketApi->list_tickets:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TicketApi->list_tickets: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **department** | **str**| Filter by department ID(s), comma delimited e.g. 1,2,3 | [optional] 
 **status** | **str**| Filter by status ID(s), comma delimited e.g. 1,2,3 | [optional] 
 **assigned** | **str**| Filter by assigned operator ID(s), use -1 for unassigned tickets | [optional] 
 **start** | **int**| The first result offset (1-indexed) | [optional] [default to 1]
 **limit** | **int**| The number of results to fetch per page | [optional] [default to 50]
 **order_column** | **str**|  | [optional] [default to &#39;id&#39;]
 **order_direction** | **str**|  | [optional] [default to asc]
 **created_at_min** | **int**| Filter tickets created since this UNIX timestamp | [optional] 
 **created_at_max** | **int**| Filter tickets created before this UNIX timestamp | [optional] 
 **updated_at_min** | **int**| Filter tickets updated since this UNIX timestamp | [optional] 
 **updated_at_max** | **int**| Filter tickets updated before this UNIX timestamp | [optional] 

### Return type

[**TicketListResponse**](TicketListResponse.md)

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

