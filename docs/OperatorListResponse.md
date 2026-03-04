# OperatorListResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**count** | **int** | Total number of records matching the query | [optional] 
**data** | [**List[Operator]**](Operator.md) |  | [optional] 

## Example

```python
from supportpal_client.models.operator_list_response import OperatorListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OperatorListResponse from a JSON string
operator_list_response_instance = OperatorListResponse.from_json(json)
# print the JSON string representation of the object
print(OperatorListResponse.to_json())

# convert the object into a dict
operator_list_response_dict = operator_list_response_instance.to_dict()
# create an instance of OperatorListResponse from a dict
operator_list_response_from_dict = OperatorListResponse.from_dict(operator_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


