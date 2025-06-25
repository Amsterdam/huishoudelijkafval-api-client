# HuishoudelijkafvaladresLoopafstandV2

adresLoopafstandV2

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultAdresLoopafstandV2Links**](HuishoudelijkafvaldefaultAdresLoopafstandV2Links.md) |  | 
**id** | **str** | Uniek identificerend kenmerk van het record | 
**adresseerbaarobject_id** | **str** | Uniek identificerend kenmerk van adresseerbaarobject | [optional] 
**adresseerbaarobject_type** | **str** | Typering adresseerbaar object conform BAG: verblijfsobject, ligplaats , standplaats | [optional] 
**nummeraanduiding_id** | **str** | BAG:Landelijke identificatie nummeraanduiding | [optional] 
**gebruiksdoel** | **str** | BAG:Een categorisering van de gebruiksdoelen van het betreffende verblijfsobject, ligplaats en standplaatsen zoals dit door de overheid als zodanig is toegestaan | [optional] 
**cluster_id** | **str** | Uniek identificerend kenmerk van cluster waarnaar de afstand is berekend | [readonly] 
**fractie** | **str** | Code afvalfractie waarnaar de afstand is bepaald | [optional] 
**fractie_omschrijving** | **str** | Omschrijving afvalfractie waarnaar de afstand is bepaald | [optional] 
**loopafstand_categorie_id** | **str** | Relatie naar de categorie waarin de berekende loopafstand valt | [readonly] 
**loopafstand** | **float** | Berekende afstand over de weg in meter  van woning tot cluster van containers van de betreffende afvalfractie | [optional] 
**geometrie** | [**Point**](Point.md) |  | [optional] 
**wijzigingsdatum_dp** | **datetime** | Datum waarop het object is gewijzigd | [optional] 
**verwijderd_dp** | **bool** | Indicatie of het object verwijderd is in de datapijplijn | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaladres_loopafstand_v2 import HuishoudelijkafvaladresLoopafstandV2

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaladresLoopafstandV2 from a JSON string
huishoudelijkafvaladres_loopafstand_v2_instance = HuishoudelijkafvaladresLoopafstandV2.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaladresLoopafstandV2.to_json())

# convert the object into a dict
huishoudelijkafvaladres_loopafstand_v2_dict = huishoudelijkafvaladres_loopafstand_v2_instance.to_dict()
# create an instance of HuishoudelijkafvaladresLoopafstandV2 from a dict
huishoudelijkafvaladres_loopafstand_v2_from_dict = HuishoudelijkafvaladresLoopafstandV2.from_dict(huishoudelijkafvaladres_loopafstand_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


