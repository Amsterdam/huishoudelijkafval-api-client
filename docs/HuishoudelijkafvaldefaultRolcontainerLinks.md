# HuishoudelijkafvaldefaultRolcontainerLinks

The contents of the `rolcontainer._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalrolcontainerLink**](HuishoudelijkafvalrolcontainerLink.md) |  | 
**bag_woonplaats** | [**BagWoonplaatsenRawIdentifier**](BagWoonplaatsenRawIdentifier.md) |  | 
**bag_openbareruimte** | [**BagOpenbareruimtesRawIdentifier**](BagOpenbareruimtesRawIdentifier.md) |  | 
**bag_verblijfsobject** | [**BagVerblijfsobjectenRawIdentifier**](BagVerblijfsobjectenRawIdentifier.md) |  | 
**bag_nummeraanduiding** | [**BagNummeraanduidingenRawIdentifier**](BagNummeraanduidingenRawIdentifier.md) |  | 
**gebied_buurt** | [**GebiedenBuurtenRawIdentifier**](GebiedenBuurtenRawIdentifier.md) |  | 
**gebied_wijk** | [**GebiedenWijkenRawIdentifier**](GebiedenWijkenRawIdentifier.md) |  | 
**gebied_stadsdeel** | [**GebiedenStadsdelenRawIdentifier**](GebiedenStadsdelenRawIdentifier.md) |  | 
**gebied_ggw** | [**GebiedenGgwgebiedenRawIdentifier**](GebiedenGgwgebiedenRawIdentifier.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_rolcontainer_links import HuishoudelijkafvaldefaultRolcontainerLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultRolcontainerLinks from a JSON string
huishoudelijkafvaldefault_rolcontainer_links_instance = HuishoudelijkafvaldefaultRolcontainerLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultRolcontainerLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_rolcontainer_links_dict = huishoudelijkafvaldefault_rolcontainer_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultRolcontainerLinks from a dict
huishoudelijkafvaldefault_rolcontainer_links_from_dict = HuishoudelijkafvaldefaultRolcontainerLinks.from_dict(huishoudelijkafvaldefault_rolcontainer_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


