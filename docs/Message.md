# Message


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**ticket_id** | **int** |  | [optional] 
**channel_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**user_ip_address** | **str** |  | [optional] 
**by** | **int** | Author type: 0 &#x3D; operator, 1 &#x3D; user (customer) | [optional] 
**type** | **int** | Message type: 0 &#x3D; message, 1 &#x3D; internal note | [optional] 
**text** | **str** |  | [optional] 
**is_draft** | **int** |  | [optional] 
**social_id** | **str** |  | [optional] 
**created_at** | **int** |  | [optional] 
**updated_at** | **int** |  | [optional] 
**user** | [**UserSummary**](UserSummary.md) |  | [optional] 

## Example

```python
from supportpal_client.models.message import Message

# TODO update the JSON string below
json = "{}"
# create an instance of Message from a JSON string
message_instance = Message.from_json(json)
# print the JSON string representation of the object
print(Message.to_json())

# convert the object into a dict
message_dict = message_instance.to_dict()
# create an instance of Message from a dict
message_from_dict = Message.from_dict(message_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


