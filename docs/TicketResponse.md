# TicketResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**data** | [**Ticket**](Ticket.md) |  | [optional] 

## Example

```python
from supportpal_api_client.models.ticket_response import TicketResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TicketResponse from a JSON string
ticket_response_instance = TicketResponse.from_json(json)
# print the JSON string representation of the object
print(TicketResponse.to_json())

# convert the object into a dict
ticket_response_dict = ticket_response_instance.to_dict()
# create an instance of TicketResponse from a dict
ticket_response_from_dict = TicketResponse.from_dict(ticket_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


