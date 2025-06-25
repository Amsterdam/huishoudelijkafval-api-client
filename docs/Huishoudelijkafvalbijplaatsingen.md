# Huishoudelijkafvalbijplaatsingen

De Aanpak Bijplaatsingen (ABP) richt zich op afval dat op onjuiste wijze buiten wordt geplaatst. Momenteel wordt dit door de Gemeente Amsterdam op wijkniveau aangepakt via de ABP. Door communicatiemiddelen en interventies in te zetten rondom de meest vervuilde containerlocaties, neemt de netheid toe en daalt het aantal bijplaatsingen. Dit dataproduct bevat de registratie van bijplaatsingen zoals vastgelegd door de bevoegde medewerkers.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultBijplaatsingenLinks**](HuishoudelijkafvaldefaultBijplaatsingenLinks.md) |  | 
**id** | **str** | Unieke aanduiding van het record. | 
**datum_waarneming** | **date** | De datum waarop de waarneming is geregistreerd. | [optional] 
**tijd_waarneming** | **str** | De tijdstip waarop de waarneming is geregistreerd. | [optional] 
**cluster_id** | **str** | Uniek identificerend kenmerk van cluster | [readonly] 
**gbd_buurt_code** | **str** | Unieke code (hierin zie je de Stadsdeel- en Wijkcode terug) | [optional] 
**gbd_buurt_id** | **str** | Unieke identificatie van het object (naam van het kenmerk wijzigt van ID naar Identificatie in 2019) | [readonly] 
**bag_openbareruimte_id** | **str** | Unieke identificatie van het object | [readonly] 
**bag_verblijfsobject_id** | **str** | Een identificatiecode van een verblijfsobject is een authentiek gegeven en een unieke aanduiding van het verblijfsobject. | [readonly] 
**bag_nummeraanduiding_id** | **str** | Identificatie nummeraanduiding | [readonly] 
**bag_woonplaats_id** | **str** | Identificatie woonplaats | [readonly] 
**geometrie** | [**Point**](Point.md) |  | [optional] 
**bruingoed** | **bool** | Aangetroffen afvalsoort (bruingoed) rondom de container(s) | [optional] 
**containervies** | **bool** | De uiterlijke toestand van de container(s). Container is vies en moet worden schoongemaakt | [optional] 
**crow_score** | **str** | De score van CROW inspectie. A+: 0 stuks afval, A: &lt;&#x3D; 1 stuk, B: &lt;&#x3D; 3 stuks, C: &lt;&#x3D; 5 stuks, D: &gt; 5 stuks | [optional] 
**glas** | **bool** | Aangetroffen afvalsoort (glas afval) rondom de container(s) | [optional] 
**glasgestremd** | **bool** | De glascontainer is gestremd | [optional] 
**glastoegankelijk** | **bool** | De glascontainer is toegangelijk | [optional] 
**glasvol** | **bool** | De glascontainer is vol | [optional] 
**grof** | **bool** | Aangetroffen afvalsoort (grofvuil) rondom de container(s) | [optional] 
**handhaving** | **bool** | Er zijn items aangetroffen met adresgegevens en is er dus handhaving nodig | [optional] 
**waarde_handhaving** | **str** | Hoe veel items met adresgegevens zijn er aangetroffen? | [optional] 
**huisvuil** | **bool** | Aangetroffen afvalsoort (huisvuil) rondom de container(s) | [optional] 
**karton** | **bool** | Aangetroffen afvalsoort (karton) rondom de container(s) | [optional] 
**overig** | **bool** | Aangetroffen afvalsoort (overig) rondom de container(s) | [optional] 
**papiervol** | **bool** | De papiercontainer is vol | [optional] 
**papiergestremd** | **bool** | De papiercontainer is gestremd | [optional] 
**papiertoegankelijk** | **bool** | De papiercontainer is toegankelijk | [optional] 
**restgestremd** | **bool** | De restcontainer is gestremd | [optional] 
**resttoegankelijk** | **bool** | De restcontainer is toegankelijk | [optional] 
**restvol** | **bool** | De restcontainer is vol | [optional] 
**veegvuil** | **bool** | Aangetroffen afvalsoort (veegvuil) rondom de container(s) | [optional] 
**zwerfafval** | **bool** | Aangetroffen afvalsoort (zwerfafval) rondom de container(s) | [optional] 
**waarnemer_rol** | **str** | De rol van de melder | [optional] 
**gbd_stadsdeel_naam** | **str** | Naam van het stadsdeel waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). | [optional] 
**postcode** | **str** | De postcode van de locatie waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). | [optional] 
**straatnaam** | **str** | De straat van de locatie waar de waarneming is geregistreerd (afgeleid op basis van de geometrie). | [optional] 
**locatie_waarnemer** | **str** | De locatie (stadsdeel) vanwaar de waarnemer in het systeem is ingelogd. | [optional] 
**type_waarneming** | **str** | Geeft aan of de waarneming een CROW waarneming is. | [optional] 
**grofvuildagen** | **str** | De waarde is &#39;true&#39; of &#39;false&#39; en geeft per dag aan of het waar of onwaar is. De eerste waarde correspondeert met maandag. | [optional] 
**adres_type** | **str** | Het type meetlocatie geeft aan om wat voor soort locatie het gaat. De locatie typen zijn er. Extra: De gemeten locatie bevond zich niet op de route, maar er is wel een meting van uitgevoerd. Bijvoorbeeld: een locatie die buiten de route ligt, heeft bijplaatsingen ernaast staan. Null: De gemeten locatie bevond zich op de route en werd direct gemeten zodra deze verscheen. Postponed: De meting van de locatie was eerder uitgesteld. Bijvoorbeeld, wanneer een locatie niet bereikbaar is, kun je deze uitstellen, waarna deze later opnieuw op de route verschijnt.  Forwarded: De gemeten locatie is bij het team binnengekomen omdat een ander team daar iets relevants had aangetroffen. Bijvoorbeeld: de werkbrigade vindt karton met adressen bij een locatie, vult aan het einde van het formulier in dat dit door het team gecontroleerd moet worden. De locatie wordt vervolgens toegevoegd aan de route.  | [optional] 
**dumpplek** | **bool** | Het geeft aan of de locatie een dumpplek is. | [optional] 
**melding_door_collega_doorgezet** | **str** | Het geeft aan of de waarneming door een collega is doorgezet. | [optional] 
**naam_melding_doorgezet** | **str** | Soort doorgezette waarneming. | [optional] 
**gebruikers_rol** | **str** | De rol van de gebruiker in de applicatie. | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalbijplaatsingen import Huishoudelijkafvalbijplaatsingen

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalbijplaatsingen from a JSON string
huishoudelijkafvalbijplaatsingen_instance = Huishoudelijkafvalbijplaatsingen.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalbijplaatsingen.to_json())

# convert the object into a dict
huishoudelijkafvalbijplaatsingen_dict = huishoudelijkafvalbijplaatsingen_instance.to_dict()
# create an instance of Huishoudelijkafvalbijplaatsingen from a dict
huishoudelijkafvalbijplaatsingen_from_dict = Huishoudelijkafvalbijplaatsingen.from_dict(huishoudelijkafvalbijplaatsingen_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


