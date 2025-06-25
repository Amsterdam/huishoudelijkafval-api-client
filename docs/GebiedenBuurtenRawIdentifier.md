# GebiedenBuurtenRawIdentifier

The identifier of the relationship to buurten.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**identificatie** | **str** |  | 

## Example

```python
from huishoudelijkafval_api_client.models.gebieden_buurten_raw_identifier import GebiedenBuurtenRawIdentifier

# TODO update the JSON string below
json = "{}"
# create an instance of GebiedenBuurtenRawIdentifier from a JSON string
gebieden_buurten_raw_identifier_instance = GebiedenBuurtenRawIdentifier.from_json(json)
# print the JSON string representation of the object
print(GebiedenBuurtenRawIdentifier.to_json())

# convert the object into a dict
gebieden_buurten_raw_identifier_dict = gebieden_buurten_raw_identifier_instance.to_dict()
# create an instance of GebiedenBuurtenRawIdentifier from a dict
gebieden_buurten_raw_identifier_from_dict = GebiedenBuurtenRawIdentifier.from_dict(gebieden_buurten_raw_identifier_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


