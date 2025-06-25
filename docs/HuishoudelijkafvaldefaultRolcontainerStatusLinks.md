# HuishoudelijkafvaldefaultRolcontainerStatusLinks

The contents of the `rolcontainerStatus._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalrolcontainerStatusLink**](HuishoudelijkafvalrolcontainerStatusLink.md) |  | 
**rolcontainer** | [**HuishoudelijkafvalrolcontainerLink**](HuishoudelijkafvalrolcontainerLink.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_rolcontainer_status_links import HuishoudelijkafvaldefaultRolcontainerStatusLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultRolcontainerStatusLinks from a JSON string
huishoudelijkafvaldefault_rolcontainer_status_links_instance = HuishoudelijkafvaldefaultRolcontainerStatusLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultRolcontainerStatusLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_rolcontainer_status_links_dict = huishoudelijkafvaldefault_rolcontainer_status_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultRolcontainerStatusLinks from a dict
huishoudelijkafvaldefault_rolcontainer_status_links_from_dict = HuishoudelijkafvaldefaultRolcontainerStatusLinks.from_dict(huishoudelijkafvaldefault_rolcontainer_status_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


