# HuishoudelijkafvalplanningVoertuigen

Planningsgegevens van afvalinzamelingsvoertuigen voor huishoudelijk- en bedrijfsafval

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultPlanningVoertuigenLinks**](HuishoudelijkafvaldefaultPlanningVoertuigenLinks.md) |  | 
**id** | **int** | Uniek identificerend kenmerk van het record. | 
**soort_werkzaamheden** | **str** | Specificatie van soort planning (Inzet of Onderhoud). | [optional] 
**kenteken** | **str** | Kenteken afvalinzamelingsvoertuig. | [optional] 
**kenteken_kort** | **str** | Kenteken afvalinzamelingsvoertuig zonder koppeltekens (-). | [optional] 
**categorie** | **str** | Categorie afvalverwerking waar het voertuig op is gepland. | [optional] 
**activiteit** | **str** | Fractie van de afvalverwerking (afgeleid van categorie, werkzaamheden en of memo). | [optional] 
**werkzaamheden_code** | **str** | Code voor de werkzaamheden waarop het voertuig is gepland. | [optional] 
**werkzaamheden_omschrijving** | **str** | Omschrijving voor de werkzaamheden waarop het voertuig is gepland. | [optional] 
**werkzaamheden_datum** | **datetime** | Datum waarop de werkzaamheden zijn gepland. | [optional] 
**werkzaamheden_datum_ref_id** | **int** | Verwijzing naar datum dimensie. | [readonly] 
**werkzaamheden_starttijd** | **str** | Starttijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM | [optional] 
**werkzaamheden_eindtijd** | **str** | Eindtijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM. | [optional] 
**werkzaamheden_uren_gepland** | **float** | Berekening van het aantal bruto uren van de werkzaamheden (&#x3D; eindtijd - starttijd). | [optional] 
**pauze_starttijd** | **str** | Starttijd van de pauze op de WERKZAAMHEDEN_DATUM. | [optional] 
**pauze_eindtijd** | **str** | Eindtijd van de pauze op de WERKZAAMHEDEN_DATUM. | [optional] 
**pauze_uren_gepland** | **float** | Berekening van het aantal bruto uren van de pauze (&#x3D; eindtijd - starttijd). | [optional] 
**fase** | **str** | Label van de fase waarin de planning zich bevindt. | [optional] 
**memo** | **str** | Extra toelichting zoals opgegeven in (planningsdata)bronsysteem. | [optional] 
**team** | **str** | Team waarvoor de voertuigplanning is gemaakt. In veel gevallen een stadsdeel, maar kan ook bijvoorbeeld Bedrijfsafval Centrum (BAC) zijn). | [optional] 
**voertuig_inhuur_indicatie** | **str** | Is het voertuig ingehuurd (Ja / Nee). | [optional] 
**aantal_medewerkers** | **float** | Aantal medewerkers dat op het voertuig is gepland. | [optional] 
**aantal_medewerkers_intern** | **float** | Aantal interne medewerkers dat op het voertuig is gepland. | [optional] 
**aantal_medewerkers_inhuur** | **float** | Aantal externe medewerkers dat op het voertuig is gepland. | [optional] 
**uren_inzet_medewerker_intern** | **float** | Som van het totaal aantal netto uren van de interne medewerkers die op de planning zijn gezet (excl pauze). | [optional] 
**uren_inzet_medewerker_inhuur** | **float** | Som van het totaal aantal netto uren van de externe medewerkers die op de planning zijn gezet (excl pauze). | [optional] 
**uren_inzet_voertuig** | **float** | Netto inzeturen van het voertuig (bruto - pauze). | [optional] 
**datum_verwerkt_stadsdelen** | **datetime** | Moment van laden data vanuit het (planningsdata)bronsysteem in het DWH stadsdelen (als intermediair voor datalevering). | [optional] 
**datum_aanwezig_bron** | **datetime** | Indicatie over de actualiteit van de gegevens in deze set (laatste wijziging in de bron). | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalplanning_voertuigen import HuishoudelijkafvalplanningVoertuigen

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalplanningVoertuigen from a JSON string
huishoudelijkafvalplanning_voertuigen_instance = HuishoudelijkafvalplanningVoertuigen.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalplanningVoertuigen.to_json())

# convert the object into a dict
huishoudelijkafvalplanning_voertuigen_dict = huishoudelijkafvalplanning_voertuigen_instance.to_dict()
# create an instance of HuishoudelijkafvalplanningVoertuigen from a dict
huishoudelijkafvalplanning_voertuigen_from_dict = HuishoudelijkafvalplanningVoertuigen.from_dict(huishoudelijkafvalplanning_voertuigen_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


