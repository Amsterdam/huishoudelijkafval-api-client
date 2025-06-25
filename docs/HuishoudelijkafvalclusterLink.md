# HuishoudelijkafvalclusterLink

The identifier of the relationship to cluster.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**id** | **str** | Uniek identificerend kenmerk van cluster | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalcluster_link import HuishoudelijkafvalclusterLink

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalclusterLink from a JSON string
huishoudelijkafvalcluster_link_instance = HuishoudelijkafvalclusterLink.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalclusterLink.to_json())

# convert the object into a dict
huishoudelijkafvalcluster_link_dict = huishoudelijkafvalcluster_link_instance.to_dict()
# create an instance of HuishoudelijkafvalclusterLink from a dict
huishoudelijkafvalcluster_link_from_dict = HuishoudelijkafvalclusterLink.from_dict(huishoudelijkafvalcluster_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


