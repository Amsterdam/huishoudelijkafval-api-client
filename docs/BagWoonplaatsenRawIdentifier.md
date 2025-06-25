# BagWoonplaatsenRawIdentifier

The identifier of the relationship to woonplaatsen.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**identificatie** | **str** |  | 

## Example

```python
from huishoudelijkafval_api_client.models.bag_woonplaatsen_raw_identifier import BagWoonplaatsenRawIdentifier

# TODO update the JSON string below
json = "{}"
# create an instance of BagWoonplaatsenRawIdentifier from a JSON string
bag_woonplaatsen_raw_identifier_instance = BagWoonplaatsenRawIdentifier.from_json(json)
# print the JSON string representation of the object
print(BagWoonplaatsenRawIdentifier.to_json())

# convert the object into a dict
bag_woonplaatsen_raw_identifier_dict = bag_woonplaatsen_raw_identifier_instance.to_dict()
# create an instance of BagWoonplaatsenRawIdentifier from a dict
bag_woonplaatsen_raw_identifier_from_dict = BagWoonplaatsenRawIdentifier.from_dict(bag_woonplaatsen_raw_identifier_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


