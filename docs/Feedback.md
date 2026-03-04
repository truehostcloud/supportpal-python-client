# Feedback


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**ticket_id** | **int** |  | [optional] 
**form_id** | **int** |  | [optional] 
**rating** | **int** | Customer satisfaction rating: null &#x3D; not yet responded, 0 &#x3D; bad, 1 &#x3D; good, 2 &#x3D; neutral | [optional] 
**fields_answered** | **int** |  | [optional] 
**token** | **str** |  | [optional] 
**expiry_time** | **int** |  | [optional] 
**values** | **List[object]** |  | [optional] 
**form** | [**FeedbackForm**](FeedbackForm.md) |  | [optional] 
**created_at** | **int** |  | [optional] 
**updated_at** | **int** |  | [optional] 

## Example

```python
from supportpal_client.models.feedback import Feedback

# TODO update the JSON string below
json = "{}"
# create an instance of Feedback from a JSON string
feedback_instance = Feedback.from_json(json)
# print the JSON string representation of the object
print(Feedback.to_json())

# convert the object into a dict
feedback_dict = feedback_instance.to_dict()
# create an instance of Feedback from a dict
feedback_from_dict = Feedback.from_dict(feedback_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


