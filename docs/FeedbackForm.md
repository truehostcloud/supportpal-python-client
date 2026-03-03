# FeedbackForm


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**email_template_id** | **int** |  | [optional] 
**condition_group_type** | **int** |  | [optional] 
**expiry_time** | **int** |  | [optional] 
**time_after_resolved** | **int** |  | [optional] 
**fields** | **List[object]** |  | [optional] 
**translations** | **List[object]** |  | [optional] 
**created_at** | **int** |  | [optional] 
**updated_at** | **int** |  | [optional] 

## Example

```python
from supportpal_api_client.models.feedback_form import FeedbackForm

# TODO update the JSON string below
json = "{}"
# create an instance of FeedbackForm from a JSON string
feedback_form_instance = FeedbackForm.from_json(json)
# print the JSON string representation of the object
print(FeedbackForm.to_json())

# convert the object into a dict
feedback_form_dict = feedback_form_instance.to_dict()
# create an instance of FeedbackForm from a dict
feedback_form_from_dict = FeedbackForm.from_dict(feedback_form_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


