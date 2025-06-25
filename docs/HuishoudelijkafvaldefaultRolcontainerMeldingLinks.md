# HuishoudelijkafvaldefaultRolcontainerMeldingLinks

The contents of the `rolcontainerMelding._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalrolcontainerMeldingLink**](HuishoudelijkafvalrolcontainerMeldingLink.md) |  | 
**rolcontainer** | [**HuishoudelijkafvalrolcontainerLink**](HuishoudelijkafvalrolcontainerLink.md) |  | 
**bag_verblijfsobject** | [**BagVerblijfsobjectenRawIdentifier**](BagVerblijfsobjectenRawIdentifier.md) |  | 
**bag_nummeraanduiding** | [**BagNummeraanduidingenRawIdentifier**](BagNummeraanduidingenRawIdentifier.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_rolcontainer_melding_links import HuishoudelijkafvaldefaultRolcontainerMeldingLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultRolcontainerMeldingLinks from a JSON string
huishoudelijkafvaldefault_rolcontainer_melding_links_instance = HuishoudelijkafvaldefaultRolcontainerMeldingLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultRolcontainerMeldingLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_rolcontainer_melding_links_dict = huishoudelijkafvaldefault_rolcontainer_melding_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultRolcontainerMeldingLinks from a dict
huishoudelijkafvaldefault_rolcontainer_melding_links_from_dict = HuishoudelijkafvaldefaultRolcontainerMeldingLinks.from_dict(huishoudelijkafvaldefault_rolcontainer_melding_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


