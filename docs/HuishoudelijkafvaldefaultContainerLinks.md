# HuishoudelijkafvaldefaultContainerLinks

The contents of the `container._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalcontainerLink**](HuishoudelijkafvalcontainerLink.md) |  | 
**cluster** | [**HuishoudelijkafvalclusterLink**](HuishoudelijkafvalclusterLink.md) |  | 
**locatie** | [**HuishoudelijkafvalcontainerlocatieLink**](HuishoudelijkafvalcontainerlocatieLink.md) |  | 
**type** | [**HuishoudelijkafvalcontainertypeLink**](HuishoudelijkafvalcontainertypeLink.md) |  | 
**bag_hoofdadres_verblijfsobject** | [**BagVerblijfsobjectenRawIdentifier**](BagVerblijfsobjectenRawIdentifier.md) |  | 
**gbd_buurt** | [**GebiedenBuurtenRawIdentifier**](GebiedenBuurtenRawIdentifier.md) |  | 
**bag_openbareruimte** | [**BagOpenbareruimtesRawIdentifier**](BagOpenbareruimtesRawIdentifier.md) |  | 
**bag_nummeraanduiding** | [**BagNummeraanduidingenRawIdentifier**](BagNummeraanduidingenRawIdentifier.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_container_links import HuishoudelijkafvaldefaultContainerLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultContainerLinks from a JSON string
huishoudelijkafvaldefault_container_links_instance = HuishoudelijkafvaldefaultContainerLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultContainerLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_container_links_dict = huishoudelijkafvaldefault_container_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultContainerLinks from a dict
huishoudelijkafvaldefault_container_links_from_dict = HuishoudelijkafvaldefaultContainerLinks.from_dict(huishoudelijkafvaldefault_container_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


