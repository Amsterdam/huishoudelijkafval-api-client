# HuishoudelijkafvaldefaultBijplaatsingenLinks

The contents of the `bijplaatsingen._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalbijplaatsingenLink**](HuishoudelijkafvalbijplaatsingenLink.md) |  | 
**cluster** | [**HuishoudelijkafvalclusterLink**](HuishoudelijkafvalclusterLink.md) |  | 
**gbd_buurt** | [**GebiedenBuurtenRawIdentifier**](GebiedenBuurtenRawIdentifier.md) |  | 
**bag_openbareruimte** | [**BagOpenbareruimtesRawIdentifier**](BagOpenbareruimtesRawIdentifier.md) |  | 
**bag_verblijfsobject** | [**BagVerblijfsobjectenRawIdentifier**](BagVerblijfsobjectenRawIdentifier.md) |  | 
**bag_nummeraanduiding** | [**BagNummeraanduidingenRawIdentifier**](BagNummeraanduidingenRawIdentifier.md) |  | 
**bag_woonplaats** | [**BagWoonplaatsenRawIdentifier**](BagWoonplaatsenRawIdentifier.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_bijplaatsingen_links import HuishoudelijkafvaldefaultBijplaatsingenLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultBijplaatsingenLinks from a JSON string
huishoudelijkafvaldefault_bijplaatsingen_links_instance = HuishoudelijkafvaldefaultBijplaatsingenLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultBijplaatsingenLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_bijplaatsingen_links_dict = huishoudelijkafvaldefault_bijplaatsingen_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultBijplaatsingenLinks from a dict
huishoudelijkafvaldefault_bijplaatsingen_links_from_dict = HuishoudelijkafvaldefaultBijplaatsingenLinks.from_dict(huishoudelijkafvaldefault_bijplaatsingen_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


