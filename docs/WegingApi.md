# huishoudelijkafval_api_client.WegingApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_weging_list2**](WegingApi.md#huishoudelijkafval_weging_list2) | **GET** /weging | 
[**huishoudelijkafval_weging_retrieve2**](WegingApi.md#huishoudelijkafval_weging_retrieve2) | **GET** /weging/{id} | 


# **huishoudelijkafval_weging_list2**
> PaginatedHuishoudelijkafvalwegingList huishoudelijkafval_weging_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bediening_code=bediening_code, bediening_code_gt=bediening_code_gt, bediening_code_gte=bediening_code_gte, bediening_code_in=bediening_code_in, bediening_code_isnull=bediening_code_isnull, bediening_code_lt=bediening_code_lt, bediening_code_lte=bediening_code_lte, bediening_code_not=bediening_code_not, bediening_omschrijving=bediening_omschrijving, bediening_omschrijving_in=bediening_omschrijving_in, bediening_omschrijving_isempty=bediening_omschrijving_isempty, bediening_omschrijving_isnull=bediening_omschrijving_isnull, bediening_omschrijving_like=bediening_omschrijving_like, bediening_omschrijving_not=bediening_omschrijving_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, cluster_subcluster_indicatie=cluster_subcluster_indicatie, cluster_subcluster_indicatie_isnull=cluster_subcluster_indicatie_isnull, datum_weging=datum_weging, datum_weging_gt=datum_weging_gt, datum_weging_gte=datum_weging_gte, datum_weging_in=datum_weging_in, datum_weging_isnull=datum_weging_isnull, datum_weging_lt=datum_weging_lt, datum_weging_lte=datum_weging_lte, datum_weging_not=datum_weging_not, eerste_weging=eerste_weging, eerste_weging_gt=eerste_weging_gt, eerste_weging_gte=eerste_weging_gte, eerste_weging_in=eerste_weging_in, eerste_weging_isnull=eerste_weging_isnull, eerste_weging_lt=eerste_weging_lt, eerste_weging_lte=eerste_weging_lte, eerste_weging_not=eerste_weging_not, fractie_code=fractie_code, fractie_code_gt=fractie_code_gt, fractie_code_gte=fractie_code_gte, fractie_code_in=fractie_code_in, fractie_code_isnull=fractie_code_isnull, fractie_code_lt=fractie_code_lt, fractie_code_lte=fractie_code_lte, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, locatienummer=locatienummer, locatienummer_in=locatienummer_in, locatienummer_isempty=locatienummer_isempty, locatienummer_isnull=locatienummer_isnull, locatienummer_like=locatienummer_like, locatienummer_not=locatienummer_not, netto_gewicht=netto_gewicht, netto_gewicht_gt=netto_gewicht_gt, netto_gewicht_gte=netto_gewicht_gte, netto_gewicht_in=netto_gewicht_in, netto_gewicht_isnull=netto_gewicht_isnull, netto_gewicht_lt=netto_gewicht_lt, netto_gewicht_lte=netto_gewicht_lte, netto_gewicht_not=netto_gewicht_not, page=page, tijdstip_weging=tijdstip_weging, tijdstip_weging_gt=tijdstip_weging_gt, tijdstip_weging_gte=tijdstip_weging_gte, tijdstip_weging_in=tijdstip_weging_in, tijdstip_weging_isnull=tijdstip_weging_isnull, tijdstip_weging_lt=tijdstip_weging_lt, tijdstip_weging_lte=tijdstip_weging_lte, tijdstip_weging_not=tijdstip_weging_not, tweede_weging=tweede_weging, tweede_weging_gt=tweede_weging_gt, tweede_weging_gte=tweede_weging_gte, tweede_weging_in=tweede_weging_in, tweede_weging_isnull=tweede_weging_isnull, tweede_weging_lt=tweede_weging_lt, tweede_weging_lte=tweede_weging_lte, tweede_weging_not=tweede_weging_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volgnummer=volgnummer, volgnummer_gt=volgnummer_gt, volgnummer_gte=volgnummer_gte, volgnummer_in=volgnummer_in, volgnummer_isnull=volgnummer_isnull, volgnummer_lt=volgnummer_lt, volgnummer_lte=volgnummer_lte, volgnummer_not=volgnummer_not, weegsysteem_id=weegsysteem_id, weegsysteem_id_gt=weegsysteem_id_gt, weegsysteem_id_gte=weegsysteem_id_gte, weegsysteem_id_in=weegsysteem_id_in, weegsysteem_id_isnull=weegsysteem_id_isnull, weegsysteem_id_lt=weegsysteem_id_lt, weegsysteem_id_lte=weegsysteem_id_lte, weegsysteem_id_not=weegsysteem_id_not, weegsysteem_omschrijving=weegsysteem_omschrijving, weegsysteem_omschrijving_in=weegsysteem_omschrijving_in, weegsysteem_omschrijving_isempty=weegsysteem_omschrijving_isempty, weegsysteem_omschrijving_isnull=weegsysteem_omschrijving_isnull, weegsysteem_omschrijving_like=weegsysteem_omschrijving_like, weegsysteem_omschrijving_not=weegsysteem_omschrijving_not, weging_kenteken=weging_kenteken, weging_kenteken_in=weging_kenteken_in, weging_kenteken_isempty=weging_kenteken_isempty, weging_kenteken_isnull=weging_kenteken_isnull, weging_kenteken_like=weging_kenteken_like, weging_kenteken_not=weging_kenteken_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalweging_list import PaginatedHuishoudelijkafvalwegingList
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
    api_instance = huishoudelijkafval_api_client.WegingApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'bagHoofdadresVerblijfsobject' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    bag_hoofdadres_verblijfsobject_identificatie = 'bag_hoofdadres_verblijfsobject_identificatie_example' # str | De unieke aanduiding van een verblijfsobject (optional)
    bag_hoofdadres_verblijfsobject_identificatie_in = ['bag_hoofdadres_verblijfsobject_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_hoofdadres_verblijfsobject_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_hoofdadres_verblijfsobject_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_hoofdadres_verblijfsobject_identificatie_like = 'bag_hoofdadres_verblijfsobject_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_hoofdadres_verblijfsobject_identificatie_not = ['bag_hoofdadres_verblijfsobject_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
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
    bediening_code = 56 # int | Code van de wijze waarop de bediening van de weging heeft plaatsgevonden. Mogelijke waarden: 0 - Handmatig, 1 - Automatisch, 3 - onbekend. (optional)
    bediening_code_gt = 56 # int | Greater than; number (optional)
    bediening_code_gte = 56 # int | Greater than or equal to; number (optional)
    bediening_code_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bediening_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bediening_code_lt = 56 # int | Less than; number (optional)
    bediening_code_lte = 56 # int | Less than or equal to; number (optional)
    bediening_code_not = [56] # List[int] | Exclude matches; number (optional)
    bediening_omschrijving = 'bediening_omschrijving_example' # str | Omschrijving van de wijze waarop de bediening van de weging heeft plaatsgevonden (optional)
    bediening_omschrijving_in = ['bediening_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bediening_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    bediening_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bediening_omschrijving_like = 'bediening_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    bediening_omschrijving_not = ['bediening_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_subcluster_indicatie = True # bool | Indicatie of het een cluster betreft dat is gesplitst door een weg (optional)
    cluster_subcluster_indicatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_weging = '2013-10-20' # date | Datum wanneer de weging is uitgevoerd (yyyy-mm-dd) (optional)
    datum_weging_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_weging_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_weging_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_weging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_weging_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_weging_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_weging_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    eerste_weging = 3.4 # float | Eerste weging container: gewicht vol in Kg (optional)
    eerste_weging_gt = 3.4 # float | Greater than; number (optional)
    eerste_weging_gte = 3.4 # float | Greater than or equal to; number (optional)
    eerste_weging_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    eerste_weging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    eerste_weging_lt = 3.4 # float | Less than; number (optional)
    eerste_weging_lte = 3.4 # float | Less than or equal to; number (optional)
    eerste_weging_not = [3.4] # List[float] | Exclude matches; number (optional)
    fractie_code = 56 # int | Code afvalfractie zoals door Welvaarts is aangeleverd, 1: Rest, 2: Glas, 3: Papier, 4: Plastic, 5: Textiel, 6: GFT, 7: Grof, 8: PMD, 9: Brood, -99: Onbekend (optional)
    fractie_code_gt = 56 # int | Greater than; number (optional)
    fractie_code_gte = 56 # int | Greater than or equal to; number (optional)
    fractie_code_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_code_lt = 56 # int | Less than; number (optional)
    fractie_code_lte = 56 # int | Less than or equal to; number (optional)
    fractie_code_not = [56] # List[int] | Exclude matches; number (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Omschrijving afvalfractie zoals door Welvaarts is aangeleverd (optional)
    fractie_omschrijving_in = ['fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_omschrijving_like = 'fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_omschrijving_not = ['fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Puntgeometrie in RD (epsg:28992) van de weging zoals door Welvaarts aangeleverd (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id = 'id_example' # str | Uniek identificerend kenmerk weging. Deze is per container vastgelegd (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    locatienummer = 'locatienummer_example' # str | Locatienummer (cluster) zoals door Welvaarts is aangeleverd (optional)
    locatienummer_in = ['locatienummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    locatienummer_isempty = True # bool | Whether the field is empty or not. (optional)
    locatienummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    locatienummer_like = 'locatienummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    locatienummer_not = ['locatienummer_not_example'] # List[str] | Exclude matches; text (optional)
    netto_gewicht = 3.4 # float | Netto gewicht van het ingezamelde afval van de container in Kg (optional)
    netto_gewicht_gt = 3.4 # float | Greater than; number (optional)
    netto_gewicht_gte = 3.4 # float | Greater than or equal to; number (optional)
    netto_gewicht_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    netto_gewicht_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    netto_gewicht_lt = 3.4 # float | Less than; number (optional)
    netto_gewicht_lte = 3.4 # float | Less than or equal to; number (optional)
    netto_gewicht_not = [3.4] # List[float] | Exclude matches; number (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    tijdstip_weging = 'tijdstip_weging_example' # str | Tijdstip wanneer de weging is uitgevoerd (HH24:MI:SS) (optional)
    tijdstip_weging_gt = 'tijdstip_weging_gt_example' # str | Greater than; use hh:mm[:ss[.ms]] (optional)
    tijdstip_weging_gte = 'tijdstip_weging_gte_example' # str | Greater than or equal to; use hh:mm[:ss[.ms]] (optional)
    tijdstip_weging_in = ['tijdstip_weging_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    tijdstip_weging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    tijdstip_weging_lt = 'tijdstip_weging_lt_example' # str | Less than; use hh:mm[:ss[.ms]] (optional)
    tijdstip_weging_lte = 'tijdstip_weging_lte_example' # str | Less than or equal to; use hh:mm[:ss[.ms]] (optional)
    tijdstip_weging_not = ['tijdstip_weging_not_example'] # List[str] | Exclude matches; use hh:mm[:ss[.ms]] (optional)
    tweede_weging = 3.4 # float | Tweede weging container: gewicht vol in Kg (optional)
    tweede_weging_gt = 3.4 # float | Greater than; number (optional)
    tweede_weging_gte = 3.4 # float | Greater than or equal to; number (optional)
    tweede_weging_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    tweede_weging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    tweede_weging_lt = 3.4 # float | Less than; number (optional)
    tweede_weging_lte = 3.4 # float | Less than or equal to; number (optional)
    tweede_weging_not = [3.4] # List[float] | Exclude matches; number (optional)
    verwijderd_dp = True # bool | Indicatie of het object verwijderd is bij de bronhouder (optional)
    verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volgnummer = 56 # int | Oplopende nummering wegingen per weegsysteem (optional)
    volgnummer_gt = 56 # int | Greater than; number (optional)
    volgnummer_gte = 56 # int | Greater than or equal to; number (optional)
    volgnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volgnummer_lt = 56 # int | Less than; number (optional)
    volgnummer_lte = 56 # int | Less than or equal to; number (optional)
    volgnummer_not = [56] # List[int] | Exclude matches; number (optional)
    weegsysteem_id = 56 # int | Identificerend kenmerk weegsysteem (behorend bij voertuig) (optional)
    weegsysteem_id_gt = 56 # int | Greater than; number (optional)
    weegsysteem_id_gte = 56 # int | Greater than or equal to; number (optional)
    weegsysteem_id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    weegsysteem_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    weegsysteem_id_lt = 56 # int | Less than; number (optional)
    weegsysteem_id_lte = 56 # int | Less than or equal to; number (optional)
    weegsysteem_id_not = [56] # List[int] | Exclude matches; number (optional)
    weegsysteem_omschrijving = 'weegsysteem_omschrijving_example' # str | Omschrijving van weegsysteem (optional)
    weegsysteem_omschrijving_in = ['weegsysteem_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    weegsysteem_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    weegsysteem_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    weegsysteem_omschrijving_like = 'weegsysteem_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    weegsysteem_omschrijving_not = ['weegsysteem_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    weging_kenteken = 'weging_kenteken_example' # str | Het kenteken van het voertuig (optional)
    weging_kenteken_in = ['weging_kenteken_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    weging_kenteken_isempty = True # bool | Whether the field is empty or not. (optional)
    weging_kenteken_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    weging_kenteken_like = 'weging_kenteken_like_example' # str | Matches text using wildcards (? and *). (optional)
    weging_kenteken_not = ['weging_kenteken_not_example'] # List[str] | Exclude matches; text (optional)
    wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop het object is gewijzigd (optional)
    wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_weging_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bediening_code=bediening_code, bediening_code_gt=bediening_code_gt, bediening_code_gte=bediening_code_gte, bediening_code_in=bediening_code_in, bediening_code_isnull=bediening_code_isnull, bediening_code_lt=bediening_code_lt, bediening_code_lte=bediening_code_lte, bediening_code_not=bediening_code_not, bediening_omschrijving=bediening_omschrijving, bediening_omschrijving_in=bediening_omschrijving_in, bediening_omschrijving_isempty=bediening_omschrijving_isempty, bediening_omschrijving_isnull=bediening_omschrijving_isnull, bediening_omschrijving_like=bediening_omschrijving_like, bediening_omschrijving_not=bediening_omschrijving_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, cluster_subcluster_indicatie=cluster_subcluster_indicatie, cluster_subcluster_indicatie_isnull=cluster_subcluster_indicatie_isnull, datum_weging=datum_weging, datum_weging_gt=datum_weging_gt, datum_weging_gte=datum_weging_gte, datum_weging_in=datum_weging_in, datum_weging_isnull=datum_weging_isnull, datum_weging_lt=datum_weging_lt, datum_weging_lte=datum_weging_lte, datum_weging_not=datum_weging_not, eerste_weging=eerste_weging, eerste_weging_gt=eerste_weging_gt, eerste_weging_gte=eerste_weging_gte, eerste_weging_in=eerste_weging_in, eerste_weging_isnull=eerste_weging_isnull, eerste_weging_lt=eerste_weging_lt, eerste_weging_lte=eerste_weging_lte, eerste_weging_not=eerste_weging_not, fractie_code=fractie_code, fractie_code_gt=fractie_code_gt, fractie_code_gte=fractie_code_gte, fractie_code_in=fractie_code_in, fractie_code_isnull=fractie_code_isnull, fractie_code_lt=fractie_code_lt, fractie_code_lte=fractie_code_lte, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, locatienummer=locatienummer, locatienummer_in=locatienummer_in, locatienummer_isempty=locatienummer_isempty, locatienummer_isnull=locatienummer_isnull, locatienummer_like=locatienummer_like, locatienummer_not=locatienummer_not, netto_gewicht=netto_gewicht, netto_gewicht_gt=netto_gewicht_gt, netto_gewicht_gte=netto_gewicht_gte, netto_gewicht_in=netto_gewicht_in, netto_gewicht_isnull=netto_gewicht_isnull, netto_gewicht_lt=netto_gewicht_lt, netto_gewicht_lte=netto_gewicht_lte, netto_gewicht_not=netto_gewicht_not, page=page, tijdstip_weging=tijdstip_weging, tijdstip_weging_gt=tijdstip_weging_gt, tijdstip_weging_gte=tijdstip_weging_gte, tijdstip_weging_in=tijdstip_weging_in, tijdstip_weging_isnull=tijdstip_weging_isnull, tijdstip_weging_lt=tijdstip_weging_lt, tijdstip_weging_lte=tijdstip_weging_lte, tijdstip_weging_not=tijdstip_weging_not, tweede_weging=tweede_weging, tweede_weging_gt=tweede_weging_gt, tweede_weging_gte=tweede_weging_gte, tweede_weging_in=tweede_weging_in, tweede_weging_isnull=tweede_weging_isnull, tweede_weging_lt=tweede_weging_lt, tweede_weging_lte=tweede_weging_lte, tweede_weging_not=tweede_weging_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volgnummer=volgnummer, volgnummer_gt=volgnummer_gt, volgnummer_gte=volgnummer_gte, volgnummer_in=volgnummer_in, volgnummer_isnull=volgnummer_isnull, volgnummer_lt=volgnummer_lt, volgnummer_lte=volgnummer_lte, volgnummer_not=volgnummer_not, weegsysteem_id=weegsysteem_id, weegsysteem_id_gt=weegsysteem_id_gt, weegsysteem_id_gte=weegsysteem_id_gte, weegsysteem_id_in=weegsysteem_id_in, weegsysteem_id_isnull=weegsysteem_id_isnull, weegsysteem_id_lt=weegsysteem_id_lt, weegsysteem_id_lte=weegsysteem_id_lte, weegsysteem_id_not=weegsysteem_id_not, weegsysteem_omschrijving=weegsysteem_omschrijving, weegsysteem_omschrijving_in=weegsysteem_omschrijving_in, weegsysteem_omschrijving_isempty=weegsysteem_omschrijving_isempty, weegsysteem_omschrijving_isnull=weegsysteem_omschrijving_isnull, weegsysteem_omschrijving_like=weegsysteem_omschrijving_like, weegsysteem_omschrijving_not=weegsysteem_omschrijving_not, weging_kenteken=weging_kenteken, weging_kenteken_in=weging_kenteken_in, weging_kenteken_isempty=weging_kenteken_isempty, weging_kenteken_isnull=weging_kenteken_isnull, weging_kenteken_like=weging_kenteken_like, weging_kenteken_not=weging_kenteken_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of WegingApi->huishoudelijkafval_weging_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WegingApi->huishoudelijkafval_weging_list2: %s\n" % e)
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
 **bag_hoofdadres_verblijfsobject_identificatie** | **str**| De unieke aanduiding van een verblijfsobject | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
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
 **bediening_code** | **int**| Code van de wijze waarop de bediening van de weging heeft plaatsgevonden. Mogelijke waarden: 0 - Handmatig, 1 - Automatisch, 3 - onbekend. | [optional] 
 **bediening_code_gt** | **int**| Greater than; number | [optional] 
 **bediening_code_gte** | **int**| Greater than or equal to; number | [optional] 
 **bediening_code_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bediening_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bediening_code_lt** | **int**| Less than; number | [optional] 
 **bediening_code_lte** | **int**| Less than or equal to; number | [optional] 
 **bediening_code_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **bediening_omschrijving** | **str**| Omschrijving van de wijze waarop de bediening van de weging heeft plaatsgevonden | [optional] 
 **bediening_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bediening_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bediening_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bediening_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bediening_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_subcluster_indicatie** | **bool**| Indicatie of het een cluster betreft dat is gesplitst door een weg | [optional] 
 **cluster_subcluster_indicatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_weging** | **date**| Datum wanneer de weging is uitgevoerd (yyyy-mm-dd) | [optional] 
 **datum_weging_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_weging_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_weging_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_weging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_weging_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_weging_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_weging_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **eerste_weging** | **float**| Eerste weging container: gewicht vol in Kg | [optional] 
 **eerste_weging_gt** | **float**| Greater than; number | [optional] 
 **eerste_weging_gte** | **float**| Greater than or equal to; number | [optional] 
 **eerste_weging_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **eerste_weging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **eerste_weging_lt** | **float**| Less than; number | [optional] 
 **eerste_weging_lte** | **float**| Less than or equal to; number | [optional] 
 **eerste_weging_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **fractie_code** | **int**| Code afvalfractie zoals door Welvaarts is aangeleverd, 1: Rest, 2: Glas, 3: Papier, 4: Plastic, 5: Textiel, 6: GFT, 7: Grof, 8: PMD, 9: Brood, -99: Onbekend | [optional] 
 **fractie_code_gt** | **int**| Greater than; number | [optional] 
 **fractie_code_gte** | **int**| Greater than or equal to; number | [optional] 
 **fractie_code_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_code_lt** | **int**| Less than; number | [optional] 
 **fractie_code_lte** | **int**| Less than or equal to; number | [optional] 
 **fractie_code_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **fractie_omschrijving** | **str**| Omschrijving afvalfractie zoals door Welvaarts is aangeleverd | [optional] 
 **fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Puntgeometrie in RD (epsg:28992) van de weging zoals door Welvaarts aangeleverd | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id** | **str**| Uniek identificerend kenmerk weging. Deze is per container vastgelegd | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **locatienummer** | **str**| Locatienummer (cluster) zoals door Welvaarts is aangeleverd | [optional] 
 **locatienummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **locatienummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **locatienummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **locatienummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **locatienummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **netto_gewicht** | **float**| Netto gewicht van het ingezamelde afval van de container in Kg | [optional] 
 **netto_gewicht_gt** | **float**| Greater than; number | [optional] 
 **netto_gewicht_gte** | **float**| Greater than or equal to; number | [optional] 
 **netto_gewicht_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **netto_gewicht_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **netto_gewicht_lt** | **float**| Less than; number | [optional] 
 **netto_gewicht_lte** | **float**| Less than or equal to; number | [optional] 
 **netto_gewicht_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **tijdstip_weging** | **str**| Tijdstip wanneer de weging is uitgevoerd (HH24:MI:SS) | [optional] 
 **tijdstip_weging_gt** | **str**| Greater than; use hh:mm[:ss[.ms]] | [optional] 
 **tijdstip_weging_gte** | **str**| Greater than or equal to; use hh:mm[:ss[.ms]] | [optional] 
 **tijdstip_weging_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **tijdstip_weging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **tijdstip_weging_lt** | **str**| Less than; use hh:mm[:ss[.ms]] | [optional] 
 **tijdstip_weging_lte** | **str**| Less than or equal to; use hh:mm[:ss[.ms]] | [optional] 
 **tijdstip_weging_not** | [**List[str]**](str.md)| Exclude matches; use hh:mm[:ss[.ms]] | [optional] 
 **tweede_weging** | **float**| Tweede weging container: gewicht vol in Kg | [optional] 
 **tweede_weging_gt** | **float**| Greater than; number | [optional] 
 **tweede_weging_gte** | **float**| Greater than or equal to; number | [optional] 
 **tweede_weging_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **tweede_weging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **tweede_weging_lt** | **float**| Less than; number | [optional] 
 **tweede_weging_lte** | **float**| Less than or equal to; number | [optional] 
 **tweede_weging_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **verwijderd_dp** | **bool**| Indicatie of het object verwijderd is bij de bronhouder | [optional] 
 **verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volgnummer** | **int**| Oplopende nummering wegingen per weegsysteem | [optional] 
 **volgnummer_gt** | **int**| Greater than; number | [optional] 
 **volgnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **volgnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volgnummer_lt** | **int**| Less than; number | [optional] 
 **volgnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **volgnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **weegsysteem_id** | **int**| Identificerend kenmerk weegsysteem (behorend bij voertuig) | [optional] 
 **weegsysteem_id_gt** | **int**| Greater than; number | [optional] 
 **weegsysteem_id_gte** | **int**| Greater than or equal to; number | [optional] 
 **weegsysteem_id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **weegsysteem_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **weegsysteem_id_lt** | **int**| Less than; number | [optional] 
 **weegsysteem_id_lte** | **int**| Less than or equal to; number | [optional] 
 **weegsysteem_id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **weegsysteem_omschrijving** | **str**| Omschrijving van weegsysteem | [optional] 
 **weegsysteem_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **weegsysteem_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **weegsysteem_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **weegsysteem_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **weegsysteem_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **weging_kenteken** | **str**| Het kenteken van het voertuig | [optional] 
 **weging_kenteken_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **weging_kenteken_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **weging_kenteken_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **weging_kenteken_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **weging_kenteken_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **wijzigingsdatum_dp** | **datetime**| Datum waarop het object is gewijzigd | [optional] 
 **wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalwegingList**](PaginatedHuishoudelijkafvalwegingList.md)

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

# **huishoudelijkafval_weging_retrieve2**
> Huishoudelijkafvalweging huishoudelijkafval_weging_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bediening_code=bediening_code, bediening_code_gt=bediening_code_gt, bediening_code_gte=bediening_code_gte, bediening_code_in=bediening_code_in, bediening_code_isnull=bediening_code_isnull, bediening_code_lt=bediening_code_lt, bediening_code_lte=bediening_code_lte, bediening_code_not=bediening_code_not, bediening_omschrijving=bediening_omschrijving, bediening_omschrijving_in=bediening_omschrijving_in, bediening_omschrijving_isempty=bediening_omschrijving_isempty, bediening_omschrijving_isnull=bediening_omschrijving_isnull, bediening_omschrijving_like=bediening_omschrijving_like, bediening_omschrijving_not=bediening_omschrijving_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, cluster_subcluster_indicatie=cluster_subcluster_indicatie, cluster_subcluster_indicatie_isnull=cluster_subcluster_indicatie_isnull, datum_weging=datum_weging, datum_weging_gt=datum_weging_gt, datum_weging_gte=datum_weging_gte, datum_weging_in=datum_weging_in, datum_weging_isnull=datum_weging_isnull, datum_weging_lt=datum_weging_lt, datum_weging_lte=datum_weging_lte, datum_weging_not=datum_weging_not, eerste_weging=eerste_weging, eerste_weging_gt=eerste_weging_gt, eerste_weging_gte=eerste_weging_gte, eerste_weging_in=eerste_weging_in, eerste_weging_isnull=eerste_weging_isnull, eerste_weging_lt=eerste_weging_lt, eerste_weging_lte=eerste_weging_lte, eerste_weging_not=eerste_weging_not, fractie_code=fractie_code, fractie_code_gt=fractie_code_gt, fractie_code_gte=fractie_code_gte, fractie_code_in=fractie_code_in, fractie_code_isnull=fractie_code_isnull, fractie_code_lt=fractie_code_lt, fractie_code_lte=fractie_code_lte, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, locatienummer=locatienummer, locatienummer_in=locatienummer_in, locatienummer_isempty=locatienummer_isempty, locatienummer_isnull=locatienummer_isnull, locatienummer_like=locatienummer_like, locatienummer_not=locatienummer_not, netto_gewicht=netto_gewicht, netto_gewicht_gt=netto_gewicht_gt, netto_gewicht_gte=netto_gewicht_gte, netto_gewicht_in=netto_gewicht_in, netto_gewicht_isnull=netto_gewicht_isnull, netto_gewicht_lt=netto_gewicht_lt, netto_gewicht_lte=netto_gewicht_lte, netto_gewicht_not=netto_gewicht_not, tijdstip_weging=tijdstip_weging, tijdstip_weging_gt=tijdstip_weging_gt, tijdstip_weging_gte=tijdstip_weging_gte, tijdstip_weging_in=tijdstip_weging_in, tijdstip_weging_isnull=tijdstip_weging_isnull, tijdstip_weging_lt=tijdstip_weging_lt, tijdstip_weging_lte=tijdstip_weging_lte, tijdstip_weging_not=tijdstip_weging_not, tweede_weging=tweede_weging, tweede_weging_gt=tweede_weging_gt, tweede_weging_gte=tweede_weging_gte, tweede_weging_in=tweede_weging_in, tweede_weging_isnull=tweede_weging_isnull, tweede_weging_lt=tweede_weging_lt, tweede_weging_lte=tweede_weging_lte, tweede_weging_not=tweede_weging_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volgnummer=volgnummer, volgnummer_gt=volgnummer_gt, volgnummer_gte=volgnummer_gte, volgnummer_in=volgnummer_in, volgnummer_isnull=volgnummer_isnull, volgnummer_lt=volgnummer_lt, volgnummer_lte=volgnummer_lte, volgnummer_not=volgnummer_not, weegsysteem_id=weegsysteem_id, weegsysteem_id_gt=weegsysteem_id_gt, weegsysteem_id_gte=weegsysteem_id_gte, weegsysteem_id_in=weegsysteem_id_in, weegsysteem_id_isnull=weegsysteem_id_isnull, weegsysteem_id_lt=weegsysteem_id_lt, weegsysteem_id_lte=weegsysteem_id_lte, weegsysteem_id_not=weegsysteem_id_not, weegsysteem_omschrijving=weegsysteem_omschrijving, weegsysteem_omschrijving_in=weegsysteem_omschrijving_in, weegsysteem_omschrijving_isempty=weegsysteem_omschrijving_isempty, weegsysteem_omschrijving_isnull=weegsysteem_omschrijving_isnull, weegsysteem_omschrijving_like=weegsysteem_omschrijving_like, weegsysteem_omschrijving_not=weegsysteem_omschrijving_not, weging_kenteken=weging_kenteken, weging_kenteken_in=weging_kenteken_in, weging_kenteken_isempty=weging_kenteken_isempty, weging_kenteken_isnull=weging_kenteken_isnull, weging_kenteken_like=weging_kenteken_like, weging_kenteken_not=weging_kenteken_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalweging import Huishoudelijkafvalweging
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
    api_instance = huishoudelijkafval_api_client.WegingApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'bagHoofdadresVerblijfsobject' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    bag_hoofdadres_verblijfsobject_identificatie = 'bag_hoofdadres_verblijfsobject_identificatie_example' # str | De unieke aanduiding van een verblijfsobject (optional)
    bag_hoofdadres_verblijfsobject_identificatie_in = ['bag_hoofdadres_verblijfsobject_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_hoofdadres_verblijfsobject_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_hoofdadres_verblijfsobject_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_hoofdadres_verblijfsobject_identificatie_like = 'bag_hoofdadres_verblijfsobject_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_hoofdadres_verblijfsobject_identificatie_not = ['bag_hoofdadres_verblijfsobject_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
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
    bediening_code = 56 # int | Code van de wijze waarop de bediening van de weging heeft plaatsgevonden. Mogelijke waarden: 0 - Handmatig, 1 - Automatisch, 3 - onbekend. (optional)
    bediening_code_gt = 56 # int | Greater than; number (optional)
    bediening_code_gte = 56 # int | Greater than or equal to; number (optional)
    bediening_code_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bediening_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bediening_code_lt = 56 # int | Less than; number (optional)
    bediening_code_lte = 56 # int | Less than or equal to; number (optional)
    bediening_code_not = [56] # List[int] | Exclude matches; number (optional)
    bediening_omschrijving = 'bediening_omschrijving_example' # str | Omschrijving van de wijze waarop de bediening van de weging heeft plaatsgevonden (optional)
    bediening_omschrijving_in = ['bediening_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bediening_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    bediening_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bediening_omschrijving_like = 'bediening_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    bediening_omschrijving_not = ['bediening_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_subcluster_indicatie = True # bool | Indicatie of het een cluster betreft dat is gesplitst door een weg (optional)
    cluster_subcluster_indicatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_weging = '2013-10-20' # date | Datum wanneer de weging is uitgevoerd (yyyy-mm-dd) (optional)
    datum_weging_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_weging_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_weging_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_weging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_weging_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_weging_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_weging_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    eerste_weging = 3.4 # float | Eerste weging container: gewicht vol in Kg (optional)
    eerste_weging_gt = 3.4 # float | Greater than; number (optional)
    eerste_weging_gte = 3.4 # float | Greater than or equal to; number (optional)
    eerste_weging_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    eerste_weging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    eerste_weging_lt = 3.4 # float | Less than; number (optional)
    eerste_weging_lte = 3.4 # float | Less than or equal to; number (optional)
    eerste_weging_not = [3.4] # List[float] | Exclude matches; number (optional)
    fractie_code = 56 # int | Code afvalfractie zoals door Welvaarts is aangeleverd, 1: Rest, 2: Glas, 3: Papier, 4: Plastic, 5: Textiel, 6: GFT, 7: Grof, 8: PMD, 9: Brood, -99: Onbekend (optional)
    fractie_code_gt = 56 # int | Greater than; number (optional)
    fractie_code_gte = 56 # int | Greater than or equal to; number (optional)
    fractie_code_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_code_lt = 56 # int | Less than; number (optional)
    fractie_code_lte = 56 # int | Less than or equal to; number (optional)
    fractie_code_not = [56] # List[int] | Exclude matches; number (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Omschrijving afvalfractie zoals door Welvaarts is aangeleverd (optional)
    fractie_omschrijving_in = ['fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_omschrijving_like = 'fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_omschrijving_not = ['fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Puntgeometrie in RD (epsg:28992) van de weging zoals door Welvaarts aangeleverd (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id2 = 'id_example' # str | Uniek identificerend kenmerk weging. Deze is per container vastgelegd (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    locatienummer = 'locatienummer_example' # str | Locatienummer (cluster) zoals door Welvaarts is aangeleverd (optional)
    locatienummer_in = ['locatienummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    locatienummer_isempty = True # bool | Whether the field is empty or not. (optional)
    locatienummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    locatienummer_like = 'locatienummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    locatienummer_not = ['locatienummer_not_example'] # List[str] | Exclude matches; text (optional)
    netto_gewicht = 3.4 # float | Netto gewicht van het ingezamelde afval van de container in Kg (optional)
    netto_gewicht_gt = 3.4 # float | Greater than; number (optional)
    netto_gewicht_gte = 3.4 # float | Greater than or equal to; number (optional)
    netto_gewicht_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    netto_gewicht_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    netto_gewicht_lt = 3.4 # float | Less than; number (optional)
    netto_gewicht_lte = 3.4 # float | Less than or equal to; number (optional)
    netto_gewicht_not = [3.4] # List[float] | Exclude matches; number (optional)
    tijdstip_weging = 'tijdstip_weging_example' # str | Tijdstip wanneer de weging is uitgevoerd (HH24:MI:SS) (optional)
    tijdstip_weging_gt = 'tijdstip_weging_gt_example' # str | Greater than; use hh:mm[:ss[.ms]] (optional)
    tijdstip_weging_gte = 'tijdstip_weging_gte_example' # str | Greater than or equal to; use hh:mm[:ss[.ms]] (optional)
    tijdstip_weging_in = ['tijdstip_weging_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    tijdstip_weging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    tijdstip_weging_lt = 'tijdstip_weging_lt_example' # str | Less than; use hh:mm[:ss[.ms]] (optional)
    tijdstip_weging_lte = 'tijdstip_weging_lte_example' # str | Less than or equal to; use hh:mm[:ss[.ms]] (optional)
    tijdstip_weging_not = ['tijdstip_weging_not_example'] # List[str] | Exclude matches; use hh:mm[:ss[.ms]] (optional)
    tweede_weging = 3.4 # float | Tweede weging container: gewicht vol in Kg (optional)
    tweede_weging_gt = 3.4 # float | Greater than; number (optional)
    tweede_weging_gte = 3.4 # float | Greater than or equal to; number (optional)
    tweede_weging_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    tweede_weging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    tweede_weging_lt = 3.4 # float | Less than; number (optional)
    tweede_weging_lte = 3.4 # float | Less than or equal to; number (optional)
    tweede_weging_not = [3.4] # List[float] | Exclude matches; number (optional)
    verwijderd_dp = True # bool | Indicatie of het object verwijderd is bij de bronhouder (optional)
    verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volgnummer = 56 # int | Oplopende nummering wegingen per weegsysteem (optional)
    volgnummer_gt = 56 # int | Greater than; number (optional)
    volgnummer_gte = 56 # int | Greater than or equal to; number (optional)
    volgnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volgnummer_lt = 56 # int | Less than; number (optional)
    volgnummer_lte = 56 # int | Less than or equal to; number (optional)
    volgnummer_not = [56] # List[int] | Exclude matches; number (optional)
    weegsysteem_id = 56 # int | Identificerend kenmerk weegsysteem (behorend bij voertuig) (optional)
    weegsysteem_id_gt = 56 # int | Greater than; number (optional)
    weegsysteem_id_gte = 56 # int | Greater than or equal to; number (optional)
    weegsysteem_id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    weegsysteem_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    weegsysteem_id_lt = 56 # int | Less than; number (optional)
    weegsysteem_id_lte = 56 # int | Less than or equal to; number (optional)
    weegsysteem_id_not = [56] # List[int] | Exclude matches; number (optional)
    weegsysteem_omschrijving = 'weegsysteem_omschrijving_example' # str | Omschrijving van weegsysteem (optional)
    weegsysteem_omschrijving_in = ['weegsysteem_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    weegsysteem_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    weegsysteem_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    weegsysteem_omschrijving_like = 'weegsysteem_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    weegsysteem_omschrijving_not = ['weegsysteem_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    weging_kenteken = 'weging_kenteken_example' # str | Het kenteken van het voertuig (optional)
    weging_kenteken_in = ['weging_kenteken_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    weging_kenteken_isempty = True # bool | Whether the field is empty or not. (optional)
    weging_kenteken_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    weging_kenteken_like = 'weging_kenteken_like_example' # str | Matches text using wildcards (? and *). (optional)
    weging_kenteken_not = ['weging_kenteken_not_example'] # List[str] | Exclude matches; text (optional)
    wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop het object is gewijzigd (optional)
    wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_weging_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bediening_code=bediening_code, bediening_code_gt=bediening_code_gt, bediening_code_gte=bediening_code_gte, bediening_code_in=bediening_code_in, bediening_code_isnull=bediening_code_isnull, bediening_code_lt=bediening_code_lt, bediening_code_lte=bediening_code_lte, bediening_code_not=bediening_code_not, bediening_omschrijving=bediening_omschrijving, bediening_omschrijving_in=bediening_omschrijving_in, bediening_omschrijving_isempty=bediening_omschrijving_isempty, bediening_omschrijving_isnull=bediening_omschrijving_isnull, bediening_omschrijving_like=bediening_omschrijving_like, bediening_omschrijving_not=bediening_omschrijving_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, cluster_subcluster_indicatie=cluster_subcluster_indicatie, cluster_subcluster_indicatie_isnull=cluster_subcluster_indicatie_isnull, datum_weging=datum_weging, datum_weging_gt=datum_weging_gt, datum_weging_gte=datum_weging_gte, datum_weging_in=datum_weging_in, datum_weging_isnull=datum_weging_isnull, datum_weging_lt=datum_weging_lt, datum_weging_lte=datum_weging_lte, datum_weging_not=datum_weging_not, eerste_weging=eerste_weging, eerste_weging_gt=eerste_weging_gt, eerste_weging_gte=eerste_weging_gte, eerste_weging_in=eerste_weging_in, eerste_weging_isnull=eerste_weging_isnull, eerste_weging_lt=eerste_weging_lt, eerste_weging_lte=eerste_weging_lte, eerste_weging_not=eerste_weging_not, fractie_code=fractie_code, fractie_code_gt=fractie_code_gt, fractie_code_gte=fractie_code_gte, fractie_code_in=fractie_code_in, fractie_code_isnull=fractie_code_isnull, fractie_code_lt=fractie_code_lt, fractie_code_lte=fractie_code_lte, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, locatienummer=locatienummer, locatienummer_in=locatienummer_in, locatienummer_isempty=locatienummer_isempty, locatienummer_isnull=locatienummer_isnull, locatienummer_like=locatienummer_like, locatienummer_not=locatienummer_not, netto_gewicht=netto_gewicht, netto_gewicht_gt=netto_gewicht_gt, netto_gewicht_gte=netto_gewicht_gte, netto_gewicht_in=netto_gewicht_in, netto_gewicht_isnull=netto_gewicht_isnull, netto_gewicht_lt=netto_gewicht_lt, netto_gewicht_lte=netto_gewicht_lte, netto_gewicht_not=netto_gewicht_not, tijdstip_weging=tijdstip_weging, tijdstip_weging_gt=tijdstip_weging_gt, tijdstip_weging_gte=tijdstip_weging_gte, tijdstip_weging_in=tijdstip_weging_in, tijdstip_weging_isnull=tijdstip_weging_isnull, tijdstip_weging_lt=tijdstip_weging_lt, tijdstip_weging_lte=tijdstip_weging_lte, tijdstip_weging_not=tijdstip_weging_not, tweede_weging=tweede_weging, tweede_weging_gt=tweede_weging_gt, tweede_weging_gte=tweede_weging_gte, tweede_weging_in=tweede_weging_in, tweede_weging_isnull=tweede_weging_isnull, tweede_weging_lt=tweede_weging_lt, tweede_weging_lte=tweede_weging_lte, tweede_weging_not=tweede_weging_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volgnummer=volgnummer, volgnummer_gt=volgnummer_gt, volgnummer_gte=volgnummer_gte, volgnummer_in=volgnummer_in, volgnummer_isnull=volgnummer_isnull, volgnummer_lt=volgnummer_lt, volgnummer_lte=volgnummer_lte, volgnummer_not=volgnummer_not, weegsysteem_id=weegsysteem_id, weegsysteem_id_gt=weegsysteem_id_gt, weegsysteem_id_gte=weegsysteem_id_gte, weegsysteem_id_in=weegsysteem_id_in, weegsysteem_id_isnull=weegsysteem_id_isnull, weegsysteem_id_lt=weegsysteem_id_lt, weegsysteem_id_lte=weegsysteem_id_lte, weegsysteem_id_not=weegsysteem_id_not, weegsysteem_omschrijving=weegsysteem_omschrijving, weegsysteem_omschrijving_in=weegsysteem_omschrijving_in, weegsysteem_omschrijving_isempty=weegsysteem_omschrijving_isempty, weegsysteem_omschrijving_isnull=weegsysteem_omschrijving_isnull, weegsysteem_omschrijving_like=weegsysteem_omschrijving_like, weegsysteem_omschrijving_not=weegsysteem_omschrijving_not, weging_kenteken=weging_kenteken, weging_kenteken_in=weging_kenteken_in, weging_kenteken_isempty=weging_kenteken_isempty, weging_kenteken_isnull=weging_kenteken_isnull, weging_kenteken_like=weging_kenteken_like, weging_kenteken_not=weging_kenteken_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of WegingApi->huishoudelijkafval_weging_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WegingApi->huishoudelijkafval_weging_retrieve2: %s\n" % e)
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
 **bag_hoofdadres_verblijfsobject_identificatie** | **str**| De unieke aanduiding van een verblijfsobject | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_hoofdadres_verblijfsobject_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
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
 **bediening_code** | **int**| Code van de wijze waarop de bediening van de weging heeft plaatsgevonden. Mogelijke waarden: 0 - Handmatig, 1 - Automatisch, 3 - onbekend. | [optional] 
 **bediening_code_gt** | **int**| Greater than; number | [optional] 
 **bediening_code_gte** | **int**| Greater than or equal to; number | [optional] 
 **bediening_code_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bediening_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bediening_code_lt** | **int**| Less than; number | [optional] 
 **bediening_code_lte** | **int**| Less than or equal to; number | [optional] 
 **bediening_code_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **bediening_omschrijving** | **str**| Omschrijving van de wijze waarop de bediening van de weging heeft plaatsgevonden | [optional] 
 **bediening_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bediening_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bediening_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bediening_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bediening_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_subcluster_indicatie** | **bool**| Indicatie of het een cluster betreft dat is gesplitst door een weg | [optional] 
 **cluster_subcluster_indicatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_weging** | **date**| Datum wanneer de weging is uitgevoerd (yyyy-mm-dd) | [optional] 
 **datum_weging_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_weging_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_weging_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_weging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_weging_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_weging_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_weging_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **eerste_weging** | **float**| Eerste weging container: gewicht vol in Kg | [optional] 
 **eerste_weging_gt** | **float**| Greater than; number | [optional] 
 **eerste_weging_gte** | **float**| Greater than or equal to; number | [optional] 
 **eerste_weging_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **eerste_weging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **eerste_weging_lt** | **float**| Less than; number | [optional] 
 **eerste_weging_lte** | **float**| Less than or equal to; number | [optional] 
 **eerste_weging_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **fractie_code** | **int**| Code afvalfractie zoals door Welvaarts is aangeleverd, 1: Rest, 2: Glas, 3: Papier, 4: Plastic, 5: Textiel, 6: GFT, 7: Grof, 8: PMD, 9: Brood, -99: Onbekend | [optional] 
 **fractie_code_gt** | **int**| Greater than; number | [optional] 
 **fractie_code_gte** | **int**| Greater than or equal to; number | [optional] 
 **fractie_code_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_code_lt** | **int**| Less than; number | [optional] 
 **fractie_code_lte** | **int**| Less than or equal to; number | [optional] 
 **fractie_code_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **fractie_omschrijving** | **str**| Omschrijving afvalfractie zoals door Welvaarts is aangeleverd | [optional] 
 **fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Puntgeometrie in RD (epsg:28992) van de weging zoals door Welvaarts aangeleverd | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id2** | **str**| Uniek identificerend kenmerk weging. Deze is per container vastgelegd | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **locatienummer** | **str**| Locatienummer (cluster) zoals door Welvaarts is aangeleverd | [optional] 
 **locatienummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **locatienummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **locatienummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **locatienummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **locatienummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **netto_gewicht** | **float**| Netto gewicht van het ingezamelde afval van de container in Kg | [optional] 
 **netto_gewicht_gt** | **float**| Greater than; number | [optional] 
 **netto_gewicht_gte** | **float**| Greater than or equal to; number | [optional] 
 **netto_gewicht_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **netto_gewicht_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **netto_gewicht_lt** | **float**| Less than; number | [optional] 
 **netto_gewicht_lte** | **float**| Less than or equal to; number | [optional] 
 **netto_gewicht_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **tijdstip_weging** | **str**| Tijdstip wanneer de weging is uitgevoerd (HH24:MI:SS) | [optional] 
 **tijdstip_weging_gt** | **str**| Greater than; use hh:mm[:ss[.ms]] | [optional] 
 **tijdstip_weging_gte** | **str**| Greater than or equal to; use hh:mm[:ss[.ms]] | [optional] 
 **tijdstip_weging_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **tijdstip_weging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **tijdstip_weging_lt** | **str**| Less than; use hh:mm[:ss[.ms]] | [optional] 
 **tijdstip_weging_lte** | **str**| Less than or equal to; use hh:mm[:ss[.ms]] | [optional] 
 **tijdstip_weging_not** | [**List[str]**](str.md)| Exclude matches; use hh:mm[:ss[.ms]] | [optional] 
 **tweede_weging** | **float**| Tweede weging container: gewicht vol in Kg | [optional] 
 **tweede_weging_gt** | **float**| Greater than; number | [optional] 
 **tweede_weging_gte** | **float**| Greater than or equal to; number | [optional] 
 **tweede_weging_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **tweede_weging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **tweede_weging_lt** | **float**| Less than; number | [optional] 
 **tweede_weging_lte** | **float**| Less than or equal to; number | [optional] 
 **tweede_weging_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **verwijderd_dp** | **bool**| Indicatie of het object verwijderd is bij de bronhouder | [optional] 
 **verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volgnummer** | **int**| Oplopende nummering wegingen per weegsysteem | [optional] 
 **volgnummer_gt** | **int**| Greater than; number | [optional] 
 **volgnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **volgnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volgnummer_lt** | **int**| Less than; number | [optional] 
 **volgnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **volgnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **weegsysteem_id** | **int**| Identificerend kenmerk weegsysteem (behorend bij voertuig) | [optional] 
 **weegsysteem_id_gt** | **int**| Greater than; number | [optional] 
 **weegsysteem_id_gte** | **int**| Greater than or equal to; number | [optional] 
 **weegsysteem_id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **weegsysteem_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **weegsysteem_id_lt** | **int**| Less than; number | [optional] 
 **weegsysteem_id_lte** | **int**| Less than or equal to; number | [optional] 
 **weegsysteem_id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **weegsysteem_omschrijving** | **str**| Omschrijving van weegsysteem | [optional] 
 **weegsysteem_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **weegsysteem_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **weegsysteem_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **weegsysteem_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **weegsysteem_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **weging_kenteken** | **str**| Het kenteken van het voertuig | [optional] 
 **weging_kenteken_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **weging_kenteken_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **weging_kenteken_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **weging_kenteken_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **weging_kenteken_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **wijzigingsdatum_dp** | **datetime**| Datum waarop het object is gewijzigd | [optional] 
 **wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**Huishoudelijkafvalweging**](Huishoudelijkafvalweging.md)

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

