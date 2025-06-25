# HuishoudelijkafvalcontainerLink

The identifier of the relationship to container.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**id** | **str** | Unieke aanduiding objecttype | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalcontainer_link import HuishoudelijkafvalcontainerLink

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalcontainerLink from a JSON string
huishoudelijkafvalcontainer_link_instance = HuishoudelijkafvalcontainerLink.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalcontainerLink.to_json())

# convert the object into a dict
huishoudelijkafvalcontainer_link_dict = huishoudelijkafvalcontainer_link_instance.to_dict()
# create an instance of HuishoudelijkafvalcontainerLink from a dict
huishoudelijkafvalcontainer_link_from_dict = HuishoudelijkafvalcontainerLink.from_dict(huishoudelijkafvalcontainer_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


