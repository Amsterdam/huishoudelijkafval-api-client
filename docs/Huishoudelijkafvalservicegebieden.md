# Huishoudelijkafvalservicegebieden

Een afvalservicegebied is een verzameling van panden die dicht bij elkaar liggen op basis van hun loopafstand tot een afvalophaal locatie. De bewoners van deze panden maken gebruik van het dichtstbijzijnde afvalservicepunt.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultServicegebiedenLinks**](HuishoudelijkafvaldefaultServicegebiedenLinks.md) |  | 
**id** | **str** | Unieke identificatie van een afval servicegebied | 
**bag_object_id** | **str** | Unieke BAG object (pand, ligplaats en standplaats) identificatie | [optional] 
**bag_object_type** | **str** | Type BAG object (pand, ligplaats en standplaats) | [optional] 
**servicegebieden_locatie_id** | **str** | Identificatie van een servicegebied locatie. De Servicegebieden locaties correspenderen met de afvalcluster | [readonly] 
**fractie_code** | **str** | Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood | [optional] 
**fractie_omschrijving** | **str** | Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. | [optional] 
**loopafstand_categorie_id** | **str** | Unieke identificatie van loopafstanden categoriën | [optional] 
**loopafstand_categorie_omschrijving** | **str** | De loopafstanden zijn volgens een vastgestelde indelijng gecategoriseerd. Bijvoorbeeld: 30 - 90 meter | [optional] 
**loopafstand_categorie_vanaf** | **float** | De loopafstand vanaf een bepaalde meter. Volgens de loopafstand categorisatie. | [optional] 
**loopafstand_categorie_tot** | **float** | De loopafstand tot een bepaalde meter volgens de loopafstandcategorisatie. | [optional] 
**categorie_wijzigingsdatum_dp** | **datetime** | De datum waarop de loopafstandcategorie in de datapijplijn is gewijzigd | [optional] 
**categorie_verwijderd_dp** | **bool** | De datum waarop de loopafstandcategorie in de datapijplijn is verwijderd. | [optional] 
**geometrie** | [**Polygon**](Polygon.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalservicegebieden import Huishoudelijkafvalservicegebieden

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalservicegebieden from a JSON string
huishoudelijkafvalservicegebieden_instance = Huishoudelijkafvalservicegebieden.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalservicegebieden.to_json())

# convert the object into a dict
huishoudelijkafvalservicegebieden_dict = huishoudelijkafvalservicegebieden_instance.to_dict()
# create an instance of Huishoudelijkafvalservicegebieden from a dict
huishoudelijkafvalservicegebieden_from_dict = Huishoudelijkafvalservicegebieden.from_dict(huishoudelijkafvalservicegebieden_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


