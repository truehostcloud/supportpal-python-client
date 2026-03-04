# Ticket


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**number** | **str** |  | [optional] 
**department_id** | **int** |  | [optional] 
**department_email_id** | **int** |  | [optional] 
**brand_id** | **int** |  | [optional] 
**channel_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**status_id** | **int** |  | [optional] 
**priority_id** | **int** |  | [optional] 
**sla_plan_id** | **int** |  | [optional] 
**subject** | **str** |  | [optional] 
**due_time** | **int** |  | [optional] 
**resolved_time** | **int** |  | [optional] 
**cc** | **List[str]** |  | [optional] 
**locked** | **int** |  | [optional] 
**merged** | **int** |  | [optional] 
**internal** | **int** |  | [optional] 
**created_at** | **int** |  | [optional] 
**updated_at** | **int** |  | [optional] 
**deleted_at** | **int** |  | [optional] 
**frontend_url** | **str** |  | [optional] 
**operator_url** | **str** |  | [optional] 
**token** | **str** |  | [optional] 
**department** | [**Department**](Department.md) |  | [optional] 
**channel** | [**Channel**](Channel.md) |  | [optional] 
**user** | [**UserSummary**](UserSummary.md) |  | [optional] 
**status** | [**TicketStatus**](TicketStatus.md) |  | [optional] 
**priority** | [**Priority**](Priority.md) |  | [optional] 
**slaplan** | **object** |  | [optional] 

## Example

```python
from supportpal_client.models.ticket import Ticket

# TODO update the JSON string below
json = "{}"
# create an instance of Ticket from a JSON string
ticket_instance = Ticket.from_json(json)
# print the JSON string representation of the object
print(Ticket.to_json())

# convert the object into a dict
ticket_dict = ticket_instance.to_dict()
# create an instance of Ticket from a dict
ticket_from_dict = Ticket.from_dict(ticket_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


