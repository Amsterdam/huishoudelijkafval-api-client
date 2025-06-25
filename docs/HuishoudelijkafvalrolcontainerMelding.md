# HuishoudelijkafvalrolcontainerMelding

Deze tabel bevat informatie over de meldingen die door de bewoners zijn gedaan. De meldingen gaan over een of meer containers.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultRolcontainerMeldingLinks**](HuishoudelijkafvaldefaultRolcontainerMeldingLinks.md) |  | 
**id** | **int** | Unieke aanduiding van een melding | 
**rolcontainer_id** | **int** | Unieke aanduiding van een rolcontainer. (foreign key) | [readonly] 
**melding_type** | **str** | Het type van een melding. Bijvoorbeeld: Algemene informatie | [optional] 
**afkomst_verzoek** | **str** | Dit attribuut geeft aan of de melding intern of extern is gedaan. | [optional] 
**soort_verzoek** | **str** | Dit attribuut geeft aan welk communicatiemiddel is gebruikt om de melding te registreren. | [optional] 
**aanmaakdatum** | **datetime** | De datum en tijd waarop de registratie van de melding in het systeem is vastgelegd | [optional] 
**wijzigingsdatum** | **datetime** | De datum en tijd waarop de registratie van de melding voor het laatst in het systeem is aangepast | [optional] 
**bag_verblijfsobject_id** | **str** | Een identificatiecode van een verblijfsobject is een authentiek gegeven en een unieke aanduiding van het verblijfsobject. | [readonly] 
**bag_nummeraanduiding_id** | **str** | BAG Nummeraanduiding identificatie | [readonly] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalrolcontainer_melding import HuishoudelijkafvalrolcontainerMelding

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalrolcontainerMelding from a JSON string
huishoudelijkafvalrolcontainer_melding_instance = HuishoudelijkafvalrolcontainerMelding.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalrolcontainerMelding.to_json())

# convert the object into a dict
huishoudelijkafvalrolcontainer_melding_dict = huishoudelijkafvalrolcontainer_melding_instance.to_dict()
# create an instance of HuishoudelijkafvalrolcontainerMelding from a dict
huishoudelijkafvalrolcontainer_melding_from_dict = HuishoudelijkafvalrolcontainerMelding.from_dict(huishoudelijkafvalrolcontainer_melding_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


