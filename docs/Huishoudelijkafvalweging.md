# Huishoudelijkafvalweging

weging

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**Huishoudelijkafvalv1WegingLinks**](Huishoudelijkafvalv1WegingLinks.md) |  | 
**id** | **str** | Uniek identificerend kenmerk weging. Deze is per container vastgelegd | 
**cluster_id** | **str** | Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd | [optional] 
**cluster_subcluster_indicatie** | **bool** | Indicatie of het een cluster betreft dat is gesplitst door een weg | [optional] 
**weegsysteem_id** | **int** | Identificerend kenmerk weegsysteem (behorend bij voertuig) | [optional] 
**weegsysteem_omschrijving** | **str** | Omschrijving van weegsysteem | [optional] 
**volgnummer** | **int** | Oplopende nummering wegingen per weegsysteem | [optional] 
**datum_weging** | **date** | Datum wanneer de weging is uitgevoerd (yyyy-mm-dd) | [optional] 
**tijdstip_weging** | **str** | Tijdstip wanneer de weging is uitgevoerd (HH24:MI:SS) | [optional] 
**locatienummer** | **str** | Locatienummer (cluster) zoals door Welvaarts is aangeleverd | [optional] 
**fractie_code** | **int** | Code afvalfractie zoals door Welvaarts is aangeleverd, 1: Rest, 2: Glas, 3: Papier, 4: Plastic, 5: Textiel, 6: GFT, 7: Grof, 8: PMD, 9: Brood, -99: Onbekend | [optional] 
**fractie_omschrijving** | **str** | Omschrijving afvalfractie zoals door Welvaarts is aangeleverd | [optional] 
**eerste_weging** | **float** | Eerste weging container: gewicht vol in Kg | [optional] 
**tweede_weging** | **float** | Tweede weging container: gewicht vol in Kg | [optional] 
**netto_gewicht** | **float** | Netto gewicht van het ingezamelde afval van de container in Kg | [optional] 
**geometrie** | [**Point**](Point.md) |  | [optional] 
**bediening_code** | **int** | Code van de wijze waarop de bediening van de weging heeft plaatsgevonden. Mogelijke waarden: 0 - Handmatig, 1 - Automatisch, 3 - onbekend. | [optional] 
**bediening_omschrijving** | **str** | Omschrijving van de wijze waarop de bediening van de weging heeft plaatsgevonden | [optional] 
**wijzigingsdatum_dp** | **datetime** | Datum waarop het object is gewijzigd | [optional] 
**verwijderd_dp** | **bool** | Indicatie of het object verwijderd is bij de bronhouder | [optional] 
**bag_hoofdadres_verblijfsobject_id** | **str** | Een identificatiecode van een verblijfsobject is een authentiek gegeven en een unieke aanduiding van het verblijfsobject. | [readonly] 
**gbd_buurt_id** | **str** | Unieke identificatie van het object | [readonly] 
**bag_openbareruimte_id** | **str** | Openbare ruimte identificatie | [readonly] 
**bag_nummeraanduiding_id** | **str** | Identificatie nummeraanduiding | [readonly] 
**weging_kenteken** | **str** | Het kenteken van het voertuig | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalweging import Huishoudelijkafvalweging

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalweging from a JSON string
huishoudelijkafvalweging_instance = Huishoudelijkafvalweging.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalweging.to_json())

# convert the object into a dict
huishoudelijkafvalweging_dict = huishoudelijkafvalweging_instance.to_dict()
# create an instance of Huishoudelijkafvalweging from a dict
huishoudelijkafvalweging_from_dict = Huishoudelijkafvalweging.from_dict(huishoudelijkafvalweging_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


