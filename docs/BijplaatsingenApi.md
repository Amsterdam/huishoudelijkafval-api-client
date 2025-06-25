# huishoudelijkafval_api_client.BijplaatsingenApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_bijplaatsingen_list2**](BijplaatsingenApi.md#huishoudelijkafval_bijplaatsingen_list2) | **GET** /bijplaatsingen | 
[**huishoudelijkafval_bijplaatsingen_retrieve2**](BijplaatsingenApi.md#huishoudelijkafval_bijplaatsingen_retrieve2) | **GET** /bijplaatsingen/{id} | 


# **huishoudelijkafval_bijplaatsingen_list2**
> PaginatedHuishoudelijkafvalbijplaatsingenList huishoudelijkafval_bijplaatsingen_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, adres_type=adres_type, adres_type_in=adres_type_in, adres_type_isempty=adres_type_isempty, adres_type_isnull=adres_type_isnull, adres_type_like=adres_type_like, adres_type_not=adres_type_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bag_woonplaats_identificatie=bag_woonplaats_identificatie, bag_woonplaats_identificatie_in=bag_woonplaats_identificatie_in, bag_woonplaats_identificatie_isempty=bag_woonplaats_identificatie_isempty, bag_woonplaats_identificatie_isnull=bag_woonplaats_identificatie_isnull, bag_woonplaats_identificatie_like=bag_woonplaats_identificatie_like, bag_woonplaats_identificatie_not=bag_woonplaats_identificatie_not, bruingoed=bruingoed, bruingoed_isnull=bruingoed_isnull, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, containervies=containervies, containervies_isnull=containervies_isnull, crow_score=crow_score, crow_score_in=crow_score_in, crow_score_isempty=crow_score_isempty, crow_score_isnull=crow_score_isnull, crow_score_like=crow_score_like, crow_score_not=crow_score_not, datum_waarneming=datum_waarneming, datum_waarneming_gt=datum_waarneming_gt, datum_waarneming_gte=datum_waarneming_gte, datum_waarneming_in=datum_waarneming_in, datum_waarneming_isnull=datum_waarneming_isnull, datum_waarneming_lt=datum_waarneming_lt, datum_waarneming_lte=datum_waarneming_lte, datum_waarneming_not=datum_waarneming_not, dumpplek=dumpplek, dumpplek_isnull=dumpplek_isnull, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, gbd_buurt_code=gbd_buurt_code, gbd_buurt_code_in=gbd_buurt_code_in, gbd_buurt_code_isempty=gbd_buurt_code_isempty, gbd_buurt_code_isnull=gbd_buurt_code_isnull, gbd_buurt_code_like=gbd_buurt_code_like, gbd_buurt_code_not=gbd_buurt_code_not, gbd_stadsdeel_naam=gbd_stadsdeel_naam, gbd_stadsdeel_naam_in=gbd_stadsdeel_naam_in, gbd_stadsdeel_naam_isempty=gbd_stadsdeel_naam_isempty, gbd_stadsdeel_naam_isnull=gbd_stadsdeel_naam_isnull, gbd_stadsdeel_naam_like=gbd_stadsdeel_naam_like, gbd_stadsdeel_naam_not=gbd_stadsdeel_naam_not, gebruikers_rol=gebruikers_rol, gebruikers_rol_in=gebruikers_rol_in, gebruikers_rol_isempty=gebruikers_rol_isempty, gebruikers_rol_isnull=gebruikers_rol_isnull, gebruikers_rol_like=gebruikers_rol_like, gebruikers_rol_not=gebruikers_rol_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, glas=glas, glas_isnull=glas_isnull, glasgestremd=glasgestremd, glasgestremd_isnull=glasgestremd_isnull, glastoegankelijk=glastoegankelijk, glastoegankelijk_isnull=glastoegankelijk_isnull, glasvol=glasvol, glasvol_isnull=glasvol_isnull, grof=grof, grof_isnull=grof_isnull, grofvuildagen=grofvuildagen, grofvuildagen_in=grofvuildagen_in, grofvuildagen_isempty=grofvuildagen_isempty, grofvuildagen_isnull=grofvuildagen_isnull, grofvuildagen_like=grofvuildagen_like, grofvuildagen_not=grofvuildagen_not, handhaving=handhaving, handhaving_isnull=handhaving_isnull, huisvuil=huisvuil, huisvuil_isnull=huisvuil_isnull, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, karton=karton, karton_isnull=karton_isnull, locatie_waarnemer=locatie_waarnemer, locatie_waarnemer_in=locatie_waarnemer_in, locatie_waarnemer_isempty=locatie_waarnemer_isempty, locatie_waarnemer_isnull=locatie_waarnemer_isnull, locatie_waarnemer_like=locatie_waarnemer_like, locatie_waarnemer_not=locatie_waarnemer_not, melding_door_collega_doorgezet=melding_door_collega_doorgezet, melding_door_collega_doorgezet_in=melding_door_collega_doorgezet_in, melding_door_collega_doorgezet_isempty=melding_door_collega_doorgezet_isempty, melding_door_collega_doorgezet_isnull=melding_door_collega_doorgezet_isnull, melding_door_collega_doorgezet_like=melding_door_collega_doorgezet_like, melding_door_collega_doorgezet_not=melding_door_collega_doorgezet_not, naam_melding_doorgezet=naam_melding_doorgezet, naam_melding_doorgezet_in=naam_melding_doorgezet_in, naam_melding_doorgezet_isempty=naam_melding_doorgezet_isempty, naam_melding_doorgezet_isnull=naam_melding_doorgezet_isnull, naam_melding_doorgezet_like=naam_melding_doorgezet_like, naam_melding_doorgezet_not=naam_melding_doorgezet_not, overig=overig, overig_isnull=overig_isnull, page=page, papiergestremd=papiergestremd, papiergestremd_isnull=papiergestremd_isnull, papiertoegankelijk=papiertoegankelijk, papiertoegankelijk_isnull=papiertoegankelijk_isnull, papiervol=papiervol, papiervol_isnull=papiervol_isnull, postcode=postcode, postcode_in=postcode_in, postcode_isempty=postcode_isempty, postcode_isnull=postcode_isnull, postcode_like=postcode_like, postcode_not=postcode_not, restgestremd=restgestremd, restgestremd_isnull=restgestremd_isnull, resttoegankelijk=resttoegankelijk, resttoegankelijk_isnull=resttoegankelijk_isnull, restvol=restvol, restvol_isnull=restvol_isnull, straatnaam=straatnaam, straatnaam_in=straatnaam_in, straatnaam_isempty=straatnaam_isempty, straatnaam_isnull=straatnaam_isnull, straatnaam_like=straatnaam_like, straatnaam_not=straatnaam_not, tijd_waarneming=tijd_waarneming, tijd_waarneming_gt=tijd_waarneming_gt, tijd_waarneming_gte=tijd_waarneming_gte, tijd_waarneming_in=tijd_waarneming_in, tijd_waarneming_isnull=tijd_waarneming_isnull, tijd_waarneming_lt=tijd_waarneming_lt, tijd_waarneming_lte=tijd_waarneming_lte, tijd_waarneming_not=tijd_waarneming_not, type_waarneming=type_waarneming, type_waarneming_in=type_waarneming_in, type_waarneming_isempty=type_waarneming_isempty, type_waarneming_isnull=type_waarneming_isnull, type_waarneming_like=type_waarneming_like, type_waarneming_not=type_waarneming_not, veegvuil=veegvuil, veegvuil_isnull=veegvuil_isnull, waarde_handhaving=waarde_handhaving, waarde_handhaving_in=waarde_handhaving_in, waarde_handhaving_isempty=waarde_handhaving_isempty, waarde_handhaving_isnull=waarde_handhaving_isnull, waarde_handhaving_like=waarde_handhaving_like, waarde_handhaving_not=waarde_handhaving_not, waarnemer_rol=waarnemer_rol, waarnemer_rol_in=waarnemer_rol_in, waarnemer_rol_isempty=waarnemer_rol_isempty, waarnemer_rol_isnull=waarnemer_rol_isnull, waarnemer_rol_like=waarnemer_rol_like, waarnemer_rol_not=waarnemer_rol_not, zwerfafval=zwerfafval, zwerfafval_isnull=zwerfafval_isnull)

