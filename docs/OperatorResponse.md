# OperatorResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**data** | [**Operator**](Operator.md) |  | [optional] 

## Example

```python
from supportpal_client.models.operator_response import OperatorResponse

# TODO update the JSON string below
json = "{}"
# create an instance of OperatorResponse from a JSON string
operator_response_instance = OperatorResponse.from_json(json)
# print the JSON string representation of the object
print(OperatorResponse.to_json())

# convert the object into a dict
operator_response_dict = operator_response_instance.to_dict()
# create an instance of OperatorResponse from a dict
operator_response_from_dict = OperatorResponse.from_dict(operator_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


