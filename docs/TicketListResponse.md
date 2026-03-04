# TicketListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**count** | **int** | Total number of records matching the query | [optional] 
**data** | [**List[Ticket]**](Ticket.md) |  | [optional] 

## Example

```python
from supportpal_client.models.ticket_list_response import TicketListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of TicketListResponse from a JSON string
ticket_list_response_instance = TicketListResponse.from_json(json)
# print the JSON string representation of the object
print(TicketListResponse.to_json())

# convert the object into a dict
ticket_list_response_dict = ticket_list_response_instance.to_dict()
# create an instance of TicketListResponse from a dict
ticket_list_response_from_dict = TicketListResponse.from_dict(ticket_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


