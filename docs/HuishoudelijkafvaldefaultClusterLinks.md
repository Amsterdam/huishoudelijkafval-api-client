# HuishoudelijkafvaldefaultClusterLinks

The contents of the `cluster._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalclusterLink**](HuishoudelijkafvalclusterLink.md) |  | 
**bag_hoofdadres_verblijfsobject** | [**BagVerblijfsobjectenRawIdentifier**](BagVerblijfsobjectenRawIdentifier.md) |  | 
**gbd_buurt** | [**GebiedenBuurtenRawIdentifier**](GebiedenBuurtenRawIdentifier.md) |  | 
**bag_openbareruimte** | [**BagOpenbareruimtesRawIdentifier**](BagOpenbareruimtesRawIdentifier.md) |  | 
**bag_nummeraanduiding** | [**BagNummeraanduidingenRawIdentifier**](BagNummeraanduidingenRawIdentifier.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_cluster_links import HuishoudelijkafvaldefaultClusterLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultClusterLinks from a JSON string
huishoudelijkafvaldefault_cluster_links_instance = HuishoudelijkafvaldefaultClusterLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultClusterLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_cluster_links_dict = huishoudelijkafvaldefault_cluster_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultClusterLinks from a dict
huishoudelijkafvaldefault_cluster_links_from_dict = HuishoudelijkafvaldefaultClusterLinks.from_dict(huishoudelijkafvaldefault_cluster_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


