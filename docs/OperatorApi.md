# supportpal_api_client.OperatorApi

All URIs are relative to *https://yourdomain.com/api*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_operator**](OperatorApi.md#get_operator) | **GET** /user/operator/{id} | Get operator by ID
[**list_operators**](OperatorApi.md#list_operators) | **GET** /user/operator | List operators


# **get_operator**
> OperatorResponse get_operator(id)

Get operator by ID

### Example

* Basic Authentication (BasicAuth):

```python
import supportpal_api_client
from supportpal_api_client.models.operator_response import OperatorResponse
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
    api_instance = supportpal_api_client.OperatorApi(api_client)
    id = 56 # int | 

    try:
        # Get operator by ID
        api_response = api_instance.get_operator(id)
        print("The response of OperatorApi->get_operator:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OperatorApi->get_operator: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**OperatorResponse**](OperatorResponse.md)

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

# **list_operators**
> OperatorListResponse list_operators(active=active, email=email, start=start, limit=limit)

List operators

### Example

* Basic Authentication (BasicAuth):

```python
import supportpal_api_client
from supportpal_api_client.models.operator_list_response import OperatorListResponse
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
    api_instance = supportpal_api_client.OperatorApi(api_client)
    active = 56 # int | Filter by active status: 1 = active, 0 = inactive (optional)
    email = 'email_example' # str | Search for operators by email (optional)
    start = 1 # int |  (optional) (default to 1)
    limit = 50 # int |  (optional) (default to 50)

    try:
        # List operators
        api_response = api_instance.list_operators(active=active, email=email, start=start, limit=limit)
        print("The response of OperatorApi->list_operators:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OperatorApi->list_operators: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **active** | **int**| Filter by active status: 1 &#x3D; active, 0 &#x3D; inactive | [optional] 
 **email** | **str**| Search for operators by email | [optional] 
 **start** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 50]

### Return type

[**OperatorListResponse**](OperatorListResponse.md)

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

