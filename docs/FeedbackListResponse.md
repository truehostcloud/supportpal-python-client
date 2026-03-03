# FeedbackListResponse

Both the list and single-resource feedback endpoints return an array in data.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**count** | **int** | Total number of records matching the query | [optional] 
**data** | [**List[Feedback]**](Feedback.md) |  | [optional] 

## Example

```python
from supportpal_api_client.models.feedback_list_response import FeedbackListResponse

# TODO update the JSON string below
json = "{}"
# create an instance of FeedbackListResponse from a JSON string
feedback_list_response_instance = FeedbackListResponse.from_json(json)
# print the JSON string representation of the object
print(FeedbackListResponse.to_json())

# convert the object into a dict
feedback_list_response_dict = feedback_list_response_instance.to_dict()
# create an instance of FeedbackListResponse from a dict
feedback_list_response_from_dict = FeedbackListResponse.from_dict(feedback_list_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


