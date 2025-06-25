# Huishoudelijkafvalcontainerlocatie

containerlocatie

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultContainerlocatieLinks**](HuishoudelijkafvaldefaultContainerlocatieLinks.md) |  | 
**id** | **str** | Identificerend kenmerk van de put waarin de container is geplaatst | 
**serienummer** | **str** | serienummer uitgegeven door de fabrikant | [optional] 
**status** | **int** | Status van de container, 0 - inactief, 1 - actief, 2 - gepland | [optional] 
**geometrie** | [**Point**](Point.md) |  | [optional] 
**eigenaar_id** | **str** | Identificerend kenmerk eigenaar | [optional] 
**eigenaar_naam** | **str** | Naam eigenaar | [optional] 
**datum_creatie** | **str** | Datum waarop het object is gecreëerd in container management systeem | [optional] 
**datum_plaatsing** | **str** | Datum waarop het object op de locatie is geplaatst | [optional] 
**datum_operationeel** | **str** | Datum waarop het object is operationeel gezet | [optional] 
**datum_oplevering** | **str** | Datum waarop het object is opgeleleverd | [optional] 
**wijzigingsdatum_dp** | **datetime** | Datum waarop het object is gewijzigd | [optional] 
**verwijderd_dp** | **bool** | Indicatie of het object verwijderd is bij de bronhouder | [optional] 
**datum_einde_garantie** | **str** | Datum waarop de garantie verloopt | [optional] 
**ind_bevat_container** | **bool** | Indicatie dat de containerlocatie een container bevat | [optional] 
**bag_hoofdadres_verblijfsobject_id** | **str** | Een identificatiecode van een verblijfsobject is een authentiek gegeven en een unieke aanduiding van het verblijfsobject. | [readonly] 
**gbd_buurt_id** | **str** | Unieke identificatie van het object | [readonly] 
**bag_openbareruimte_id** | **str** | Openbare ruimte identificatie | [readonly] 
**bag_nummeraanduiding_id** | **str** | Identificatie nummeraanduiding | [readonly] 
**containerlocatie_type_naam** | **str** | Het type van de containerlocatie | [optional] 
**containerlocatie_id_nummer** | **str** | Definitie volgt nog | [optional] 
**containerlocatie_datum_wijziging** | **datetime** | Datum waarop het object is gewijzigd. | [optional] 
**containerlocatie_opmerking** | **str** | Opmerking over het object. | [optional] 
**containerlocatie_end_of_life** | **date** | Datum waarop het object het einde van zijn levenscyclus heeft bereikt. | [optional] 
**containerlocatie_eigenaarschap** | **str** | Soort eigenaarschap | [optional] 
**containerlocatie_eigenaarschap_opmerking** | **str** | Beschrijving van het type eigenaarschap. | [optional] 
**containerlocatie_type_artikelcode** | **str** | Artikelcode van het containerlocatietype. | [optional] 
**bronadres** | **str** | Adres van de containerlocatie zoals die in bron geregistreerd is. | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalcontainerlocatie import Huishoudelijkafvalcontainerlocatie

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalcontainerlocatie from a JSON string
huishoudelijkafvalcontainerlocatie_instance = Huishoudelijkafvalcontainerlocatie.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalcontainerlocatie.to_json())

# convert the object into a dict
huishoudelijkafvalcontainerlocatie_dict = huishoudelijkafvalcontainerlocatie_instance.to_dict()
# create an instance of Huishoudelijkafvalcontainerlocatie from a dict
huishoudelijkafvalcontainerlocatie_from_dict = Huishoudelijkafvalcontainerlocatie.from_dict(huishoudelijkafvalcontainerlocatie_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


