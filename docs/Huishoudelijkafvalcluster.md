# Huishoudelijkafvalcluster

cluster

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultClusterLinks**](HuishoudelijkafvaldefaultClusterLinks.md) |  | 
**id** | **str** | Uniek identificerend kenmerk van cluster | 
**subcluster_indicatie** | **bool** | Indicatie of het een cluster betreft dat is gesplitst door een weg | [optional] 
**geometrie** | [**Point**](Point.md) |  | [optional] 
**datum_opvoer** | **datetime** | Datum opvoer van het cluster. Dit is afgeleid van wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 | [optional] 
**datum_ontstaan** | **date** | Datum ontstaan van het cluster. Dit is afgeleid van de plaatsingsdatum van de oudste container ,wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 | [optional] 
**datum_einde** | **date** | Datum wanneer het cluster geen relaties meer heeft met containers met status&#x3D;1. | [optional] 
**wijzigingsdatum_dp** | **datetime** | Datum waarop het object is gewijzigd | [optional] 
**verwijderd_dp** | **bool** | Indicatie of het object verwijderd is bij de bronhouder | [optional] 
**status** | **int** | Status van het cluster (0 - inactief , 1 - actief) | [optional] 
**bag_hoofdadres_verblijfsobject_id** | **str** | Een identificatiecode van een verblijfsobject is een authentiek gegeven en een unieke aanduiding van het verblijfsobject. | [readonly] 
**gbd_buurt_id** | **str** | Unieke identificatie van het object | [readonly] 
**bag_openbareruimte_id** | **str** | Openbare ruimte identificatie | [readonly] 
**bag_nummeraanduiding_id** | **str** | Identificatie nummeraanduiding | [readonly] 
**bronadres** | **str** | Adres van het cluster zoals die in bron geregistreerd is. | [optional] 
**opmerking** | **str** | Extra aanwijzing van de locatie voor de bestuurder. | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalcluster import Huishoudelijkafvalcluster

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalcluster from a JSON string
huishoudelijkafvalcluster_instance = Huishoudelijkafvalcluster.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalcluster.to_json())

# convert the object into a dict
huishoudelijkafvalcluster_dict = huishoudelijkafvalcluster_instance.to_dict()
# create an instance of Huishoudelijkafvalcluster from a dict
huishoudelijkafvalcluster_from_dict = Huishoudelijkafvalcluster.from_dict(huishoudelijkafvalcluster_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


