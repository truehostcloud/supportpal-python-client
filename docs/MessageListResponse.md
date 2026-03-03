# MessageListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**count** | **int** | Total number of records matching the query | [optional] 
**data** | [**List[Message]**](Message.md) |  | [optional] 

## Example

```python
from supportpal_api_client.models.message_list_response import MessageListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of MessageListResponse from a JSON string
message_list_response_instance = MessageListResponse.from_json(json)
# print the JSON string representation of the object
print(MessageListResponse.to_json())

# convert the object into a dict
message_list_response_dict = message_list_response_instance.to_dict()
# create an instance of MessageListResponse from a dict
message_list_response_from_dict = MessageListResponse.from_dict(message_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


