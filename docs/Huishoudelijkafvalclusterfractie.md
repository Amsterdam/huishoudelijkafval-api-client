# Huishoudelijkafvalclusterfractie

clusterfractie

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultClusterfractieLinks**](HuishoudelijkafvaldefaultClusterfractieLinks.md) |  | 
**id** | **str** | Uniek identificerend kenmerk van clusterfractie | 
**cluster_id** | **str** | Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd | [optional] 
**aantal_containers** | **int** | Aantal containers per clusterfractie | [optional] 
**volume_m3** | **float** | De som van het volume (m3) van containers per clusterfractie | [optional] 
**code** | **str** | Code afvalfractie zoals door Welvaarts is aanleverd. 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 7 - Grof, 8 - PMD, 9 - Brood, -999 - Onbekend | [optional] 
**omschrijving** | **str** | Afvalfractie zoals door Welvaarts is aangeleverd | [optional] 
**datum_opvoer** | **datetime** | De datum waarop de cluster in het systeem is opgevoerd. | [optional] 
**datum_einde** | **date** | De datum waarop de cluster in het systeem is eindigd. | [optional] 
**wijzigingsdatum_dp** | **datetime** | De datum waarop de cluster in het systeem is gewijzigd. | [optional] 
**verwijderd_dp** | **bool** | indicatie of het object verwijderd is bij de bronhouder | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalclusterfractie import Huishoudelijkafvalclusterfractie

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalclusterfractie from a JSON string
huishoudelijkafvalclusterfractie_instance = Huishoudelijkafvalclusterfractie.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalclusterfractie.to_json())

# convert the object into a dict
huishoudelijkafvalclusterfractie_dict = huishoudelijkafvalclusterfractie_instance.to_dict()
# create an instance of Huishoudelijkafvalclusterfractie from a dict
huishoudelijkafvalclusterfractie_from_dict = Huishoudelijkafvalclusterfractie.from_dict(huishoudelijkafvalclusterfractie_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


