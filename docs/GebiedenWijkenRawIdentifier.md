# GebiedenWijkenRawIdentifier

The identifier of the relationship to wijken.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**identificatie** | **str** |  | 

## Example

```python
from huishoudelijkafval_api_client.models.gebieden_wijken_raw_identifier import GebiedenWijkenRawIdentifier

# TODO update the JSON string below
json = "{}"
# create an instance of GebiedenWijkenRawIdentifier from a JSON string
gebieden_wijken_raw_identifier_instance = GebiedenWijkenRawIdentifier.from_json(json)
# print the JSON string representation of the object
print(GebiedenWijkenRawIdentifier.to_json())

# convert the object into a dict
gebieden_wijken_raw_identifier_dict = gebieden_wijken_raw_identifier_instance.to_dict()
# create an instance of GebiedenWijkenRawIdentifier from a dict
gebieden_wijken_raw_identifier_from_dict = GebiedenWijkenRawIdentifier.from_dict(gebieden_wijken_raw_identifier_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


