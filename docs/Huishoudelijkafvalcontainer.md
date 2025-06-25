# Huishoudelijkafvalcontainer

Bevat een overzicht van alle onder- en bovengronds afvalcontainers in Gemeente Amsterdam

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultContainerLinks**](HuishoudelijkafvaldefaultContainerLinks.md) |  | 
**id** | **str** | Unieke aanduiding objecttype | 
**id_nummer** | **str** | Identificatie dat door de fabrikant aan het object is gegeven | [optional] 
**serienummer** | **str** | serienummer uitgegeven door de fabrikant | [optional] 
**cluster_id** | **str** | Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd | [readonly] 
**eigenaar_id** | **str** | Identificerend kenmerk eigenaar | [optional] 
**eigenaar_naam** | **str** | Naam eigenaar | [optional] 
**status** | **int** | Status van de container,0 - inactief, 1 - actief, 2 - gepland | [optional] 
**fractie_code** | **str** | Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood | [optional] 
**fractie_omschrijving** | **str** | Container fractieomschrijving zoals door leverancier is geleverd. | [optional] 
**datum_creatie** | **date** | Datum waarop het object is gecreëerd in container management systeem | [optional] 
**datum_plaatsing** | **date** | Datum waarop het object op de locatie is geplaatst | [optional] 
**datum_operationeel** | **date** | Datum dat de container operationeel is voor het aanbieden van afval | [optional] 
**datum_aflopen_garantie** | **date** | Datum waarop de garantie verloopt | [optional] 
**datum_oplevering** | **date** | Datum waarop het object is geleverd | [optional] 
**wijzigingsdatum_dp** | **datetime** | Datum waarop het object is gewijzigd | [optional] 
**verwijderd_dp** | **bool** | Indicatie of het object verwijderd is bij de bronhouder | [optional] 
**geadopteerd_ind** | **bool** | indicatie of het object door een bewoner geadopteerd is | [optional] 
**locatie_id** | **str** | Identificerend kenmerk van de put waarin de container is geplaatst | [readonly] 
**geometrie** | [**Point**](Point.md) |  | [optional] 
**type_id** | **str** | Identificerend kenmerk van het containertype | [readonly] 
**bag_hoofdadres_verblijfsobject_id** | **str** | Een identificatiecode van een verblijfsobject is een authentiek gegeven en een unieke aanduiding van het verblijfsobject. | [readonly] 
**gbd_buurt_id** | **str** | Unieke identificatie van het object | [readonly] 
**bag_openbareruimte_id** | **str** | Openbare ruimte identificatie | [readonly] 
**bag_nummeraanduiding_id** | **str** | Identificatie nummeraanduiding | [readonly] 
**container_ral_kleur_naam** | **str** | De naam van de ralkleur | [optional] 
**container_ral_kleur_code** | **str** | De internationale ralkleurcode. | [optional] 
**container_ral_kleur_hexcode** | **str** | De hexcode van de ralkleur. | [optional] 
**container_chip_nummber** | **str** | Het identificatienummer van de chip die registreert wanneer de container wordt geleegd. | [optional] 
**container_unit_card_lezer_id** | **str** | Het identificatienummer van de kaartlezer. | [optional] 
**container_kleur** | **str** | De naam van de kleur | [optional] 
**container_mark** | **int** | Definitie volgt nog | [optional] 
**container_datum_vervanging** | **date** | De datum waarop de container wordt vervangen. | [optional] 
**container_datum_wijziging** | **datetime** | Datum waarop de container is gewijzigd. | [optional] 
**container_end_of_life** | **date** | Datum waarop het object het einde van zijn levenscyclus heeft bereikt. | [optional] 
**container_eigenaarschap** | **str** | De soort eigenaarschap van het object. | [optional] 
**container_eigenaarschap_opmerking** | **str** | Beschrijving van  het type eigenaarschap. | [optional] 
**container_opmerking** | **str** | Opmerking over het object door de betrokken medewerker. | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalcontainer import Huishoudelijkafvalcontainer

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalcontainer from a JSON string
huishoudelijkafvalcontainer_instance = Huishoudelijkafvalcontainer.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalcontainer.to_json())

# convert the object into a dict
huishoudelijkafvalcontainer_dict = huishoudelijkafvalcontainer_instance.to_dict()
# create an instance of Huishoudelijkafvalcontainer from a dict
huishoudelijkafvalcontainer_from_dict = Huishoudelijkafvalcontainer.from_dict(huishoudelijkafvalcontainer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


