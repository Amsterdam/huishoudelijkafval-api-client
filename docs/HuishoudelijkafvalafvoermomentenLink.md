# HuishoudelijkafvalafvoermomentenLink

The identifier of the relationship to afvoermomenten.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**id** | **str** | Unieke aanduiding van het record. Combinatie verwerker en bon nummer | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalafvoermomenten_link import HuishoudelijkafvalafvoermomentenLink

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalafvoermomentenLink from a JSON string
huishoudelijkafvalafvoermomenten_link_instance = HuishoudelijkafvalafvoermomentenLink.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalafvoermomentenLink.to_json())

# convert the object into a dict
huishoudelijkafvalafvoermomenten_link_dict = huishoudelijkafvalafvoermomenten_link_instance.to_dict()
# create an instance of HuishoudelijkafvalafvoermomentenLink from a dict
huishoudelijkafvalafvoermomenten_link_from_dict = HuishoudelijkafvalafvoermomentenLink.from_dict(huishoudelijkafvalafvoermomenten_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


