# HuishoudelijkafvalloopafstandCategorieV2

loopafstandCategorieV2

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultLoopafstandCategorieV2Links**](HuishoudelijkafvaldefaultLoopafstandCategorieV2Links.md) |  | 
**id** | **str** | identificatie categorie loopafstand | 
**fractie** | **str** | Code afvalfractie waarnaar de afstand is bepaald | [optional] 
**fractie_omschrijving** | **str** | Omschrijving afvalfractie waarnaar de afstand is bepaald | [optional] 
**loopafstand_categorie_omschrijving** | **str** | Omschrijving van de categorie waarin de berekende loopafstand valt | [optional] 
**loopafstand_categorie_vanaf** | **int** | Ondergrens van de categorie waarin de berekende loopafstand valt | [optional] 
**loopafstand_categorie_tot** | **int** | Bovengrens van de categorie waarin de berekende loopafstand valt | [optional] 
**wijzigingsdatum_dp** | **datetime** | Datum waarop het object is gewijzigd | [optional] 
**verwijderd_dp** | **bool** | Indicatie of het object verwijderd is in de datapijplijn | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalloopafstand_categorie_v2 import HuishoudelijkafvalloopafstandCategorieV2

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalloopafstandCategorieV2 from a JSON string
huishoudelijkafvalloopafstand_categorie_v2_instance = HuishoudelijkafvalloopafstandCategorieV2.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalloopafstandCategorieV2.to_json())

# convert the object into a dict
huishoudelijkafvalloopafstand_categorie_v2_dict = huishoudelijkafvalloopafstand_categorie_v2_instance.to_dict()
# create an instance of HuishoudelijkafvalloopafstandCategorieV2 from a dict
huishoudelijkafvalloopafstand_categorie_v2_from_dict = HuishoudelijkafvalloopafstandCategorieV2.from_dict(huishoudelijkafvalloopafstand_categorie_v2_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