De Aanpak Bijplaatsingen (ABP) richt zich op afval dat op onjuiste wijze buiten wordt geplaatst. Momenteel wordt dit door de Gemeente Amsterdam op wijkniveau aangepakt via de ABP. Door communicatiemiddelen en interventies in te zetten rondom de meest vervuilde containerlocaties, neemt de netheid toe en daalt het aantal bijplaatsingen. Dit dataproduct bevat de registratie van bijplaatsingen zoals vastgelegd door de bevoegde medewerkers.

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalbijplaatsingen_list import PaginatedHuishoudelijkafvalbijplaatsingenList
from huishoudelijkafval_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.data.amsterdam.nl
# See configuration.py for a list of all supported configuration parameters.
configuration = huishoudelijkafval_api_client.Configuration(
    host = "https://api.data.amsterdam.nl"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
async with huishoudelijkafval_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = huishoudelijkafval_api_client.BijplaatsingenApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'bagNummeraanduiding' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    adres_type = 'adres_type_example' # str | Het type meetlocatie geeft aan om wat voor soort locatie het gaat. De locatie typen zijn er. Extra: De gemeten locatie bevond zich niet op de route, maar er is wel een meting van uitgevoerd. Bijvoorbeeld: een locatie die buiten de route ligt, heeft bijplaatsingen ernaast staan. Null: De gemeten locatie bevond zich op de route en werd direct gemeten zodra deze verscheen. Postponed: De meting van de locatie was eerder uitgesteld. Bijvoorbeeld, wanneer een locatie niet bereikbaar is, kun je deze uitstellen, waarna deze later opnieuw op de route verschijnt.  Forwarded: De gemeten locatie is bij het team binnengekomen omdat een ander team daar iets relevants had aangetroffen. Bijvoorbeeld: de werkbrigade vindt karton met adressen bij een locatie, vult aan het einde van het formulier in dat dit door het team gecontroleerd moet worden. De locatie wordt vervolgens toegevoegd aan de route.  (optional)
    adres_type_in = ['adres_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    adres_type_isempty = True # bool | Whether the field is empty or not. (optional)
    adres_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    adres_type_like = 'adres_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    adres_type_not = ['adres_type_not_example'] # List[str] | Exclude matches; text (optional)
    bag_nummeraanduiding_identificatie = 'bag_nummeraanduiding_identificatie_example' # str | De unieke aanduiding van een nummeraanduiding (optional)
    bag_nummeraanduiding_identificatie_in = ['bag_nummeraanduiding_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_nummeraanduiding_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_nummeraanduiding_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_nummeraanduiding_identificatie_like = 'bag_nummeraanduiding_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_nummeraanduiding_identificatie_not = ['bag_nummeraanduiding_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_openbareruimte_identificatie = 'bag_openbareruimte_identificatie_example' # str | De unieke aanduiding van een openbare ruimte (optional)
    bag_openbareruimte_identificatie_in = ['bag_openbareruimte_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_openbareruimte_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_openbareruimte_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_openbareruimte_identificatie_like = 'bag_openbareruimte_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_openbareruimte_identificatie_not = ['bag_openbareruimte_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_verblijfsobject_identificatie = 'bag_verblijfsobject_identificatie_example' # str | De unieke aanduiding van een verblijfsobject (optional)
    bag_verblijfsobject_identificatie_in = ['bag_verblijfsobject_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_verblijfsobject_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_verblijfsobject_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_verblijfsobject_identificatie_like = 'bag_verblijfsobject_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_verblijfsobject_identificatie_not = ['bag_verblijfsobject_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_woonplaats_identificatie = 'bag_woonplaats_identificatie_example' # str | De unieke aanduiding van een woonplaats (optional)
    bag_woonplaats_identificatie_in = ['bag_woonplaats_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_woonplaats_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_woonplaats_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_woonplaats_identificatie_like = 'bag_woonplaats_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_woonplaats_identificatie_not = ['bag_woonplaats_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bruingoed = True # bool | Aangetroffen afvalsoort (bruingoed) rondom de container(s) (optional)
    bruingoed_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
    containervies = True # bool | De uiterlijke toestand van de container(s). Container is vies en moet worden schoongemaakt (optional)
    containervies_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    crow_score = 'crow_score_example' # str | De score van CROW inspectie. A+: 0 stuks afval, A: <= 1 stuk, B: <= 3 stuks, C: <= 5 stuks, D: > 5 stuks (optional)
    crow_score_in = ['crow_score_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    crow_score_isempty = True # bool | Whether the field is empty or not. (optional)
    crow_score_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    crow_score_like = 'crow_score_like_example' # str | Matches text using wildcards (? and *). (optional)
    crow_score_not = ['crow_score_not_example'] # List[str] | Exclude matches; text (optional)
    datum_waarneming = '2013-10-20' # date | De datum waarop de waarneming is geregistreerd. (optional)
    datum_waarneming_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_waarneming_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_waarneming_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_waarneming_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_waarneming_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_waarneming_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_waarneming_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    dumpplek = True # bool | Het geeft aan of de locatie een dumpplek is. (optional)
    dumpplek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_code = 'gbd_buurt_code_example' # str | Unieke code (hierin zie je de Stadsdeel- en Wijkcode terug) (optional)
    gbd_buurt_code_in = ['gbd_buurt_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_code_like = 'gbd_buurt_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_code_not = ['gbd_buurt_code_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_stadsdeel_naam = 'gbd_stadsdeel_naam_example' # str | Naam van het stadsdeel waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). (optional)
    gbd_stadsdeel_naam_in = ['gbd_stadsdeel_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_stadsdeel_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_stadsdeel_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_stadsdeel_naam_like = 'gbd_stadsdeel_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_stadsdeel_naam_not = ['gbd_stadsdeel_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebruikers_rol = 'gebruikers_rol_example' # str | De rol van de gebruiker in de applicatie. (optional)
    gebruikers_rol_in = ['gebruikers_rol_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebruikers_rol_isempty = True # bool | Whether the field is empty or not. (optional)
    gebruikers_rol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebruikers_rol_like = 'gebruikers_rol_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebruikers_rol_not = ['gebruikers_rol_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de waarneming RD(epsg:28992) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    glas = True # bool | Aangetroffen afvalsoort (glas afval) rondom de container(s) (optional)
    glas_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    glasgestremd = True # bool | De glascontainer is gestremd (optional)
    glasgestremd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    glastoegankelijk = True # bool | De glascontainer is toegangelijk (optional)
    glastoegankelijk_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    glasvol = True # bool | De glascontainer is vol (optional)
    glasvol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    grof = True # bool | Aangetroffen afvalsoort (grofvuil) rondom de container(s) (optional)
    grof_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    grofvuildagen = 'grofvuildagen_example' # str | De waarde is 'true' of 'false' en geeft per dag aan of het waar of onwaar is. De eerste waarde correspondeert met maandag. (optional)
    grofvuildagen_in = ['grofvuildagen_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    grofvuildagen_isempty = True # bool | Whether the field is empty or not. (optional)
    grofvuildagen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    grofvuildagen_like = 'grofvuildagen_like_example' # str | Matches text using wildcards (? and *). (optional)
    grofvuildagen_not = ['grofvuildagen_not_example'] # List[str] | Exclude matches; text (optional)
    handhaving = True # bool | Er zijn items aangetroffen met adresgegevens en is er dus handhaving nodig (optional)
    handhaving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    huisvuil = True # bool | Aangetroffen afvalsoort (huisvuil) rondom de container(s) (optional)
    huisvuil_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id = 'id_example' # str | Unieke aanduiding van het record. (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    karton = True # bool | Aangetroffen afvalsoort (karton) rondom de container(s) (optional)
    karton_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    locatie_waarnemer = 'locatie_waarnemer_example' # str | De locatie (stadsdeel) vanwaar de waarnemer in het systeem is ingelogd. (optional)
    locatie_waarnemer_in = ['locatie_waarnemer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    locatie_waarnemer_isempty = True # bool | Whether the field is empty or not. (optional)
    locatie_waarnemer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    locatie_waarnemer_like = 'locatie_waarnemer_like_example' # str | Matches text using wildcards (? and *). (optional)
    locatie_waarnemer_not = ['locatie_waarnemer_not_example'] # List[str] | Exclude matches; text (optional)
    melding_door_collega_doorgezet = 'melding_door_collega_doorgezet_example' # str | Het geeft aan of de waarneming door een collega is doorgezet. (optional)
    melding_door_collega_doorgezet_in = ['melding_door_collega_doorgezet_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    melding_door_collega_doorgezet_isempty = True # bool | Whether the field is empty or not. (optional)
    melding_door_collega_doorgezet_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    melding_door_collega_doorgezet_like = 'melding_door_collega_doorgezet_like_example' # str | Matches text using wildcards (? and *). (optional)
    melding_door_collega_doorgezet_not = ['melding_door_collega_doorgezet_not_example'] # List[str] | Exclude matches; text (optional)
    naam_melding_doorgezet = 'naam_melding_doorgezet_example' # str | Soort doorgezette waarneming. (optional)
    naam_melding_doorgezet_in = ['naam_melding_doorgezet_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    naam_melding_doorgezet_isempty = True # bool | Whether the field is empty or not. (optional)
    naam_melding_doorgezet_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    naam_melding_doorgezet_like = 'naam_melding_doorgezet_like_example' # str | Matches text using wildcards (? and *). (optional)
    naam_melding_doorgezet_not = ['naam_melding_doorgezet_not_example'] # List[str] | Exclude matches; text (optional)
    overig = True # bool | Aangetroffen afvalsoort (overig) rondom de container(s) (optional)
    overig_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    papiergestremd = True # bool | De papiercontainer is gestremd (optional)
    papiergestremd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    papiertoegankelijk = True # bool | De papiercontainer is toegankelijk (optional)
    papiertoegankelijk_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    papiervol = True # bool | De papiercontainer is vol (optional)
    papiervol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    postcode = 'postcode_example' # str | De postcode van de locatie waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). (optional)
    postcode_in = ['postcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    postcode_isempty = True # bool | Whether the field is empty or not. (optional)
    postcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    postcode_like = 'postcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    postcode_not = ['postcode_not_example'] # List[str] | Exclude matches; text (optional)
    restgestremd = True # bool | De restcontainer is gestremd (optional)
    restgestremd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    resttoegankelijk = True # bool | De restcontainer is toegankelijk (optional)
    resttoegankelijk_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    restvol = True # bool | De restcontainer is vol (optional)
    restvol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    straatnaam = 'straatnaam_example' # str | De straat van de locatie waar de waarneming is geregistreerd (afgeleid op basis van de geometrie). (optional)
    straatnaam_in = ['straatnaam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    straatnaam_isempty = True # bool | Whether the field is empty or not. (optional)
    straatnaam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    straatnaam_like = 'straatnaam_like_example' # str | Matches text using wildcards (? and *). (optional)
    straatnaam_not = ['straatnaam_not_example'] # List[str] | Exclude matches; text (optional)
    tijd_waarneming = 'tijd_waarneming_example' # str | De tijdstip waarop de waarneming is geregistreerd. (optional)
    tijd_waarneming_gt = 'tijd_waarneming_gt_example' # str | Greater than; use hh:mm[:ss[.ms]] (optional)
    tijd_waarneming_gte = 'tijd_waarneming_gte_example' # str | Greater than or equal to; use hh:mm[:ss[.ms]] (optional)
    tijd_waarneming_in = ['tijd_waarneming_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    tijd_waarneming_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    tijd_waarneming_lt = 'tijd_waarneming_lt_example' # str | Less than; use hh:mm[:ss[.ms]] (optional)
    tijd_waarneming_lte = 'tijd_waarneming_lte_example' # str | Less than or equal to; use hh:mm[:ss[.ms]] (optional)
    tijd_waarneming_not = ['tijd_waarneming_not_example'] # List[str] | Exclude matches; use hh:mm[:ss[.ms]] (optional)
    type_waarneming = 'type_waarneming_example' # str | Geeft aan of de waarneming een CROW waarneming is. (optional)
    type_waarneming_in = ['type_waarneming_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    type_waarneming_isempty = True # bool | Whether the field is empty or not. (optional)
    type_waarneming_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    type_waarneming_like = 'type_waarneming_like_example' # str | Matches text using wildcards (? and *). (optional)
    type_waarneming_not = ['type_waarneming_not_example'] # List[str] | Exclude matches; text (optional)
    veegvuil = True # bool | Aangetroffen afvalsoort (veegvuil) rondom de container(s) (optional)
    veegvuil_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    waarde_handhaving = 'waarde_handhaving_example' # str | Hoe veel items met adresgegevens zijn er aangetroffen? (optional)
    waarde_handhaving_in = ['waarde_handhaving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    waarde_handhaving_isempty = True # bool | Whether the field is empty or not. (optional)
    waarde_handhaving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    waarde_handhaving_like = 'waarde_handhaving_like_example' # str | Matches text using wildcards (? and *). (optional)
    waarde_handhaving_not = ['waarde_handhaving_not_example'] # List[str] | Exclude matches; text (optional)
    waarnemer_rol = 'waarnemer_rol_example' # str | De rol van de melder (optional)
    waarnemer_rol_in = ['waarnemer_rol_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    waarnemer_rol_isempty = True # bool | Whether the field is empty or not. (optional)
    waarnemer_rol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    waarnemer_rol_like = 'waarnemer_rol_like_example' # str | Matches text using wildcards (? and *). (optional)
    waarnemer_rol_not = ['waarnemer_rol_not_example'] # List[str] | Exclude matches; text (optional)
    zwerfafval = True # bool | Aangetroffen afvalsoort (zwerfafval) rondom de container(s) (optional)
    zwerfafval_isnull = True # bool | Whether the field has a NULL value or not. (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_bijplaatsingen_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, adres_type=adres_type, adres_type_in=adres_type_in, adres_type_isempty=adres_type_isempty, adres_type_isnull=adres_type_isnull, adres_type_like=adres_type_like, adres_type_not=adres_type_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bag_woonplaats_identificatie=bag_woonplaats_identificatie, bag_woonplaats_identificatie_in=bag_woonplaats_identificatie_in, bag_woonplaats_identificatie_isempty=bag_woonplaats_identificatie_isempty, bag_woonplaats_identificatie_isnull=bag_woonplaats_identificatie_isnull, bag_woonplaats_identificatie_like=bag_woonplaats_identificatie_like, bag_woonplaats_identificatie_not=bag_woonplaats_identificatie_not, bruingoed=bruingoed, bruingoed_isnull=bruingoed_isnull, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, containervies=containervies, containervies_isnull=containervies_isnull, crow_score=crow_score, crow_score_in=crow_score_in, crow_score_isempty=crow_score_isempty, crow_score_isnull=crow_score_isnull, crow_score_like=crow_score_like, crow_score_not=crow_score_not, datum_waarneming=datum_waarneming, datum_waarneming_gt=datum_waarneming_gt, datum_waarneming_gte=datum_waarneming_gte, datum_waarneming_in=datum_waarneming_in, datum_waarneming_isnull=datum_waarneming_isnull, datum_waarneming_lt=datum_waarneming_lt, datum_waarneming_lte=datum_waarneming_lte, datum_waarneming_not=datum_waarneming_not, dumpplek=dumpplek, dumpplek_isnull=dumpplek_isnull, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, gbd_buurt_code=gbd_buurt_code, gbd_buurt_code_in=gbd_buurt_code_in, gbd_buurt_code_isempty=gbd_buurt_code_isempty, gbd_buurt_code_isnull=gbd_buurt_code_isnull, gbd_buurt_code_like=gbd_buurt_code_like, gbd_buurt_code_not=gbd_buurt_code_not, gbd_stadsdeel_naam=gbd_stadsdeel_naam, gbd_stadsdeel_naam_in=gbd_stadsdeel_naam_in, gbd_stadsdeel_naam_isempty=gbd_stadsdeel_naam_isempty, gbd_stadsdeel_naam_isnull=gbd_stadsdeel_naam_isnull, gbd_stadsdeel_naam_like=gbd_stadsdeel_naam_like, gbd_stadsdeel_naam_not=gbd_stadsdeel_naam_not, gebruikers_rol=gebruikers_rol, gebruikers_rol_in=gebruikers_rol_in, gebruikers_rol_isempty=gebruikers_rol_isempty, gebruikers_rol_isnull=gebruikers_rol_isnull, gebruikers_rol_like=gebruikers_rol_like, gebruikers_rol_not=gebruikers_rol_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, glas=glas, glas_isnull=glas_isnull, glasgestremd=glasgestremd, glasgestremd_isnull=glasgestremd_isnull, glastoegankelijk=glastoegankelijk, glastoegankelijk_isnull=glastoegankelijk_isnull, glasvol=glasvol, glasvol_isnull=glasvol_isnull, grof=grof, grof_isnull=grof_isnull, grofvuildagen=grofvuildagen, grofvuildagen_in=grofvuildagen_in, grofvuildagen_isempty=grofvuildagen_isempty, grofvuildagen_isnull=grofvuildagen_isnull, grofvuildagen_like=grofvuildagen_like, grofvuildagen_not=grofvuildagen_not, handhaving=handhaving, handhaving_isnull=handhaving_isnull, huisvuil=huisvuil, huisvuil_isnull=huisvuil_isnull, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, karton=karton, karton_isnull=karton_isnull, locatie_waarnemer=locatie_waarnemer, locatie_waarnemer_in=locatie_waarnemer_in, locatie_waarnemer_isempty=locatie_waarnemer_isempty, locatie_waarnemer_isnull=locatie_waarnemer_isnull, locatie_waarnemer_like=locatie_waarnemer_like, locatie_waarnemer_not=locatie_waarnemer_not, melding_door_collega_doorgezet=melding_door_collega_doorgezet, melding_door_collega_doorgezet_in=melding_door_collega_doorgezet_in, melding_door_collega_doorgezet_isempty=melding_door_collega_doorgezet_isempty, melding_door_collega_doorgezet_isnull=melding_door_collega_doorgezet_isnull, melding_door_collega_doorgezet_like=melding_door_collega_doorgezet_like, melding_door_collega_doorgezet_not=melding_door_collega_doorgezet_not, naam_melding_doorgezet=naam_melding_doorgezet, naam_melding_doorgezet_in=naam_melding_doorgezet_in, naam_melding_doorgezet_isempty=naam_melding_doorgezet_isempty, naam_melding_doorgezet_isnull=naam_melding_doorgezet_isnull, naam_melding_doorgezet_like=naam_melding_doorgezet_like, naam_melding_doorgezet_not=naam_melding_doorgezet_not, overig=overig, overig_isnull=overig_isnull, page=page, papiergestremd=papiergestremd, papiergestremd_isnull=papiergestremd_isnull, papiertoegankelijk=papiertoegankelijk, papiertoegankelijk_isnull=papiertoegankelijk_isnull, papiervol=papiervol, papiervol_isnull=papiervol_isnull, postcode=postcode, postcode_in=postcode_in, postcode_isempty=postcode_isempty, postcode_isnull=postcode_isnull, postcode_like=postcode_like, postcode_not=postcode_not, restgestremd=restgestremd, restgestremd_isnull=restgestremd_isnull, resttoegankelijk=resttoegankelijk, resttoegankelijk_isnull=resttoegankelijk_isnull, restvol=restvol, restvol_isnull=restvol_isnull, straatnaam=straatnaam, straatnaam_in=straatnaam_in, straatnaam_isempty=straatnaam_isempty, straatnaam_isnull=straatnaam_isnull, straatnaam_like=straatnaam_like, straatnaam_not=straatnaam_not, tijd_waarneming=tijd_waarneming, tijd_waarneming_gt=tijd_waarneming_gt, tijd_waarneming_gte=tijd_waarneming_gte, tijd_waarneming_in=tijd_waarneming_in, tijd_waarneming_isnull=tijd_waarneming_isnull, tijd_waarneming_lt=tijd_waarneming_lt, tijd_waarneming_lte=tijd_waarneming_lte, tijd_waarneming_not=tijd_waarneming_not, type_waarneming=type_waarneming, type_waarneming_in=type_waarneming_in, type_waarneming_isempty=type_waarneming_isempty, type_waarneming_isnull=type_waarneming_isnull, type_waarneming_like=type_waarneming_like, type_waarneming_not=type_waarneming_not, veegvuil=veegvuil, veegvuil_isnull=veegvuil_isnull, waarde_handhaving=waarde_handhaving, waarde_handhaving_in=waarde_handhaving_in, waarde_handhaving_isempty=waarde_handhaving_isempty, waarde_handhaving_isnull=waarde_handhaving_isnull, waarde_handhaving_like=waarde_handhaving_like, waarde_handhaving_not=waarde_handhaving_not, waarnemer_rol=waarnemer_rol, waarnemer_rol_in=waarnemer_rol_in, waarnemer_rol_isempty=waarnemer_rol_isempty, waarnemer_rol_isnull=waarnemer_rol_isnull, waarnemer_rol_like=waarnemer_rol_like, waarnemer_rol_not=waarnemer_rol_not, zwerfafval=zwerfafval, zwerfafval_isnull=zwerfafval_isnull)
        print("The response of BijplaatsingenApi->huishoudelijkafval_bijplaatsingen_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BijplaatsingenApi->huishoudelijkafval_bijplaatsingen_list2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept_crs** | **str**| Accept-Crs header for Geo queries | [optional] 
 **content_crs** | **str**| Content-Crs header for Geo queries | [optional] 
 **x_api_key** | **str**| Api Key for statistical purposes, not for authentication | [optional] 
 **count** | **bool**| Include a count of the total result set and the number of pages.Only works for responses that return a page. | [optional] 
 **expand** | **bool**| Allow to expand relations. | [optional] 
 **expand_scope** | **str**| Comma separated list of named relations to expand. | [optional] 
 **fields** | **str**| Comma-separated list of fields to display | [optional] 
 **format** | **str**| Select the export format | [optional] 
 **page_size** | **int**| Number of results to return per page. | [optional] 
 **sort** | **str**| Which field to use when ordering the results. | [optional] 
 **adres_type** | **str**| Het type meetlocatie geeft aan om wat voor soort locatie het gaat. De locatie typen zijn er. Extra: De gemeten locatie bevond zich niet op de route, maar er is wel een meting van uitgevoerd. Bijvoorbeeld: een locatie die buiten de route ligt, heeft bijplaatsingen ernaast staan. Null: De gemeten locatie bevond zich op de route en werd direct gemeten zodra deze verscheen. Postponed: De meting van de locatie was eerder uitgesteld. Bijvoorbeeld, wanneer een locatie niet bereikbaar is, kun je deze uitstellen, waarna deze later opnieuw op de route verschijnt.  Forwarded: De gemeten locatie is bij het team binnengekomen omdat een ander team daar iets relevants had aangetroffen. Bijvoorbeeld: de werkbrigade vindt karton met adressen bij een locatie, vult aan het einde van het formulier in dat dit door het team gecontroleerd moet worden. De locatie wordt vervolgens toegevoegd aan de route.  | [optional] 
 **adres_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **adres_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **adres_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **adres_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **adres_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_nummeraanduiding_identificatie** | **str**| De unieke aanduiding van een nummeraanduiding | [optional] 
 **bag_nummeraanduiding_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_nummeraanduiding_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_nummeraanduiding_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_nummeraanduiding_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_nummeraanduiding_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_openbareruimte_identificatie** | **str**| De unieke aanduiding van een openbare ruimte | [optional] 
 **bag_openbareruimte_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_openbareruimte_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_openbareruimte_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_openbareruimte_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_openbareruimte_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_verblijfsobject_identificatie** | **str**| De unieke aanduiding van een verblijfsobject | [optional] 
 **bag_verblijfsobject_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_verblijfsobject_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_verblijfsobject_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_verblijfsobject_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_verblijfsobject_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_woonplaats_identificatie** | **str**| De unieke aanduiding van een woonplaats | [optional] 
 **bag_woonplaats_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_woonplaats_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_woonplaats_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_woonplaats_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_woonplaats_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bruingoed** | **bool**| Aangetroffen afvalsoort (bruingoed) rondom de container(s) | [optional] 
 **bruingoed_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containervies** | **bool**| De uiterlijke toestand van de container(s). Container is vies en moet worden schoongemaakt | [optional] 
 **containervies_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **crow_score** | **str**| De score van CROW inspectie. A+: 0 stuks afval, A: &lt;&#x3D; 1 stuk, B: &lt;&#x3D; 3 stuks, C: &lt;&#x3D; 5 stuks, D: &gt; 5 stuks | [optional] 
 **crow_score_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **crow_score_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **crow_score_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **crow_score_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **crow_score_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_waarneming** | **date**| De datum waarop de waarneming is geregistreerd. | [optional] 
 **datum_waarneming_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_waarneming_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_waarneming_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_waarneming_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_waarneming_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_waarneming_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_waarneming_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **dumpplek** | **bool**| Het geeft aan of de locatie een dumpplek is. | [optional] 
 **dumpplek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_code** | **str**| Unieke code (hierin zie je de Stadsdeel- en Wijkcode terug) | [optional] 
 **gbd_buurt_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_stadsdeel_naam** | **str**| Naam van het stadsdeel waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). | [optional] 
 **gbd_stadsdeel_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_stadsdeel_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_stadsdeel_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_stadsdeel_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_stadsdeel_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebruikers_rol** | **str**| De rol van de gebruiker in de applicatie. | [optional] 
 **gebruikers_rol_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebruikers_rol_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebruikers_rol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebruikers_rol_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebruikers_rol_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de waarneming RD(epsg:28992) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **glas** | **bool**| Aangetroffen afvalsoort (glas afval) rondom de container(s) | [optional] 
 **glas_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **glasgestremd** | **bool**| De glascontainer is gestremd | [optional] 
 **glasgestremd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **glastoegankelijk** | **bool**| De glascontainer is toegangelijk | [optional] 
 **glastoegankelijk_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **glasvol** | **bool**| De glascontainer is vol | [optional] 
 **glasvol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **grof** | **bool**| Aangetroffen afvalsoort (grofvuil) rondom de container(s) | [optional] 
 **grof_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **grofvuildagen** | **str**| De waarde is &#39;true&#39; of &#39;false&#39; en geeft per dag aan of het waar of onwaar is. De eerste waarde correspondeert met maandag. | [optional] 
 **grofvuildagen_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **grofvuildagen_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **grofvuildagen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **grofvuildagen_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **grofvuildagen_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **handhaving** | **bool**| Er zijn items aangetroffen met adresgegevens en is er dus handhaving nodig | [optional] 
 **handhaving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **huisvuil** | **bool**| Aangetroffen afvalsoort (huisvuil) rondom de container(s) | [optional] 
 **huisvuil_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id** | **str**| Unieke aanduiding van het record. | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **karton** | **bool**| Aangetroffen afvalsoort (karton) rondom de container(s) | [optional] 
 **karton_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **locatie_waarnemer** | **str**| De locatie (stadsdeel) vanwaar de waarnemer in het systeem is ingelogd. | [optional] 
 **locatie_waarnemer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **locatie_waarnemer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **locatie_waarnemer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **locatie_waarnemer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **locatie_waarnemer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **melding_door_collega_doorgezet** | **str**| Het geeft aan of de waarneming door een collega is doorgezet. | [optional] 
 **melding_door_collega_doorgezet_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **melding_door_collega_doorgezet_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **melding_door_collega_doorgezet_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **melding_door_collega_doorgezet_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **melding_door_collega_doorgezet_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **naam_melding_doorgezet** | **str**| Soort doorgezette waarneming. | [optional] 
 **naam_melding_doorgezet_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **naam_melding_doorgezet_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **naam_melding_doorgezet_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **naam_melding_doorgezet_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **naam_melding_doorgezet_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **overig** | **bool**| Aangetroffen afvalsoort (overig) rondom de container(s) | [optional] 
 **overig_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **papiergestremd** | **bool**| De papiercontainer is gestremd | [optional] 
 **papiergestremd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **papiertoegankelijk** | **bool**| De papiercontainer is toegankelijk | [optional] 
 **papiertoegankelijk_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **papiervol** | **bool**| De papiercontainer is vol | [optional] 
 **papiervol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **postcode** | **str**| De postcode van de locatie waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). | [optional] 
 **postcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **postcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **postcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **postcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **postcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **restgestremd** | **bool**| De restcontainer is gestremd | [optional] 
 **restgestremd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **resttoegankelijk** | **bool**| De restcontainer is toegankelijk | [optional] 
 **resttoegankelijk_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **restvol** | **bool**| De restcontainer is vol | [optional] 
 **restvol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **straatnaam** | **str**| De straat van de locatie waar de waarneming is geregistreerd (afgeleid op basis van de geometrie). | [optional] 
 **straatnaam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **straatnaam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **straatnaam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **straatnaam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **straatnaam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **tijd_waarneming** | **str**| De tijdstip waarop de waarneming is geregistreerd. | [optional] 
 **tijd_waarneming_gt** | **str**| Greater than; use hh:mm[:ss[.ms]] | [optional] 
 **tijd_waarneming_gte** | **str**| Greater than or equal to; use hh:mm[:ss[.ms]] | [optional] 
 **tijd_waarneming_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **tijd_waarneming_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **tijd_waarneming_lt** | **str**| Less than; use hh:mm[:ss[.ms]] | [optional] 
 **tijd_waarneming_lte** | **str**| Less than or equal to; use hh:mm[:ss[.ms]] | [optional] 
 **tijd_waarneming_not** | [**List[str]**](str.md)| Exclude matches; use hh:mm[:ss[.ms]] | [optional] 
 **type_waarneming** | **str**| Geeft aan of de waarneming een CROW waarneming is. | [optional] 
 **type_waarneming_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **type_waarneming_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **type_waarneming_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **type_waarneming_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **type_waarneming_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **veegvuil** | **bool**| Aangetroffen afvalsoort (veegvuil) rondom de container(s) | [optional] 
 **veegvuil_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **waarde_handhaving** | **str**| Hoe veel items met adresgegevens zijn er aangetroffen? | [optional] 
 **waarde_handhaving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **waarde_handhaving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **waarde_handhaving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **waarde_handhaving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **waarde_handhaving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **waarnemer_rol** | **str**| De rol van de melder | [optional] 
 **waarnemer_rol_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **waarnemer_rol_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **waarnemer_rol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **waarnemer_rol_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **waarnemer_rol_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **zwerfafval** | **bool**| Aangetroffen afvalsoort (zwerfafval) rondom de container(s) | [optional] 
 **zwerfafval_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalbijplaatsingenList**](PaginatedHuishoudelijkafvalbijplaatsingenList.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/hal+json, text/csv, application/geo+json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **huishoudelijkafval_bijplaatsingen_retrieve2**
> Huishoudelijkafvalbijplaatsingen huishoudelijkafval_bijplaatsingen_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, adres_type=adres_type, adres_type_in=adres_type_in, adres_type_isempty=adres_type_isempty, adres_type_isnull=adres_type_isnull, adres_type_like=adres_type_like, adres_type_not=adres_type_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bag_woonplaats_identificatie=bag_woonplaats_identificatie, bag_woonplaats_identificatie_in=bag_woonplaats_identificatie_in, bag_woonplaats_identificatie_isempty=bag_woonplaats_identificatie_isempty, bag_woonplaats_identificatie_isnull=bag_woonplaats_identificatie_isnull, bag_woonplaats_identificatie_like=bag_woonplaats_identificatie_like, bag_woonplaats_identificatie_not=bag_woonplaats_identificatie_not, bruingoed=bruingoed, bruingoed_isnull=bruingoed_isnull, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, containervies=containervies, containervies_isnull=containervies_isnull, crow_score=crow_score, crow_score_in=crow_score_in, crow_score_isempty=crow_score_isempty, crow_score_isnull=crow_score_isnull, crow_score_like=crow_score_like, crow_score_not=crow_score_not, datum_waarneming=datum_waarneming, datum_waarneming_gt=datum_waarneming_gt, datum_waarneming_gte=datum_waarneming_gte, datum_waarneming_in=datum_waarneming_in, datum_waarneming_isnull=datum_waarneming_isnull, datum_waarneming_lt=datum_waarneming_lt, datum_waarneming_lte=datum_waarneming_lte, datum_waarneming_not=datum_waarneming_not, dumpplek=dumpplek, dumpplek_isnull=dumpplek_isnull, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, gbd_buurt_code=gbd_buurt_code, gbd_buurt_code_in=gbd_buurt_code_in, gbd_buurt_code_isempty=gbd_buurt_code_isempty, gbd_buurt_code_isnull=gbd_buurt_code_isnull, gbd_buurt_code_like=gbd_buurt_code_like, gbd_buurt_code_not=gbd_buurt_code_not, gbd_stadsdeel_naam=gbd_stadsdeel_naam, gbd_stadsdeel_naam_in=gbd_stadsdeel_naam_in, gbd_stadsdeel_naam_isempty=gbd_stadsdeel_naam_isempty, gbd_stadsdeel_naam_isnull=gbd_stadsdeel_naam_isnull, gbd_stadsdeel_naam_like=gbd_stadsdeel_naam_like, gbd_stadsdeel_naam_not=gbd_stadsdeel_naam_not, gebruikers_rol=gebruikers_rol, gebruikers_rol_in=gebruikers_rol_in, gebruikers_rol_isempty=gebruikers_rol_isempty, gebruikers_rol_isnull=gebruikers_rol_isnull, gebruikers_rol_like=gebruikers_rol_like, gebruikers_rol_not=gebruikers_rol_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, glas=glas, glas_isnull=glas_isnull, glasgestremd=glasgestremd, glasgestremd_isnull=glasgestremd_isnull, glastoegankelijk=glastoegankelijk, glastoegankelijk_isnull=glastoegankelijk_isnull, glasvol=glasvol, glasvol_isnull=glasvol_isnull, grof=grof, grof_isnull=grof_isnull, grofvuildagen=grofvuildagen, grofvuildagen_in=grofvuildagen_in, grofvuildagen_isempty=grofvuildagen_isempty, grofvuildagen_isnull=grofvuildagen_isnull, grofvuildagen_like=grofvuildagen_like, grofvuildagen_not=grofvuildagen_not, handhaving=handhaving, handhaving_isnull=handhaving_isnull, huisvuil=huisvuil, huisvuil_isnull=huisvuil_isnull, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, karton=karton, karton_isnull=karton_isnull, locatie_waarnemer=locatie_waarnemer, locatie_waarnemer_in=locatie_waarnemer_in, locatie_waarnemer_isempty=locatie_waarnemer_isempty, locatie_waarnemer_isnull=locatie_waarnemer_isnull, locatie_waarnemer_like=locatie_waarnemer_like, locatie_waarnemer_not=locatie_waarnemer_not, melding_door_collega_doorgezet=melding_door_collega_doorgezet, melding_door_collega_doorgezet_in=melding_door_collega_doorgezet_in, melding_door_collega_doorgezet_isempty=melding_door_collega_doorgezet_isempty, melding_door_collega_doorgezet_isnull=melding_door_collega_doorgezet_isnull, melding_door_collega_doorgezet_like=melding_door_collega_doorgezet_like, melding_door_collega_doorgezet_not=melding_door_collega_doorgezet_not, naam_melding_doorgezet=naam_melding_doorgezet, naam_melding_doorgezet_in=naam_melding_doorgezet_in, naam_melding_doorgezet_isempty=naam_melding_doorgezet_isempty, naam_melding_doorgezet_isnull=naam_melding_doorgezet_isnull, naam_melding_doorgezet_like=naam_melding_doorgezet_like, naam_melding_doorgezet_not=naam_melding_doorgezet_not, overig=overig, overig_isnull=overig_isnull, papiergestremd=papiergestremd, papiergestremd_isnull=papiergestremd_isnull, papiertoegankelijk=papiertoegankelijk, papiertoegankelijk_isnull=papiertoegankelijk_isnull, papiervol=papiervol, papiervol_isnull=papiervol_isnull, postcode=postcode, postcode_in=postcode_in, postcode_isempty=postcode_isempty, postcode_isnull=postcode_isnull, postcode_like=postcode_like, postcode_not=postcode_not, restgestremd=restgestremd, restgestremd_isnull=restgestremd_isnull, resttoegankelijk=resttoegankelijk, resttoegankelijk_isnull=resttoegankelijk_isnull, restvol=restvol, restvol_isnull=restvol_isnull, straatnaam=straatnaam, straatnaam_in=straatnaam_in, straatnaam_isempty=straatnaam_isempty, straatnaam_isnull=straatnaam_isnull, straatnaam_like=straatnaam_like, straatnaam_not=straatnaam_not, tijd_waarneming=tijd_waarneming, tijd_waarneming_gt=tijd_waarneming_gt, tijd_waarneming_gte=tijd_waarneming_gte, tijd_waarneming_in=tijd_waarneming_in, tijd_waarneming_isnull=tijd_waarneming_isnull, tijd_waarneming_lt=tijd_waarneming_lt, tijd_waarneming_lte=tijd_waarneming_lte, tijd_waarneming_not=tijd_waarneming_not, type_waarneming=type_waarneming, type_waarneming_in=type_waarneming_in, type_waarneming_isempty=type_waarneming_isempty, type_waarneming_isnull=type_waarneming_isnull, type_waarneming_like=type_waarneming_like, type_waarneming_not=type_waarneming_not, veegvuil=veegvuil, veegvuil_isnull=veegvuil_isnull, waarde_handhaving=waarde_handhaving, waarde_handhaving_in=waarde_handhaving_in, waarde_handhaving_isempty=waarde_handhaving_isempty, waarde_handhaving_isnull=waarde_handhaving_isnull, waarde_handhaving_like=waarde_handhaving_like, waarde_handhaving_not=waarde_handhaving_not, waarnemer_rol=waarnemer_rol, waarnemer_rol_in=waarnemer_rol_in, waarnemer_rol_isempty=waarnemer_rol_isempty, waarnemer_rol_isnull=waarnemer_rol_isnull, waarnemer_rol_like=waarnemer_rol_like, waarnemer_rol_not=waarnemer_rol_not, zwerfafval=zwerfafval, zwerfafval_isnull=zwerfafval_isnull)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalbijplaatsingen import Huishoudelijkafvalbijplaatsingen
from huishoudelijkafval_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.data.amsterdam.nl
# See configuration.py for a list of all supported configuration parameters.
configuration = huishoudelijkafval_api_client.Configuration(
    host = "https://api.data.amsterdam.nl"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
async with huishoudelijkafval_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = huishoudelijkafval_api_client.BijplaatsingenApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'bagNummeraanduiding' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    adres_type = 'adres_type_example' # str | Het type meetlocatie geeft aan om wat voor soort locatie het gaat. De locatie typen zijn er. Extra: De gemeten locatie bevond zich niet op de route, maar er is wel een meting van uitgevoerd. Bijvoorbeeld: een locatie die buiten de route ligt, heeft bijplaatsingen ernaast staan. Null: De gemeten locatie bevond zich op de route en werd direct gemeten zodra deze verscheen. Postponed: De meting van de locatie was eerder uitgesteld. Bijvoorbeeld, wanneer een locatie niet bereikbaar is, kun je deze uitstellen, waarna deze later opnieuw op de route verschijnt.  Forwarded: De gemeten locatie is bij het team binnengekomen omdat een ander team daar iets relevants had aangetroffen. Bijvoorbeeld: de werkbrigade vindt karton met adressen bij een locatie, vult aan het einde van het formulier in dat dit door het team gecontroleerd moet worden. De locatie wordt vervolgens toegevoegd aan de route.  (optional)
    adres_type_in = ['adres_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    adres_type_isempty = True # bool | Whether the field is empty or not. (optional)
    adres_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    adres_type_like = 'adres_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    adres_type_not = ['adres_type_not_example'] # List[str] | Exclude matches; text (optional)
    bag_nummeraanduiding_identificatie = 'bag_nummeraanduiding_identificatie_example' # str | De unieke aanduiding van een nummeraanduiding (optional)
    bag_nummeraanduiding_identificatie_in = ['bag_nummeraanduiding_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_nummeraanduiding_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_nummeraanduiding_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_nummeraanduiding_identificatie_like = 'bag_nummeraanduiding_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_nummeraanduiding_identificatie_not = ['bag_nummeraanduiding_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_openbareruimte_identificatie = 'bag_openbareruimte_identificatie_example' # str | De unieke aanduiding van een openbare ruimte (optional)
    bag_openbareruimte_identificatie_in = ['bag_openbareruimte_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_openbareruimte_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_openbareruimte_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_openbareruimte_identificatie_like = 'bag_openbareruimte_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_openbareruimte_identificatie_not = ['bag_openbareruimte_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_verblijfsobject_identificatie = 'bag_verblijfsobject_identificatie_example' # str | De unieke aanduiding van een verblijfsobject (optional)
    bag_verblijfsobject_identificatie_in = ['bag_verblijfsobject_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_verblijfsobject_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_verblijfsobject_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_verblijfsobject_identificatie_like = 'bag_verblijfsobject_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_verblijfsobject_identificatie_not = ['bag_verblijfsobject_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_woonplaats_identificatie = 'bag_woonplaats_identificatie_example' # str | De unieke aanduiding van een woonplaats (optional)
    bag_woonplaats_identificatie_in = ['bag_woonplaats_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_woonplaats_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_woonplaats_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_woonplaats_identificatie_like = 'bag_woonplaats_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_woonplaats_identificatie_not = ['bag_woonplaats_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bruingoed = True # bool | Aangetroffen afvalsoort (bruingoed) rondom de container(s) (optional)
    bruingoed_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
    containervies = True # bool | De uiterlijke toestand van de container(s). Container is vies en moet worden schoongemaakt (optional)
    containervies_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    crow_score = 'crow_score_example' # str | De score van CROW inspectie. A+: 0 stuks afval, A: <= 1 stuk, B: <= 3 stuks, C: <= 5 stuks, D: > 5 stuks (optional)
    crow_score_in = ['crow_score_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    crow_score_isempty = True # bool | Whether the field is empty or not. (optional)
    crow_score_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    crow_score_like = 'crow_score_like_example' # str | Matches text using wildcards (? and *). (optional)
    crow_score_not = ['crow_score_not_example'] # List[str] | Exclude matches; text (optional)
    datum_waarneming = '2013-10-20' # date | De datum waarop de waarneming is geregistreerd. (optional)
    datum_waarneming_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_waarneming_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_waarneming_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_waarneming_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_waarneming_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_waarneming_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_waarneming_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    dumpplek = True # bool | Het geeft aan of de locatie een dumpplek is. (optional)
    dumpplek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_code = 'gbd_buurt_code_example' # str | Unieke code (hierin zie je de Stadsdeel- en Wijkcode terug) (optional)
    gbd_buurt_code_in = ['gbd_buurt_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_code_like = 'gbd_buurt_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_code_not = ['gbd_buurt_code_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_stadsdeel_naam = 'gbd_stadsdeel_naam_example' # str | Naam van het stadsdeel waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). (optional)
    gbd_stadsdeel_naam_in = ['gbd_stadsdeel_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_stadsdeel_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_stadsdeel_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_stadsdeel_naam_like = 'gbd_stadsdeel_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_stadsdeel_naam_not = ['gbd_stadsdeel_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebruikers_rol = 'gebruikers_rol_example' # str | De rol van de gebruiker in de applicatie. (optional)
    gebruikers_rol_in = ['gebruikers_rol_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebruikers_rol_isempty = True # bool | Whether the field is empty or not. (optional)
    gebruikers_rol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebruikers_rol_like = 'gebruikers_rol_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebruikers_rol_not = ['gebruikers_rol_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de waarneming RD(epsg:28992) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    glas = True # bool | Aangetroffen afvalsoort (glas afval) rondom de container(s) (optional)
    glas_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    glasgestremd = True # bool | De glascontainer is gestremd (optional)
    glasgestremd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    glastoegankelijk = True # bool | De glascontainer is toegangelijk (optional)
    glastoegankelijk_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    glasvol = True # bool | De glascontainer is vol (optional)
    glasvol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    grof = True # bool | Aangetroffen afvalsoort (grofvuil) rondom de container(s) (optional)
    grof_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    grofvuildagen = 'grofvuildagen_example' # str | De waarde is 'true' of 'false' en geeft per dag aan of het waar of onwaar is. De eerste waarde correspondeert met maandag. (optional)
    grofvuildagen_in = ['grofvuildagen_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    grofvuildagen_isempty = True # bool | Whether the field is empty or not. (optional)
    grofvuildagen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    grofvuildagen_like = 'grofvuildagen_like_example' # str | Matches text using wildcards (? and *). (optional)
    grofvuildagen_not = ['grofvuildagen_not_example'] # List[str] | Exclude matches; text (optional)
    handhaving = True # bool | Er zijn items aangetroffen met adresgegevens en is er dus handhaving nodig (optional)
    handhaving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    huisvuil = True # bool | Aangetroffen afvalsoort (huisvuil) rondom de container(s) (optional)
    huisvuil_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id2 = 'id_example' # str | Unieke aanduiding van het record. (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    karton = True # bool | Aangetroffen afvalsoort (karton) rondom de container(s) (optional)
    karton_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    locatie_waarnemer = 'locatie_waarnemer_example' # str | De locatie (stadsdeel) vanwaar de waarnemer in het systeem is ingelogd. (optional)
    locatie_waarnemer_in = ['locatie_waarnemer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    locatie_waarnemer_isempty = True # bool | Whether the field is empty or not. (optional)
    locatie_waarnemer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    locatie_waarnemer_like = 'locatie_waarnemer_like_example' # str | Matches text using wildcards (? and *). (optional)
    locatie_waarnemer_not = ['locatie_waarnemer_not_example'] # List[str] | Exclude matches; text (optional)
    melding_door_collega_doorgezet = 'melding_door_collega_doorgezet_example' # str | Het geeft aan of de waarneming door een collega is doorgezet. (optional)
    melding_door_collega_doorgezet_in = ['melding_door_collega_doorgezet_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    melding_door_collega_doorgezet_isempty = True # bool | Whether the field is empty or not. (optional)
    melding_door_collega_doorgezet_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    melding_door_collega_doorgezet_like = 'melding_door_collega_doorgezet_like_example' # str | Matches text using wildcards (? and *). (optional)
    melding_door_collega_doorgezet_not = ['melding_door_collega_doorgezet_not_example'] # List[str] | Exclude matches; text (optional)
    naam_melding_doorgezet = 'naam_melding_doorgezet_example' # str | Soort doorgezette waarneming. (optional)
    naam_melding_doorgezet_in = ['naam_melding_doorgezet_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    naam_melding_doorgezet_isempty = True # bool | Whether the field is empty or not. (optional)
    naam_melding_doorgezet_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    naam_melding_doorgezet_like = 'naam_melding_doorgezet_like_example' # str | Matches text using wildcards (? and *). (optional)
    naam_melding_doorgezet_not = ['naam_melding_doorgezet_not_example'] # List[str] | Exclude matches; text (optional)
    overig = True # bool | Aangetroffen afvalsoort (overig) rondom de container(s) (optional)
    overig_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    papiergestremd = True # bool | De papiercontainer is gestremd (optional)
    papiergestremd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    papiertoegankelijk = True # bool | De papiercontainer is toegankelijk (optional)
    papiertoegankelijk_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    papiervol = True # bool | De papiercontainer is vol (optional)
    papiervol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    postcode = 'postcode_example' # str | De postcode van de locatie waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). (optional)
    postcode_in = ['postcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    postcode_isempty = True # bool | Whether the field is empty or not. (optional)
    postcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    postcode_like = 'postcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    postcode_not = ['postcode_not_example'] # List[str] | Exclude matches; text (optional)
    restgestremd = True # bool | De restcontainer is gestremd (optional)
    restgestremd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    resttoegankelijk = True # bool | De restcontainer is toegankelijk (optional)
    resttoegankelijk_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    restvol = True # bool | De restcontainer is vol (optional)
    restvol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    straatnaam = 'straatnaam_example' # str | De straat van de locatie waar de waarneming is geregistreerd (afgeleid op basis van de geometrie). (optional)
    straatnaam_in = ['straatnaam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    straatnaam_isempty = True # bool | Whether the field is empty or not. (optional)
    straatnaam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    straatnaam_like = 'straatnaam_like_example' # str | Matches text using wildcards (? and *). (optional)
    straatnaam_not = ['straatnaam_not_example'] # List[str] | Exclude matches; text (optional)
    tijd_waarneming = 'tijd_waarneming_example' # str | De tijdstip waarop de waarneming is geregistreerd. (optional)
    tijd_waarneming_gt = 'tijd_waarneming_gt_example' # str | Greater than; use hh:mm[:ss[.ms]] (optional)
    tijd_waarneming_gte = 'tijd_waarneming_gte_example' # str | Greater than or equal to; use hh:mm[:ss[.ms]] (optional)
    tijd_waarneming_in = ['tijd_waarneming_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    tijd_waarneming_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    tijd_waarneming_lt = 'tijd_waarneming_lt_example' # str | Less than; use hh:mm[:ss[.ms]] (optional)
    tijd_waarneming_lte = 'tijd_waarneming_lte_example' # str | Less than or equal to; use hh:mm[:ss[.ms]] (optional)
    tijd_waarneming_not = ['tijd_waarneming_not_example'] # List[str] | Exclude matches; use hh:mm[:ss[.ms]] (optional)
    type_waarneming = 'type_waarneming_example' # str | Geeft aan of de waarneming een CROW waarneming is. (optional)
    type_waarneming_in = ['type_waarneming_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    type_waarneming_isempty = True # bool | Whether the field is empty or not. (optional)
    type_waarneming_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    type_waarneming_like = 'type_waarneming_like_example' # str | Matches text using wildcards (? and *). (optional)
    type_waarneming_not = ['type_waarneming_not_example'] # List[str] | Exclude matches; text (optional)
    veegvuil = True # bool | Aangetroffen afvalsoort (veegvuil) rondom de container(s) (optional)
    veegvuil_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    waarde_handhaving = 'waarde_handhaving_example' # str | Hoe veel items met adresgegevens zijn er aangetroffen? (optional)
    waarde_handhaving_in = ['waarde_handhaving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    waarde_handhaving_isempty = True # bool | Whether the field is empty or not. (optional)
    waarde_handhaving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    waarde_handhaving_like = 'waarde_handhaving_like_example' # str | Matches text using wildcards (? and *). (optional)
    waarde_handhaving_not = ['waarde_handhaving_not_example'] # List[str] | Exclude matches; text (optional)
    waarnemer_rol = 'waarnemer_rol_example' # str | De rol van de melder (optional)
    waarnemer_rol_in = ['waarnemer_rol_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    waarnemer_rol_isempty = True # bool | Whether the field is empty or not. (optional)
    waarnemer_rol_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    waarnemer_rol_like = 'waarnemer_rol_like_example' # str | Matches text using wildcards (? and *). (optional)
    waarnemer_rol_not = ['waarnemer_rol_not_example'] # List[str] | Exclude matches; text (optional)
    zwerfafval = True # bool | Aangetroffen afvalsoort (zwerfafval) rondom de container(s) (optional)
    zwerfafval_isnull = True # bool | Whether the field has a NULL value or not. (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_bijplaatsingen_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, adres_type=adres_type, adres_type_in=adres_type_in, adres_type_isempty=adres_type_isempty, adres_type_isnull=adres_type_isnull, adres_type_like=adres_type_like, adres_type_not=adres_type_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bag_woonplaats_identificatie=bag_woonplaats_identificatie, bag_woonplaats_identificatie_in=bag_woonplaats_identificatie_in, bag_woonplaats_identificatie_isempty=bag_woonplaats_identificatie_isempty, bag_woonplaats_identificatie_isnull=bag_woonplaats_identificatie_isnull, bag_woonplaats_identificatie_like=bag_woonplaats_identificatie_like, bag_woonplaats_identificatie_not=bag_woonplaats_identificatie_not, bruingoed=bruingoed, bruingoed_isnull=bruingoed_isnull, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, containervies=containervies, containervies_isnull=containervies_isnull, crow_score=crow_score, crow_score_in=crow_score_in, crow_score_isempty=crow_score_isempty, crow_score_isnull=crow_score_isnull, crow_score_like=crow_score_like, crow_score_not=crow_score_not, datum_waarneming=datum_waarneming, datum_waarneming_gt=datum_waarneming_gt, datum_waarneming_gte=datum_waarneming_gte, datum_waarneming_in=datum_waarneming_in, datum_waarneming_isnull=datum_waarneming_isnull, datum_waarneming_lt=datum_waarneming_lt, datum_waarneming_lte=datum_waarneming_lte, datum_waarneming_not=datum_waarneming_not, dumpplek=dumpplek, dumpplek_isnull=dumpplek_isnull, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, gbd_buurt_code=gbd_buurt_code, gbd_buurt_code_in=gbd_buurt_code_in, gbd_buurt_code_isempty=gbd_buurt_code_isempty, gbd_buurt_code_isnull=gbd_buurt_code_isnull, gbd_buurt_code_like=gbd_buurt_code_like, gbd_buurt_code_not=gbd_buurt_code_not, gbd_stadsdeel_naam=gbd_stadsdeel_naam, gbd_stadsdeel_naam_in=gbd_stadsdeel_naam_in, gbd_stadsdeel_naam_isempty=gbd_stadsdeel_naam_isempty, gbd_stadsdeel_naam_isnull=gbd_stadsdeel_naam_isnull, gbd_stadsdeel_naam_like=gbd_stadsdeel_naam_like, gbd_stadsdeel_naam_not=gbd_stadsdeel_naam_not, gebruikers_rol=gebruikers_rol, gebruikers_rol_in=gebruikers_rol_in, gebruikers_rol_isempty=gebruikers_rol_isempty, gebruikers_rol_isnull=gebruikers_rol_isnull, gebruikers_rol_like=gebruikers_rol_like, gebruikers_rol_not=gebruikers_rol_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, glas=glas, glas_isnull=glas_isnull, glasgestremd=glasgestremd, glasgestremd_isnull=glasgestremd_isnull, glastoegankelijk=glastoegankelijk, glastoegankelijk_isnull=glastoegankelijk_isnull, glasvol=glasvol, glasvol_isnull=glasvol_isnull, grof=grof, grof_isnull=grof_isnull, grofvuildagen=grofvuildagen, grofvuildagen_in=grofvuildagen_in, grofvuildagen_isempty=grofvuildagen_isempty, grofvuildagen_isnull=grofvuildagen_isnull, grofvuildagen_like=grofvuildagen_like, grofvuildagen_not=grofvuildagen_not, handhaving=handhaving, handhaving_isnull=handhaving_isnull, huisvuil=huisvuil, huisvuil_isnull=huisvuil_isnull, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, karton=karton, karton_isnull=karton_isnull, locatie_waarnemer=locatie_waarnemer, locatie_waarnemer_in=locatie_waarnemer_in, locatie_waarnemer_isempty=locatie_waarnemer_isempty, locatie_waarnemer_isnull=locatie_waarnemer_isnull, locatie_waarnemer_like=locatie_waarnemer_like, locatie_waarnemer_not=locatie_waarnemer_not, melding_door_collega_doorgezet=melding_door_collega_doorgezet, melding_door_collega_doorgezet_in=melding_door_collega_doorgezet_in, melding_door_collega_doorgezet_isempty=melding_door_collega_doorgezet_isempty, melding_door_collega_doorgezet_isnull=melding_door_collega_doorgezet_isnull, melding_door_collega_doorgezet_like=melding_door_collega_doorgezet_like, melding_door_collega_doorgezet_not=melding_door_collega_doorgezet_not, naam_melding_doorgezet=naam_melding_doorgezet, naam_melding_doorgezet_in=naam_melding_doorgezet_in, naam_melding_doorgezet_isempty=naam_melding_doorgezet_isempty, naam_melding_doorgezet_isnull=naam_melding_doorgezet_isnull, naam_melding_doorgezet_like=naam_melding_doorgezet_like, naam_melding_doorgezet_not=naam_melding_doorgezet_not, overig=overig, overig_isnull=overig_isnull, papiergestremd=papiergestremd, papiergestremd_isnull=papiergestremd_isnull, papiertoegankelijk=papiertoegankelijk, papiertoegankelijk_isnull=papiertoegankelijk_isnull, papiervol=papiervol, papiervol_isnull=papiervol_isnull, postcode=postcode, postcode_in=postcode_in, postcode_isempty=postcode_isempty, postcode_isnull=postcode_isnull, postcode_like=postcode_like, postcode_not=postcode_not, restgestremd=restgestremd, restgestremd_isnull=restgestremd_isnull, resttoegankelijk=resttoegankelijk, resttoegankelijk_isnull=resttoegankelijk_isnull, restvol=restvol, restvol_isnull=restvol_isnull, straatnaam=straatnaam, straatnaam_in=straatnaam_in, straatnaam_isempty=straatnaam_isempty, straatnaam_isnull=straatnaam_isnull, straatnaam_like=straatnaam_like, straatnaam_not=straatnaam_not, tijd_waarneming=tijd_waarneming, tijd_waarneming_gt=tijd_waarneming_gt, tijd_waarneming_gte=tijd_waarneming_gte, tijd_waarneming_in=tijd_waarneming_in, tijd_waarneming_isnull=tijd_waarneming_isnull, tijd_waarneming_lt=tijd_waarneming_lt, tijd_waarneming_lte=tijd_waarneming_lte, tijd_waarneming_not=tijd_waarneming_not, type_waarneming=type_waarneming, type_waarneming_in=type_waarneming_in, type_waarneming_isempty=type_waarneming_isempty, type_waarneming_isnull=type_waarneming_isnull, type_waarneming_like=type_waarneming_like, type_waarneming_not=type_waarneming_not, veegvuil=veegvuil, veegvuil_isnull=veegvuil_isnull, waarde_handhaving=waarde_handhaving, waarde_handhaving_in=waarde_handhaving_in, waarde_handhaving_isempty=waarde_handhaving_isempty, waarde_handhaving_isnull=waarde_handhaving_isnull, waarde_handhaving_like=waarde_handhaving_like, waarde_handhaving_not=waarde_handhaving_not, waarnemer_rol=waarnemer_rol, waarnemer_rol_in=waarnemer_rol_in, waarnemer_rol_isempty=waarnemer_rol_isempty, waarnemer_rol_isnull=waarnemer_rol_isnull, waarnemer_rol_like=waarnemer_rol_like, waarnemer_rol_not=waarnemer_rol_not, zwerfafval=zwerfafval, zwerfafval_isnull=zwerfafval_isnull)
        print("The response of BijplaatsingenApi->huishoudelijkafval_bijplaatsingen_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BijplaatsingenApi->huishoudelijkafval_bijplaatsingen_retrieve2: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **accept_crs** | **str**| Accept-Crs header for Geo queries | [optional] 
 **content_crs** | **str**| Content-Crs header for Geo queries | [optional] 
 **x_api_key** | **str**| Api Key for statistical purposes, not for authentication | [optional] 
 **expand** | **bool**| Allow to expand relations. | [optional] 
 **expand_scope** | **str**| Comma separated list of named relations to expand. | [optional] 
 **fields** | **str**| Comma-separated list of fields to display | [optional] 
 **format** | **str**| Select the export format | [optional] 
 **sort** | **str**| Which field to use when ordering the results. | [optional] 
 **adres_type** | **str**| Het type meetlocatie geeft aan om wat voor soort locatie het gaat. De locatie typen zijn er. Extra: De gemeten locatie bevond zich niet op de route, maar er is wel een meting van uitgevoerd. Bijvoorbeeld: een locatie die buiten de route ligt, heeft bijplaatsingen ernaast staan. Null: De gemeten locatie bevond zich op de route en werd direct gemeten zodra deze verscheen. Postponed: De meting van de locatie was eerder uitgesteld. Bijvoorbeeld, wanneer een locatie niet bereikbaar is, kun je deze uitstellen, waarna deze later opnieuw op de route verschijnt.  Forwarded: De gemeten locatie is bij het team binnengekomen omdat een ander team daar iets relevants had aangetroffen. Bijvoorbeeld: de werkbrigade vindt karton met adressen bij een locatie, vult aan het einde van het formulier in dat dit door het team gecontroleerd moet worden. De locatie wordt vervolgens toegevoegd aan de route.  | [optional] 
 **adres_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **adres_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **adres_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **adres_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **adres_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_nummeraanduiding_identificatie** | **str**| De unieke aanduiding van een nummeraanduiding | [optional] 
 **bag_nummeraanduiding_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_nummeraanduiding_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_nummeraanduiding_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_nummeraanduiding_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_nummeraanduiding_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_openbareruimte_identificatie** | **str**| De unieke aanduiding van een openbare ruimte | [optional] 
 **bag_openbareruimte_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_openbareruimte_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_openbareruimte_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_openbareruimte_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_openbareruimte_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_verblijfsobject_identificatie** | **str**| De unieke aanduiding van een verblijfsobject | [optional] 
 **bag_verblijfsobject_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_verblijfsobject_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_verblijfsobject_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_verblijfsobject_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_verblijfsobject_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_woonplaats_identificatie** | **str**| De unieke aanduiding van een woonplaats | [optional] 
 **bag_woonplaats_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_woonplaats_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_woonplaats_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_woonplaats_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_woonplaats_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bruingoed** | **bool**| Aangetroffen afvalsoort (bruingoed) rondom de container(s) | [optional] 
 **bruingoed_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containervies** | **bool**| De uiterlijke toestand van de container(s). Container is vies en moet worden schoongemaakt | [optional] 
 **containervies_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **crow_score** | **str**| De score van CROW inspectie. A+: 0 stuks afval, A: &lt;&#x3D; 1 stuk, B: &lt;&#x3D; 3 stuks, C: &lt;&#x3D; 5 stuks, D: &gt; 5 stuks | [optional] 
 **crow_score_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **crow_score_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **crow_score_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **crow_score_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **crow_score_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_waarneming** | **date**| De datum waarop de waarneming is geregistreerd. | [optional] 
 **datum_waarneming_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_waarneming_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_waarneming_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_waarneming_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_waarneming_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_waarneming_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_waarneming_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **dumpplek** | **bool**| Het geeft aan of de locatie een dumpplek is. | [optional] 
 **dumpplek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_code** | **str**| Unieke code (hierin zie je de Stadsdeel- en Wijkcode terug) | [optional] 
 **gbd_buurt_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_stadsdeel_naam** | **str**| Naam van het stadsdeel waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). | [optional] 
 **gbd_stadsdeel_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_stadsdeel_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_stadsdeel_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_stadsdeel_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_stadsdeel_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebruikers_rol** | **str**| De rol van de gebruiker in de applicatie. | [optional] 
 **gebruikers_rol_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebruikers_rol_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebruikers_rol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebruikers_rol_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebruikers_rol_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de waarneming RD(epsg:28992) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **glas** | **bool**| Aangetroffen afvalsoort (glas afval) rondom de container(s) | [optional] 
 **glas_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **glasgestremd** | **bool**| De glascontainer is gestremd | [optional] 
 **glasgestremd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **glastoegankelijk** | **bool**| De glascontainer is toegangelijk | [optional] 
 **glastoegankelijk_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **glasvol** | **bool**| De glascontainer is vol | [optional] 
 **glasvol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **grof** | **bool**| Aangetroffen afvalsoort (grofvuil) rondom de container(s) | [optional] 
 **grof_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **grofvuildagen** | **str**| De waarde is &#39;true&#39; of &#39;false&#39; en geeft per dag aan of het waar of onwaar is. De eerste waarde correspondeert met maandag. | [optional] 
 **grofvuildagen_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **grofvuildagen_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **grofvuildagen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **grofvuildagen_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **grofvuildagen_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **handhaving** | **bool**| Er zijn items aangetroffen met adresgegevens en is er dus handhaving nodig | [optional] 
 **handhaving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **huisvuil** | **bool**| Aangetroffen afvalsoort (huisvuil) rondom de container(s) | [optional] 
 **huisvuil_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id2** | **str**| Unieke aanduiding van het record. | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **karton** | **bool**| Aangetroffen afvalsoort (karton) rondom de container(s) | [optional] 
 **karton_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **locatie_waarnemer** | **str**| De locatie (stadsdeel) vanwaar de waarnemer in het systeem is ingelogd. | [optional] 
 **locatie_waarnemer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **locatie_waarnemer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **locatie_waarnemer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **locatie_waarnemer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **locatie_waarnemer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **melding_door_collega_doorgezet** | **str**| Het geeft aan of de waarneming door een collega is doorgezet. | [optional] 
 **melding_door_collega_doorgezet_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **melding_door_collega_doorgezet_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **melding_door_collega_doorgezet_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **melding_door_collega_doorgezet_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **melding_door_collega_doorgezet_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **naam_melding_doorgezet** | **str**| Soort doorgezette waarneming. | [optional] 
 **naam_melding_doorgezet_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **naam_melding_doorgezet_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **naam_melding_doorgezet_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **naam_melding_doorgezet_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **naam_melding_doorgezet_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **overig** | **bool**| Aangetroffen afvalsoort (overig) rondom de container(s) | [optional] 
 **overig_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **papiergestremd** | **bool**| De papiercontainer is gestremd | [optional] 
 **papiergestremd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **papiertoegankelijk** | **bool**| De papiercontainer is toegankelijk | [optional] 
 **papiertoegankelijk_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **papiervol** | **bool**| De papiercontainer is vol | [optional] 
 **papiervol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **postcode** | **str**| De postcode van de locatie waar de waarneming is geregistreerd (afgeleid o.b.v. geometrie). | [optional] 
 **postcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **postcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **postcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **postcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **postcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **restgestremd** | **bool**| De restcontainer is gestremd | [optional] 
 **restgestremd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **resttoegankelijk** | **bool**| De restcontainer is toegankelijk | [optional] 
 **resttoegankelijk_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **restvol** | **bool**| De restcontainer is vol | [optional] 
 **restvol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **straatnaam** | **str**| De straat van de locatie waar de waarneming is geregistreerd (afgeleid op basis van de geometrie). | [optional] 
 **straatnaam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **straatnaam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **straatnaam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **straatnaam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **straatnaam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **tijd_waarneming** | **str**| De tijdstip waarop de waarneming is geregistreerd. | [optional] 
 **tijd_waarneming_gt** | **str**| Greater than; use hh:mm[:ss[.ms]] | [optional] 
 **tijd_waarneming_gte** | **str**| Greater than or equal to; use hh:mm[:ss[.ms]] | [optional] 
 **tijd_waarneming_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **tijd_waarneming_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **tijd_waarneming_lt** | **str**| Less than; use hh:mm[:ss[.ms]] | [optional] 
 **tijd_waarneming_lte** | **str**| Less than or equal to; use hh:mm[:ss[.ms]] | [optional] 
 **tijd_waarneming_not** | [**List[str]**](str.md)| Exclude matches; use hh:mm[:ss[.ms]] | [optional] 
 **type_waarneming** | **str**| Geeft aan of de waarneming een CROW waarneming is. | [optional] 
 **type_waarneming_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **type_waarneming_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **type_waarneming_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **type_waarneming_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **type_waarneming_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **veegvuil** | **bool**| Aangetroffen afvalsoort (veegvuil) rondom de container(s) | [optional] 
 **veegvuil_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **waarde_handhaving** | **str**| Hoe veel items met adresgegevens zijn er aangetroffen? | [optional] 
 **waarde_handhaving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **waarde_handhaving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **waarde_handhaving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **waarde_handhaving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **waarde_handhaving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **waarnemer_rol** | **str**| De rol van de melder | [optional] 
 **waarnemer_rol_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **waarnemer_rol_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **waarnemer_rol_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **waarnemer_rol_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **waarnemer_rol_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **zwerfafval** | **bool**| Aangetroffen afvalsoort (zwerfafval) rondom de container(s) | [optional] 
 **zwerfafval_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 

### Return type

[**Huishoudelijkafvalbijplaatsingen**](Huishoudelijkafvalbijplaatsingen.md)

### Authorization

[oauth2](../README.md#oauth2)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/hal+json, text/csv, application/geo+json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

