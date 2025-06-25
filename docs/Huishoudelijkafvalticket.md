# Huishoudelijkafvalticket

ticket

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultTicketLinks**](HuishoudelijkafvaldefaultTicketLinks.md) |  | 
**id** | **int** | Identificerend kenmerk van het ticket. | 
**container_id** | **str** | Identificerend kenmerk van de container. | [readonly] 
**containerlocatie_id** | **str** | Identificerend kenmerk van de containerlocatie. | [readonly] 
**datum_creatie** | **datetime** | De datum waarop het ticket aangemaakt is. | [optional] 
**datum_factuur** | **datetime** | De datum waarop het ticket gefactureerd is. | [optional] 
**factuur_nummer** | **str** | Het nummer van de factuur. | [optional] 
**datum_wijziging** | **datetime** | De datum waarop het ticket is gewijzigd. | [optional] 
**referentienummer_leverancier** | **str** | Het referentienummer dat door de leverancier aan het ticket gegeven wordt. | [optional] 
**prioriteit_opmerking** | **str** | Een opmerking die toegevoegd wordt om de prioritering te verduidelijken. | [optional] 
**prioriteit_naam** | **str** | De naam die de soort prioriteit weergeeft. | [optional] 
**prioriteit_responstijd** | **int** | De toegestane responsetijd voor deze prioriteit.  | [optional] 
**probleem_module_naam** | **List[str]** |  | [optional] 
**probleem** | **List[str]** |  | [optional] 
**oorzaak** | **List[str]** |  | [optional] 
**oplossing** | **List[str]** |  | [optional] 
**onderhoudsbedrijf** | **str** | De naam van het onderhoudsbedrijf. | [optional] 
**eigenaar** | **str** | De naam van de eigenaar van de container. | [optional] 
**ticketstatus** | **str** | De status van het ticket. | [optional] 
**tickettype** | **str** | De naam van het type ticket. | [optional] 
**rangorde_nummer_tickettype** | **int** | Het rangordenummer van het type ticket. | [optional] 
**datum_workflow_start** | **datetime** | De datum waarop de workflow start. | [optional] 
**datum_geaccepteerd** | **datetime** | De datum waarop het ticket geaccepteerd is door het onderhoudsbedrijf. | [optional] 
**datum_offerte** | **datetime** | De datum waarop de offerte is aangemaakt . | [optional] 
**datum_gepland** | **datetime** | De datum waarop de uitvoering van de werkzaamheden is ingepland. | [optional] 
**datum_gereed** | **datetime** | De datum waarop de werkzaamheden uitgevoerd zijn. | [optional] 
**datum_afgerond** | **datetime** | De datum waarop de werkzaamheden als gereed aangegeven zijn door het onderhoudsbedrijf. | [optional] 
**datum_technische_goedkeuring** | **datetime** | De datum waarop de technische aspecten van de werkzaamheden goed- of afgekeurd zijn. | [optional] 
**datum_financiele_goedkeuring** | **datetime** | De datum waarop de financiale aspecten van de werkzaamheden goed- of afgekeurd zijn. | [optional] 
**datum_gefactureerd** | **datetime** | De datum waarop de factuur in het systeem de status &#39;gefactureerd&#39; krijgt. | [optional] 
**datum_afgewezen** | **datetime** | De datum waarop het ticket de status &#39;afgewezen&#39; krijgt. | [optional] 
**reden_afgewezen** | **str** | De reden waarom het ticket de status &#39;afgewezen&#39; heeft gekregen. | [optional] 
**prijs** | **float** | De totale prijs van de gebruikte onderdelen en de uitgevoerde werkzaamheden. | [optional] 
**prijs_offerte** | **float** | De totale prijs op de offerte voor de te gebruiken onderdelen en de uit te voeren werkzaamheden. | [optional] 
**doorlooptijd** | **str** | De tijdsspanne in werkdagen tussen de &#39;datumCreatie&#39;en de &#39;datumAfgerond&#39; of de tijdsspanne in werkdagen tussen de &#39;datumCreatie&#39; en de laatste statuswijziging in het geval het ticket nog niet afgerond is. | [optional] 
**items_definitief** | **str** | De onderdelen en de werkzaamheden zoals deze op de factuur vermeld worden. | [optional] 
**items_offerte** | **str** | De onderdelen en de werkzaamheden zoals deze op de offerte vermeld worden. | [optional] 
**gbd_buurt_id** | **str** | Unieke identificatie van het object | [readonly] 
**gbd_buurt_naam** | **str** | De naam van het object. | [optional] 
**gbd_buurt_volgnummer** | **int** | Uniek volgnummer van de toestand van het object. | [optional] 
**gbd_buurt_code** | **str** | Unieke code. | [optional] 
**gbd_wijk_id** | **str** | Unieke identificatie van het object. | [readonly] 
**gbd_wijk_naam** | **str** | De naam van het object. | [optional] 
**gbd_wijk_volgnummer** | **int** | Uniek volgnummer van de toestand van het object. | [optional] 
**gbd_stadsdeel_id** | **str** | Unieke identificatie van het object. | [readonly] 
**gbd_stadsdeel_naam** | **str** | De naam van het object. | [optional] 
**gbd_stadsdeel_volgnummer** | **int** | Uniek volgnummer van de toestand van het object. | [optional] 
**gbd_ggw_id** | **str** | Unieke identificatie van het object. | [readonly] 
**gbd_ggw_naam** | **str** | De naam van het object. | [optional] 
**gbd_ggw_volgnummer** | **str** | Uniek volgnummer van de toestand van het object. | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalticket import Huishoudelijkafvalticket

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalticket from a JSON string
huishoudelijkafvalticket_instance = Huishoudelijkafvalticket.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalticket.to_json())

# convert the object into a dict
huishoudelijkafvalticket_dict = huishoudelijkafvalticket_instance.to_dict()
# create an instance of Huishoudelijkafvalticket from a dict
huishoudelijkafvalticket_from_dict = Huishoudelijkafvalticket.from_dict(huishoudelijkafvalticket_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


