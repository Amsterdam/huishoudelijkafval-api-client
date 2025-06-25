# Huishoudelijkafvalv1WegingLinks

The contents of the `weging._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalwegingLink**](HuishoudelijkafvalwegingLink.md) |  | 
**bag_hoofdadres_verblijfsobject** | [**BagVerblijfsobjectenRawIdentifier**](BagVerblijfsobjectenRawIdentifier.md) |  | 
**gbd_buurt** | [**GebiedenBuurtenRawIdentifier**](GebiedenBuurtenRawIdentifier.md) |  | 
**bag_openbareruimte** | [**BagOpenbareruimtesRawIdentifier**](BagOpenbareruimtesRawIdentifier.md) |  | 
**bag_nummeraanduiding** | [**BagNummeraanduidingenRawIdentifier**](BagNummeraanduidingenRawIdentifier.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalv1_weging_links import Huishoudelijkafvalv1WegingLinks

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalv1WegingLinks from a JSON string
huishoudelijkafvalv1_weging_links_instance = Huishoudelijkafvalv1WegingLinks.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalv1WegingLinks.to_json())

# convert the object into a dict
huishoudelijkafvalv1_weging_links_dict = huishoudelijkafvalv1_weging_links_instance.to_dict()
# create an instance of Huishoudelijkafvalv1WegingLinks from a dict
huishoudelijkafvalv1_weging_links_from_dict = Huishoudelijkafvalv1WegingLinks.from_dict(huishoudelijkafvalv1_weging_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


