# HuishoudelijkafvalrolcontainerActie

Deze tabel bevat informatie over onderhoud handelingen.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultRolcontainerActieLinks**](HuishoudelijkafvaldefaultRolcontainerActieLinks.md) |  | 
**id** | **int** | Unieke aanduiding van een onderhoudsactie | 
**rolcontainer_id** | **int** | Unieke aanduiding van een rolcontainer. (foreign key) | [readonly] 
**actie_type_code** | **str** | Dit attribuut beschrijft de code van de actie type | [optional] 
**actie_type_naam** | **str** | Dit attribuut beschrijft de aard van de actie type | [optional] 
**interventie_datum** | **str** | De geplande datum voor een bepaalde actie. | [optional] 
**status** | **str** | Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. | [optional] 
**ronde** | **str** |  | [optional] 
**bezoek** | **int** | Het aantal bezoeken dat is afgelegd om het verzoek te realiseren. | [optional] 
**afkomst_verzoek** | **str** | Deze attribuut geeft aan of de actie door intern of extern verzoek is tot stand gekomen. | [optional] 
**soort_verzoek** | **str** | Dit attribuut geeft aan welk communicatiemiddel is gebruikt om het verzoek te registreren.. | [optional] 
**team** | **str** | Het team dat verantwoordelijk is voor het afhandelen van het verzoek. | [optional] 
**chip_nummer** | **str** | Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. | [optional] 
**soort_container** | **str** | Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. | [optional] 
**aanmaakdatum** | **datetime** | Datum tijd waarop de rolcontainer in het systeem is aangemaakt | [optional] 
**wijzigingsdatum** | **datetime** | Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast | [optional] 
**bag_verblijfsobject_id** | **str** | Een identificatiecode van een verblijfsobject is een authentiek gegeven en een unieke aanduiding van het verblijfsobject. | [readonly] 
**bag_nummeraanduiding_id** | **str** | BAG Identificatie nummeraanduiding | [readonly] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalrolcontainer_actie import HuishoudelijkafvalrolcontainerActie

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalrolcontainerActie from a JSON string
huishoudelijkafvalrolcontainer_actie_instance = HuishoudelijkafvalrolcontainerActie.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalrolcontainerActie.to_json())

# convert the object into a dict
huishoudelijkafvalrolcontainer_actie_dict = huishoudelijkafvalrolcontainer_actie_instance.to_dict()
# create an instance of HuishoudelijkafvalrolcontainerActie from a dict
huishoudelijkafvalrolcontainer_actie_from_dict = HuishoudelijkafvalrolcontainerActie.from_dict(huishoudelijkafvalrolcontainer_actie_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


