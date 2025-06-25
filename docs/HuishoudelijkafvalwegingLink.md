# HuishoudelijkafvalwegingLink

The identifier of the relationship to weging.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**id** | **str** | Uniek identificerend kenmerk weging. Deze is per container vastgelegd | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalweging_link import HuishoudelijkafvalwegingLink

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalwegingLink from a JSON string
huishoudelijkafvalweging_link_instance = HuishoudelijkafvalwegingLink.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalwegingLink.to_json())

# convert the object into a dict
huishoudelijkafvalweging_link_dict = huishoudelijkafvalweging_link_instance.to_dict()
# create an instance of HuishoudelijkafvalwegingLink from a dict
huishoudelijkafvalweging_link_from_dict = HuishoudelijkafvalwegingLink.from_dict(huishoudelijkafvalweging_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


