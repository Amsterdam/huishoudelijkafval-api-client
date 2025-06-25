# Huishoudelijkafvalafvoermomenten

Bevat gegevens over wat en hoeveel is aangeboden bij verschillende afvalwerkers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**Huishoudelijkafvalv0AfvoermomentenLinks**](Huishoudelijkafvalv0AfvoermomentenLinks.md) |  | 
**id** | **str** | Unieke aanduiding van het record. Combinatie verwerker en bon nummer | 
**verwerker** | **str** | Naam van de verwerker | [optional] 
**bon_nummer** | **str** | Unieke identificatie voor de afvalverwerking van de afvalverwerker. | [optional] 
**datum** | **date** | Datum van de afvalverwerking of registratie. | [optional] 
**tijd** | **str** | Tijdstip van de verwerking of registratie. | [optional] 
**ontvangst_locatie** | **str** | Locatie waar het afval wordt ontvangen. | [optional] 
**afvalstroom_nummer** | **str** | Afvalstroomnummer, een unieke code voor de afvalstroom. | [optional] 
**aanbieder** | **str** | Naam van de afvalaanbieder (klant, bedrijf of gemeente). | [optional] 
**aanbieder_standplaats** | **str** | Locatie waar het afval is opgehaald. | [optional] 
**aanbieder_standplaats_omschrijving** | **str** | Beschrijving van de ophaallocatie. | [optional] 
**aanbieder_adres** | **str** | Adres van de afvalaanbieder. | [optional] 
**aanbieder_postcode** | **str** | Postcode van de afvalaanbieder. | [optional] 
**aanbieder_plaatsnaam** | **str** | Plaatsnaam van de afvalaanbieder. | [optional] 
**afval_soort** | **str** | Beschrijving van het afval of de activiteit. | [optional] 
**geaccepteerd** | **str** | Status of het afval is geaccepteerd bij de ontvangstlocatie. | [optional] 
**opmerking** | **str** | Aanvullende informatie over de afvalverwerking. | [optional] 
**kenteken** | **str** |  Kenteken van het voertuig dat het afval vervoert. | [optional] 
**kenteken_kort** | **str** | Kenteken zonder &#39;-&#39;. Ten behove van koppeling met wagenpark_voertuig | [optional] 
**weeg_bon** | **str** | Nummer van de weegbon van de aanbieder voor het geregistreerde gewicht. | [optional] 
**weeg_datum** | **date** | Datum waarop het afval is gewogen. | [optional] 
**weeg_tijdstip** | **str** | Tijdstip waarop het afval is gewogen. | [optional] 
**inweging** | **int** | Gewicht van het voertuig inclusief lading bij binnenkomst. | [optional] 
**uitweging** | **int** | Gewicht van het voertuig zonder lading bij vertrek. | [optional] 
**netto_gewicht** | **str** | Verschil tussen vol en leeg gewicht, oftewel het gewicht van het afval. | [optional] 
**afvalstof_code** | **str** | Code die het type afvalstof identificeert. | [optional] 
**afvalstof_omschrijving** | **str** | Kenteken van het voertuig dat het afval vervoert. | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalafvoermomenten import Huishoudelijkafvalafvoermomenten

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalafvoermomenten from a JSON string
huishoudelijkafvalafvoermomenten_instance = Huishoudelijkafvalafvoermomenten.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalafvoermomenten.to_json())

# convert the object into a dict
huishoudelijkafvalafvoermomenten_dict = huishoudelijkafvalafvoermomenten_instance.to_dict()
# create an instance of Huishoudelijkafvalafvoermomenten from a dict
huishoudelijkafvalafvoermomenten_from_dict = Huishoudelijkafvalafvoermomenten.from_dict(huishoudelijkafvalafvoermomenten_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


