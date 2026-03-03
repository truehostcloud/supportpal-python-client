# UserSummary

A user (customer) account embedded in ticket and message responses

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**firstname** | **str** |  | [optional] 
**lastname** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**email_verified** | **int** |  | [optional] 
**organisation_id** | **int** |  | [optional] 
**organisation_access_level** | **int** |  | [optional] 
**country** | **str** |  | [optional] 
**language_code** | **str** |  | [optional] 
**timezone** | **str** |  | [optional] 
**avatar** | **str** |  | [optional] 
**created_at** | **int** |  | [optional] 
**updated_at** | **int** |  | [optional] 
**formatted_name** | **str** |  | [optional] 

## Example

```python
from supportpal_api_client.models.user_summary import UserSummary

# TODO update the JSON string below
json = "{}"
# create an instance of UserSummary from a JSON string
user_summary_instance = UserSummary.from_json(json)
# print the JSON string representation of the object
print(UserSummary.to_json())

# convert the object into a dict
user_summary_dict = user_summary_instance.to_dict()
# create an instance of UserSummary from a dict
user_summary_from_dict = UserSummary.from_dict(user_summary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


