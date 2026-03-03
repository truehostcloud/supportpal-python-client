# Operator


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**firstname** | **str** |  | [optional] 
**lastname** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**email_verified** | **int** |  | [optional] 
**active** | **int** |  | [optional] 
**organisation_id** | **int** |  | [optional] 
**organisation_access_level** | **int** |  | [optional] 
**country** | **str** |  | [optional] 
**language_code** | **str** |  | [optional] 
**timezone** | **str** |  | [optional] 
**avatar** | **str** |  | [optional] 
**created_at** | **int** |  | [optional] 
**updated_at** | **int** |  | [optional] 
**formatted_name** | **str** |  | [optional] 
**phonenumbers** | **List[object]** |  | [optional] 
**groups** | **List[object]** |  | [optional] 

## Example

```python
from supportpal_api_client.models.operator import Operator

# TODO update the JSON string below
json = "{}"
# create an instance of Operator from a JSON string
operator_instance = Operator.from_json(json)
# print the JSON string representation of the object
print(Operator.to_json())

# convert the object into a dict
operator_dict = operator_instance.to_dict()
# create an instance of Operator from a dict
operator_from_dict = Operator.from_dict(operator_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


