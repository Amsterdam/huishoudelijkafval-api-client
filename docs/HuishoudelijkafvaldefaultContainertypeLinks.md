# HuishoudelijkafvaldefaultContainertypeLinks

The contents of the `containertype._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalcontainertypeLink**](HuishoudelijkafvalcontainertypeLink.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_containertype_links import HuishoudelijkafvaldefaultContainertypeLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultContainertypeLinks from a JSON string
huishoudelijkafvaldefault_containertype_links_instance = HuishoudelijkafvaldefaultContainertypeLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultContainertypeLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_containertype_links_dict = huishoudelijkafvaldefault_containertype_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultContainertypeLinks from a dict
huishoudelijkafvaldefault_containertype_links_from_dict = HuishoudelijkafvaldefaultContainertypeLinks.from_dict(huishoudelijkafvaldefault_containertype_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


