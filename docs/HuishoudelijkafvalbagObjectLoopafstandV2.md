# HuishoudelijkafvalbagObjectLoopafstandV2

bagObjectLoopafstandV2

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links**](HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links.md) |  | 
**id** | **str** | Uniek identificerend kenmerk van het record | 
**bag_object_id** | **str** | Uniek identificerend kenmerk van bagobject | [optional] 
**bag_object_type** | **str** | Typering adresseerbaar object conform BAG: verblijfsobject, ligplaats , standplaats | [optional] 
**cluster_id** | **str** | Uniek identificerend kenmerk van cluster waarnaar de afstand is berekend | [readonly] 
**fractie** | **str** | Code afvalfractie waarnaar de afstand is bepaald | [optional] 
**fractie_omschrijving** | **str** | Omschrijving afvalfractie waarnaar de afstand is bepaald | [optional] 
**loopafstand_categorie_id** | **str** | Relatie naar de categorie waarin de berekende loopafstand valt | [readonly] 
**loopafstand** | **float** | Berekende afstand over de weg in meter  van woning tot cluster van containers van de betreffende afvalfractie | [optional] 
**geometrie** | [**Polygon**](Polygon.md) |  | [optional] 
**wijzigingsdatum_dp** | **datetime** | Datum waarop het object is gewijzigd | [optional] 
**verwijderd_dp** | **bool** | Indicatie of het object verwijderd is in de datapijplijn | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalbag_object_loopafstand_v2 import HuishoudelijkafvalbagObjectLoopafstandV2

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalbagObjectLoopafstandV2 from a JSON string
huishoudelijkafvalbag_object_loopafstand_v2_instance = HuishoudelijkafvalbagObjectLoopafstandV2.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalbagObjectLoopafstandV2.to_json())

# convert the object into a dict
huishoudelijkafvalbag_object_loopafstand_v2_dict = huishoudelijkafvalbag_object_loopafstand_v2_instance.to_dict()
# create an instance of HuishoudelijkafvalbagObjectLoopafstandV2 from a dict
huishoudelijkafvalbag_object_loopafstand_v2_from_dict = HuishoudelijkafvalbagObjectLoopafstandV2.from_dict(huishoudelijkafvalbag_object_loopafstand_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


