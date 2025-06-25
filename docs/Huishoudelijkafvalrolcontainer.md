# Huishoudelijkafvalrolcontainer

Deze tabel bevat informatie over de stanmgegevens van de rolcontainers in Gemeente Amsterdam

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultRolcontainerLinks**](HuishoudelijkafvaldefaultRolcontainerLinks.md) |  | 
**id** | **int** | Unieke aanduiding van een rolcontainer | 
**fractie_omschrijving** | **str** | Container fractieomschrijving zoals door leverancier is geleverd. | [optional] 
**chip_nummer** | **str** | Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. | [optional] 
**chip_type** | **str** | Het type van de chip dat aan de rolcontainer is bevestigd. | [optional] 
**heeft_chip_sinds** | **date** | Datum waarop de chip aan de rolcontainer is bevestigd.  | [optional] 
**barcode** | **str** | De barcode van de chip dat van buitenaf leesbaar is. | [optional] 
**heeft_barcode_sinds** | **date** | Dit attribuut, heeft_barcode_sinds, geeft de datum aan waarop de chip is voorzien van een barcode.. | [optional] 
**status** | **str** | Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. | [optional] 
**status_sinds** | **date** | Datum waarop de laatste status van een rolcontainer van toepassing is | [optional] 
**aanmaakdatum** | **datetime** | Datum tijd waarop de rolcontainer in het systeem is aangemaakt | [optional] 
**wijzigingsdatum** | **datetime** | Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast | [optional] 
**soort_container** | **str** | Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. | [optional] 
**straatnaam** | **str** | Naam van de straat | [optional] 
**huisnummer** | **int** | De numerieke aanduiding zoals deze door het gemeente bestuur aan het object is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende nummering. | [optional] 
**huisletter** | **str** | Een alfabetisch teken achter het huisnummer zoals dit door het gemeentebestuur is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende toevoeging aan een huisnummer in de vorm van een alfabetisch teken. | [optional] 
**huisnummertoevoeging** | **str** | Die let­ters of te­kens die nood­za­ke­lijk zijn om, naast huis­num­mer en -let­ter, de brie­ven­bus te vin­den dan wel een door of na­mens het be­voeg­de ge­meen­te­lij­ke or­gaan ten aan­zien van een adres­seer­baar ob­ject toe­ge­ken­de toe­voe­ging aan een huis­num­mer of een com­bi­na­tie van huis­let­ter en huis­num­mer | [optional] 
**postcode** | **str** | De door de Post NL vast­ge­stel­de code be­ho­rend bij de straat­naam en het huis­num­mer dan wel de door Post NL vast­ge­stel­de code be­ho­ren­de bij een be­paal­de com­bi­na­tie van een naam open­ba­re ruim­te en een huis­num­mer. | [optional] 
**woonplaats_naam** | **str** | Een Woonplaats is een door het bevoegde gemeentelijke orgaan als zodanig aangewezen en van een naam voorzien gedeelte van het grondgebied van de gemeente. | [optional] 
**geometrie** | [**Point**](Point.md) |  | [optional] 
**typeadresseerbaarobject** | **str** | Een Adresseerbaar object is een (abstract) object waaraan adressen kunnen worden toegekend | [optional] 
**gebruiksdoel** | **str** | Een categorisering van de gebruiksdoelen van het betreffende adreseerbareobject, zoals dit door de overheid als zodanig is toegestaan | [optional] 
**bag_woonplaats_id** | **str** | Officiële naam woonplaats | [readonly] 
**bag_openbareruimte_id** | **str** | BAG Openbare ruimte identificatie | [readonly] 
**bag_verblijfsobject_id** | **str** | Een identificatiecode van een verblijfsobject is een authentiek gegeven en een unieke aanduiding van het verblijfsobject. | [readonly] 
**bag_nummeraanduiding_id** | **str** | BAG Nummeraanduiding identificatie | [readonly] 
**gebied_buurt_naam** | **str** | De naam van het object | [optional] 
**gebied_buurt_code** | **str** | Unieke code (hier in zie je de Stadsdeel- en Wijkcode terug) | [optional] 
**gebied_buurt_id** | **str** | Unieke identificatie van het object (naam van het kenmerk wijzigt van ID naar Identificatie in 2019) | [readonly] 
**gebied_wijk_naam** | **str** | De naam van de wijk | [optional] 
**gebied_wijk_code** | **str** | Volledige, samengestelde, code, bestaande uit stadsdeelcode en wijkcode | [optional] 
**gebied_wijk_id** | **str** | Unieke identificatie van het object (In 2019 wijzigt de naam van het kenmerk van ID naar Identificatie) | [readonly] 
**gebied_stadsdeel_naam** | **str** | De naam van het stadsdeel. | [optional] 
**gebied_stadsdeel_code** | **str** | Officile code van het stadsdeel | [optional] 
**gebied_stadsdeel_id** | **str** | Unieke identificatie van het object (in 2019 wijzigt de naam van het kenmerk van ID naar Identificatie) | [readonly] 
**gebied_ggw_naam** | **str** | De naam van het gebiedsgericht werken gebied | [optional] 
**gebied_ggw_code** | **str** | De unieke code van het gebiedsgericht werken gebied | [optional] 
**gebied_ggw_id** | **str** | De unieke identificatie van het gebiedsgericht werken gebied | [readonly] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalrolcontainer import Huishoudelijkafvalrolcontainer

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalrolcontainer from a JSON string
huishoudelijkafvalrolcontainer_instance = Huishoudelijkafvalrolcontainer.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalrolcontainer.to_json())

# convert the object into a dict
huishoudelijkafvalrolcontainer_dict = huishoudelijkafvalrolcontainer_instance.to_dict()
# create an instance of Huishoudelijkafvalrolcontainer from a dict
huishoudelijkafvalrolcontainer_from_dict = Huishoudelijkafvalrolcontainer.from_dict(huishoudelijkafvalrolcontainer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


