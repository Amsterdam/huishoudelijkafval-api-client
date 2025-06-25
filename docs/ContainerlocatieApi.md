# huishoudelijkafval_api_client.ContainerlocatieApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_containerlocatie_list2**](ContainerlocatieApi.md#huishoudelijkafval_containerlocatie_list2) | **GET** /containerlocatie | 
[**huishoudelijkafval_containerlocatie_retrieve2**](ContainerlocatieApi.md#huishoudelijkafval_containerlocatie_retrieve2) | **GET** /containerlocatie/{id} | 


# **huishoudelijkafval_containerlocatie_list2**
> PaginatedHuishoudelijkafvalcontainerlocatieList huishoudelijkafval_containerlocatie_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bronadres=bronadres, bronadres_in=bronadres_in, bronadres_isempty=bronadres_isempty, bronadres_isnull=bronadres_isnull, bronadres_like=bronadres_like, bronadres_not=bronadres_not, containerlocatie_datum_wijziging=containerlocatie_datum_wijziging, containerlocatie_datum_wijziging_gt=containerlocatie_datum_wijziging_gt, containerlocatie_datum_wijziging_gte=containerlocatie_datum_wijziging_gte, containerlocatie_datum_wijziging_in=containerlocatie_datum_wijziging_in, containerlocatie_datum_wijziging_isnull=containerlocatie_datum_wijziging_isnull, containerlocatie_datum_wijziging_lt=containerlocatie_datum_wijziging_lt, containerlocatie_datum_wijziging_lte=containerlocatie_datum_wijziging_lte, containerlocatie_datum_wijziging_not=containerlocatie_datum_wijziging_not, containerlocatie_eigenaarschap=containerlocatie_eigenaarschap, containerlocatie_eigenaarschap_opmerking=containerlocatie_eigenaarschap_opmerking, containerlocatie_eigenaarschap_opmerking_in=containerlocatie_eigenaarschap_opmerking_in, containerlocatie_eigenaarschap_opmerking_isempty=containerlocatie_eigenaarschap_opmerking_isempty, containerlocatie_eigenaarschap_opmerking_isnull=containerlocatie_eigenaarschap_opmerking_isnull, containerlocatie_eigenaarschap_opmerking_like=containerlocatie_eigenaarschap_opmerking_like, containerlocatie_eigenaarschap_opmerking_not=containerlocatie_eigenaarschap_opmerking_not, containerlocatie_eigenaarschap_in=containerlocatie_eigenaarschap_in, containerlocatie_eigenaarschap_isempty=containerlocatie_eigenaarschap_isempty, containerlocatie_eigenaarschap_isnull=containerlocatie_eigenaarschap_isnull, containerlocatie_eigenaarschap_like=containerlocatie_eigenaarschap_like, containerlocatie_eigenaarschap_not=containerlocatie_eigenaarschap_not, containerlocatie_end_of_life=containerlocatie_end_of_life, containerlocatie_end_of_life_gt=containerlocatie_end_of_life_gt, containerlocatie_end_of_life_gte=containerlocatie_end_of_life_gte, containerlocatie_end_of_life_in=containerlocatie_end_of_life_in, containerlocatie_end_of_life_isnull=containerlocatie_end_of_life_isnull, containerlocatie_end_of_life_lt=containerlocatie_end_of_life_lt, containerlocatie_end_of_life_lte=containerlocatie_end_of_life_lte, containerlocatie_end_of_life_not=containerlocatie_end_of_life_not, containerlocatie_id_nummer=containerlocatie_id_nummer, containerlocatie_id_nummer_in=containerlocatie_id_nummer_in, containerlocatie_id_nummer_isempty=containerlocatie_id_nummer_isempty, containerlocatie_id_nummer_isnull=containerlocatie_id_nummer_isnull, containerlocatie_id_nummer_like=containerlocatie_id_nummer_like, containerlocatie_id_nummer_not=containerlocatie_id_nummer_not, containerlocatie_opmerking=containerlocatie_opmerking, containerlocatie_opmerking_in=containerlocatie_opmerking_in, containerlocatie_opmerking_isempty=containerlocatie_opmerking_isempty, containerlocatie_opmerking_isnull=containerlocatie_opmerking_isnull, containerlocatie_opmerking_like=containerlocatie_opmerking_like, containerlocatie_opmerking_not=containerlocatie_opmerking_not, containerlocatie_type_artikelcode=containerlocatie_type_artikelcode, containerlocatie_type_artikelcode_in=containerlocatie_type_artikelcode_in, containerlocatie_type_artikelcode_isempty=containerlocatie_type_artikelcode_isempty, containerlocatie_type_artikelcode_isnull=containerlocatie_type_artikelcode_isnull, containerlocatie_type_artikelcode_like=containerlocatie_type_artikelcode_like, containerlocatie_type_artikelcode_not=containerlocatie_type_artikelcode_not, containerlocatie_type_naam=containerlocatie_type_naam, containerlocatie_type_naam_in=containerlocatie_type_naam_in, containerlocatie_type_naam_isempty=containerlocatie_type_naam_isempty, containerlocatie_type_naam_isnull=containerlocatie_type_naam_isnull, containerlocatie_type_naam_like=containerlocatie_type_naam_like, containerlocatie_type_naam_not=containerlocatie_type_naam_not, datum_creatie=datum_creatie, datum_creatie_in=datum_creatie_in, datum_creatie_isempty=datum_creatie_isempty, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_like=datum_creatie_like, datum_creatie_not=datum_creatie_not, datum_einde_garantie=datum_einde_garantie, datum_einde_garantie_in=datum_einde_garantie_in, datum_einde_garantie_isempty=datum_einde_garantie_isempty, datum_einde_garantie_isnull=datum_einde_garantie_isnull, datum_einde_garantie_like=datum_einde_garantie_like, datum_einde_garantie_not=datum_einde_garantie_not, datum_operationeel=datum_operationeel, datum_operationeel_in=datum_operationeel_in, datum_operationeel_isempty=datum_operationeel_isempty, datum_operationeel_isnull=datum_operationeel_isnull, datum_operationeel_like=datum_operationeel_like, datum_operationeel_not=datum_operationeel_not, datum_oplevering=datum_oplevering, datum_oplevering_in=datum_oplevering_in, datum_oplevering_isempty=datum_oplevering_isempty, datum_oplevering_isnull=datum_oplevering_isnull, datum_oplevering_like=datum_oplevering_like, datum_oplevering_not=datum_oplevering_not, datum_plaatsing=datum_plaatsing, datum_plaatsing_in=datum_plaatsing_in, datum_plaatsing_isempty=datum_plaatsing_isempty, datum_plaatsing_isnull=datum_plaatsing_isnull, datum_plaatsing_like=datum_plaatsing_like, datum_plaatsing_not=datum_plaatsing_not, eigenaar_id=eigenaar_id, eigenaar_id_in=eigenaar_id_in, eigenaar_id_isempty=eigenaar_id_isempty, eigenaar_id_isnull=eigenaar_id_isnull, eigenaar_id_like=eigenaar_id_like, eigenaar_id_not=eigenaar_id_not, eigenaar_naam=eigenaar_naam, eigenaar_naam_in=eigenaar_naam_in, eigenaar_naam_isempty=eigenaar_naam_isempty, eigenaar_naam_isnull=eigenaar_naam_isnull, eigenaar_naam_like=eigenaar_naam_like, eigenaar_naam_not=eigenaar_naam_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, ind_bevat_container=ind_bevat_container, ind_bevat_container_isnull=ind_bevat_container_isnull, page=page, serienummer=serienummer, serienummer_in=serienummer_in, serienummer_isempty=serienummer_isempty, serienummer_isnull=serienummer_isnull, serienummer_like=serienummer_like, serienummer_not=serienummer_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalcontainerlocatie_list import PaginatedHuishoudelijkafvalcontainerlocatieList
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
    api_instance = huishoudelijkafval_api_client.ContainerlocatieApi(api_client)
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
    bronadres = 'bronadres_example' # str | Adres van de containerlocatie zoals die in bron geregistreerd is. (optional)
    bronadres_in = ['bronadres_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bronadres_isempty = True # bool | Whether the field is empty or not. (optional)
    bronadres_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bronadres_like = 'bronadres_like_example' # str | Matches text using wildcards (? and *). (optional)
    bronadres_not = ['bronadres_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_datum_wijziging = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop het object is gewijzigd. (optional)
    containerlocatie_datum_wijziging_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_datum_wijziging_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_datum_wijziging_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_datum_wijziging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_datum_wijziging_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_datum_wijziging_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_datum_wijziging_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_eigenaarschap = 'containerlocatie_eigenaarschap_example' # str | Soort eigenaarschap (optional)
    containerlocatie_eigenaarschap_opmerking = 'containerlocatie_eigenaarschap_opmerking_example' # str | Beschrijving van het type eigenaarschap. (optional)
    containerlocatie_eigenaarschap_opmerking_in = ['containerlocatie_eigenaarschap_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_eigenaarschap_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_eigenaarschap_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_eigenaarschap_opmerking_like = 'containerlocatie_eigenaarschap_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_eigenaarschap_opmerking_not = ['containerlocatie_eigenaarschap_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_eigenaarschap_in = ['containerlocatie_eigenaarschap_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_eigenaarschap_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_eigenaarschap_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_eigenaarschap_like = 'containerlocatie_eigenaarschap_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_eigenaarschap_not = ['containerlocatie_eigenaarschap_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_end_of_life = '2013-10-20' # date | Datum waarop het object het einde van zijn levenscyclus heeft bereikt. (optional)
    containerlocatie_end_of_life_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    containerlocatie_end_of_life_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    containerlocatie_end_of_life_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_end_of_life_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_end_of_life_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    containerlocatie_end_of_life_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    containerlocatie_end_of_life_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    containerlocatie_id_nummer = 'containerlocatie_id_nummer_example' # str | Definitie volgt nog (optional)
    containerlocatie_id_nummer_in = ['containerlocatie_id_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_id_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_id_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_id_nummer_like = 'containerlocatie_id_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_id_nummer_not = ['containerlocatie_id_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_opmerking = 'containerlocatie_opmerking_example' # str | Opmerking over het object. (optional)
    containerlocatie_opmerking_in = ['containerlocatie_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_opmerking_like = 'containerlocatie_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_opmerking_not = ['containerlocatie_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_type_artikelcode = 'containerlocatie_type_artikelcode_example' # str | Artikelcode van het containerlocatietype. (optional)
    containerlocatie_type_artikelcode_in = ['containerlocatie_type_artikelcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_type_artikelcode_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_type_artikelcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_type_artikelcode_like = 'containerlocatie_type_artikelcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_type_artikelcode_not = ['containerlocatie_type_artikelcode_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_type_naam = 'containerlocatie_type_naam_example' # str | Het type van de containerlocatie (optional)
    containerlocatie_type_naam_in = ['containerlocatie_type_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_type_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_type_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_type_naam_like = 'containerlocatie_type_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_type_naam_not = ['containerlocatie_type_naam_not_example'] # List[str] | Exclude matches; text (optional)
    datum_creatie = 'datum_creatie_example' # str | Datum waarop het object is gecreëerd in container management systeem (optional)
    datum_creatie_in = ['datum_creatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_creatie_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_creatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_creatie_like = 'datum_creatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_creatie_not = ['datum_creatie_not_example'] # List[str] | Exclude matches; text (optional)
    datum_einde_garantie = 'datum_einde_garantie_example' # str | Datum waarop de garantie verloopt (optional)
    datum_einde_garantie_in = ['datum_einde_garantie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_einde_garantie_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_einde_garantie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_einde_garantie_like = 'datum_einde_garantie_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_einde_garantie_not = ['datum_einde_garantie_not_example'] # List[str] | Exclude matches; text (optional)
    datum_operationeel = 'datum_operationeel_example' # str | Datum waarop het object is operationeel gezet (optional)
    datum_operationeel_in = ['datum_operationeel_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_operationeel_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_operationeel_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_operationeel_like = 'datum_operationeel_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_operationeel_not = ['datum_operationeel_not_example'] # List[str] | Exclude matches; text (optional)
    datum_oplevering = 'datum_oplevering_example' # str | Datum waarop het object is opgeleleverd (optional)
    datum_oplevering_in = ['datum_oplevering_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_oplevering_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_oplevering_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_oplevering_like = 'datum_oplevering_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_oplevering_not = ['datum_oplevering_not_example'] # List[str] | Exclude matches; text (optional)
    datum_plaatsing = 'datum_plaatsing_example' # str | Datum waarop het object op de locatie is geplaatst (optional)
    datum_plaatsing_in = ['datum_plaatsing_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_plaatsing_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_plaatsing_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_plaatsing_like = 'datum_plaatsing_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_plaatsing_not = ['datum_plaatsing_not_example'] # List[str] | Exclude matches; text (optional)
    eigenaar_id = 'eigenaar_id_example' # str | Identificerend kenmerk eigenaar (optional)
    eigenaar_id_in = ['eigenaar_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    eigenaar_id_isempty = True # bool | Whether the field is empty or not. (optional)
    eigenaar_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    eigenaar_id_like = 'eigenaar_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    eigenaar_id_not = ['eigenaar_id_not_example'] # List[str] | Exclude matches; text (optional)
    eigenaar_naam = 'eigenaar_naam_example' # str | Naam eigenaar (optional)
    eigenaar_naam_in = ['eigenaar_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    eigenaar_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    eigenaar_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    eigenaar_naam_like = 'eigenaar_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    eigenaar_naam_not = ['eigenaar_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de containerlocatie RD (epsg:28992) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id = 'id_example' # str | Identificerend kenmerk van de put waarin de container is geplaatst (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    ind_bevat_container = True # bool | Indicatie dat de containerlocatie een container bevat (optional)
    ind_bevat_container_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    serienummer = 'serienummer_example' # str | serienummer uitgegeven door de fabrikant (optional)
    serienummer_in = ['serienummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    serienummer_isempty = True # bool | Whether the field is empty or not. (optional)
    serienummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    serienummer_like = 'serienummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    serienummer_not = ['serienummer_not_example'] # List[str] | Exclude matches; text (optional)
    status = 56 # int | Status van de container, 0 - inactief, 1 - actief, 2 - gepland (optional)
    status_gt = 56 # int | Greater than; number (optional)
    status_gte = 56 # int | Greater than or equal to; number (optional)
    status_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_lt = 56 # int | Less than; number (optional)
    status_lte = 56 # int | Less than or equal to; number (optional)
    status_not = [56] # List[int] | Exclude matches; number (optional)
    verwijderd_dp = True # bool | Indicatie of het object verwijderd is bij de bronhouder (optional)
    verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop het object is gewijzigd (optional)
    wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_containerlocatie_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bronadres=bronadres, bronadres_in=bronadres_in, bronadres_isempty=bronadres_isempty, bronadres_isnull=bronadres_isnull, bronadres_like=bronadres_like, bronadres_not=bronadres_not, containerlocatie_datum_wijziging=containerlocatie_datum_wijziging, containerlocatie_datum_wijziging_gt=containerlocatie_datum_wijziging_gt, containerlocatie_datum_wijziging_gte=containerlocatie_datum_wijziging_gte, containerlocatie_datum_wijziging_in=containerlocatie_datum_wijziging_in, containerlocatie_datum_wijziging_isnull=containerlocatie_datum_wijziging_isnull, containerlocatie_datum_wijziging_lt=containerlocatie_datum_wijziging_lt, containerlocatie_datum_wijziging_lte=containerlocatie_datum_wijziging_lte, containerlocatie_datum_wijziging_not=containerlocatie_datum_wijziging_not, containerlocatie_eigenaarschap=containerlocatie_eigenaarschap, containerlocatie_eigenaarschap_opmerking=containerlocatie_eigenaarschap_opmerking, containerlocatie_eigenaarschap_opmerking_in=containerlocatie_eigenaarschap_opmerking_in, containerlocatie_eigenaarschap_opmerking_isempty=containerlocatie_eigenaarschap_opmerking_isempty, containerlocatie_eigenaarschap_opmerking_isnull=containerlocatie_eigenaarschap_opmerking_isnull, containerlocatie_eigenaarschap_opmerking_like=containerlocatie_eigenaarschap_opmerking_like, containerlocatie_eigenaarschap_opmerking_not=containerlocatie_eigenaarschap_opmerking_not, containerlocatie_eigenaarschap_in=containerlocatie_eigenaarschap_in, containerlocatie_eigenaarschap_isempty=containerlocatie_eigenaarschap_isempty, containerlocatie_eigenaarschap_isnull=containerlocatie_eigenaarschap_isnull, containerlocatie_eigenaarschap_like=containerlocatie_eigenaarschap_like, containerlocatie_eigenaarschap_not=containerlocatie_eigenaarschap_not, containerlocatie_end_of_life=containerlocatie_end_of_life, containerlocatie_end_of_life_gt=containerlocatie_end_of_life_gt, containerlocatie_end_of_life_gte=containerlocatie_end_of_life_gte, containerlocatie_end_of_life_in=containerlocatie_end_of_life_in, containerlocatie_end_of_life_isnull=containerlocatie_end_of_life_isnull, containerlocatie_end_of_life_lt=containerlocatie_end_of_life_lt, containerlocatie_end_of_life_lte=containerlocatie_end_of_life_lte, containerlocatie_end_of_life_not=containerlocatie_end_of_life_not, containerlocatie_id_nummer=containerlocatie_id_nummer, containerlocatie_id_nummer_in=containerlocatie_id_nummer_in, containerlocatie_id_nummer_isempty=containerlocatie_id_nummer_isempty, containerlocatie_id_nummer_isnull=containerlocatie_id_nummer_isnull, containerlocatie_id_nummer_like=containerlocatie_id_nummer_like, containerlocatie_id_nummer_not=containerlocatie_id_nummer_not, containerlocatie_opmerking=containerlocatie_opmerking, containerlocatie_opmerking_in=containerlocatie_opmerking_in, containerlocatie_opmerking_isempty=containerlocatie_opmerking_isempty, containerlocatie_opmerking_isnull=containerlocatie_opmerking_isnull, containerlocatie_opmerking_like=containerlocatie_opmerking_like, containerlocatie_opmerking_not=containerlocatie_opmerking_not, containerlocatie_type_artikelcode=containerlocatie_type_artikelcode, containerlocatie_type_artikelcode_in=containerlocatie_type_artikelcode_in, containerlocatie_type_artikelcode_isempty=containerlocatie_type_artikelcode_isempty, containerlocatie_type_artikelcode_isnull=containerlocatie_type_artikelcode_isnull, containerlocatie_type_artikelcode_like=containerlocatie_type_artikelcode_like, containerlocatie_type_artikelcode_not=containerlocatie_type_artikelcode_not, containerlocatie_type_naam=containerlocatie_type_naam, containerlocatie_type_naam_in=containerlocatie_type_naam_in, containerlocatie_type_naam_isempty=containerlocatie_type_naam_isempty, containerlocatie_type_naam_isnull=containerlocatie_type_naam_isnull, containerlocatie_type_naam_like=containerlocatie_type_naam_like, containerlocatie_type_naam_not=containerlocatie_type_naam_not, datum_creatie=datum_creatie, datum_creatie_in=datum_creatie_in, datum_creatie_isempty=datum_creatie_isempty, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_like=datum_creatie_like, datum_creatie_not=datum_creatie_not, datum_einde_garantie=datum_einde_garantie, datum_einde_garantie_in=datum_einde_garantie_in, datum_einde_garantie_isempty=datum_einde_garantie_isempty, datum_einde_garantie_isnull=datum_einde_garantie_isnull, datum_einde_garantie_like=datum_einde_garantie_like, datum_einde_garantie_not=datum_einde_garantie_not, datum_operationeel=datum_operationeel, datum_operationeel_in=datum_operationeel_in, datum_operationeel_isempty=datum_operationeel_isempty, datum_operationeel_isnull=datum_operationeel_isnull, datum_operationeel_like=datum_operationeel_like, datum_operationeel_not=datum_operationeel_not, datum_oplevering=datum_oplevering, datum_oplevering_in=datum_oplevering_in, datum_oplevering_isempty=datum_oplevering_isempty, datum_oplevering_isnull=datum_oplevering_isnull, datum_oplevering_like=datum_oplevering_like, datum_oplevering_not=datum_oplevering_not, datum_plaatsing=datum_plaatsing, datum_plaatsing_in=datum_plaatsing_in, datum_plaatsing_isempty=datum_plaatsing_isempty, datum_plaatsing_isnull=datum_plaatsing_isnull, datum_plaatsing_like=datum_plaatsing_like, datum_plaatsing_not=datum_plaatsing_not, eigenaar_id=eigenaar_id, eigenaar_id_in=eigenaar_id_in, eigenaar_id_isempty=eigenaar_id_isempty, eigenaar_id_isnull=eigenaar_id_isnull, eigenaar_id_like=eigenaar_id_like, eigenaar_id_not=eigenaar_id_not, eigenaar_naam=eigenaar_naam, eigenaar_naam_in=eigenaar_naam_in, eigenaar_naam_isempty=eigenaar_naam_isempty, eigenaar_naam_isnull=eigenaar_naam_isnull, eigenaar_naam_like=eigenaar_naam_like, eigenaar_naam_not=eigenaar_naam_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, ind_bevat_container=ind_bevat_container, ind_bevat_container_isnull=ind_bevat_container_isnull, page=page, serienummer=serienummer, serienummer_in=serienummer_in, serienummer_isempty=serienummer_isempty, serienummer_isnull=serienummer_isnull, serienummer_like=serienummer_like, serienummer_not=serienummer_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ContainerlocatieApi->huishoudelijkafval_containerlocatie_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContainerlocatieApi->huishoudelijkafval_containerlocatie_list2: %s\n" % e)
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
 **bronadres** | **str**| Adres van de containerlocatie zoals die in bron geregistreerd is. | [optional] 
 **bronadres_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bronadres_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bronadres_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bronadres_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bronadres_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_datum_wijziging** | **datetime**| Datum waarop het object is gewijzigd. | [optional] 
 **containerlocatie_datum_wijziging_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_datum_wijziging_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_datum_wijziging_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_datum_wijziging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_datum_wijziging_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_datum_wijziging_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_datum_wijziging_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_eigenaarschap** | **str**| Soort eigenaarschap | [optional] 
 **containerlocatie_eigenaarschap_opmerking** | **str**| Beschrijving van het type eigenaarschap. | [optional] 
 **containerlocatie_eigenaarschap_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_eigenaarschap_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_eigenaarschap_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_eigenaarschap_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_eigenaarschap_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_eigenaarschap_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_eigenaarschap_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_eigenaarschap_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_eigenaarschap_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_eigenaarschap_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_end_of_life** | **date**| Datum waarop het object het einde van zijn levenscyclus heeft bereikt. | [optional] 
 **containerlocatie_end_of_life_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **containerlocatie_end_of_life_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **containerlocatie_end_of_life_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_end_of_life_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_end_of_life_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **containerlocatie_end_of_life_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **containerlocatie_end_of_life_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **containerlocatie_id_nummer** | **str**| Definitie volgt nog | [optional] 
 **containerlocatie_id_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_id_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_id_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_id_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_id_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_opmerking** | **str**| Opmerking over het object. | [optional] 
 **containerlocatie_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_type_artikelcode** | **str**| Artikelcode van het containerlocatietype. | [optional] 
 **containerlocatie_type_artikelcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_type_artikelcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_type_artikelcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_type_artikelcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_type_artikelcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_type_naam** | **str**| Het type van de containerlocatie | [optional] 
 **containerlocatie_type_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_type_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_type_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_type_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_type_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_creatie** | **str**| Datum waarop het object is gecreëerd in container management systeem | [optional] 
 **datum_creatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_creatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_creatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_creatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_creatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_einde_garantie** | **str**| Datum waarop de garantie verloopt | [optional] 
 **datum_einde_garantie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_einde_garantie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_einde_garantie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_einde_garantie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_einde_garantie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_operationeel** | **str**| Datum waarop het object is operationeel gezet | [optional] 
 **datum_operationeel_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_operationeel_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_operationeel_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_operationeel_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_operationeel_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_oplevering** | **str**| Datum waarop het object is opgeleleverd | [optional] 
 **datum_oplevering_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_oplevering_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_oplevering_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_oplevering_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_oplevering_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_plaatsing** | **str**| Datum waarop het object op de locatie is geplaatst | [optional] 
 **datum_plaatsing_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_plaatsing_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_plaatsing_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_plaatsing_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_plaatsing_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **eigenaar_id** | **str**| Identificerend kenmerk eigenaar | [optional] 
 **eigenaar_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **eigenaar_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **eigenaar_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **eigenaar_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **eigenaar_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **eigenaar_naam** | **str**| Naam eigenaar | [optional] 
 **eigenaar_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **eigenaar_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **eigenaar_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **eigenaar_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **eigenaar_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de containerlocatie RD (epsg:28992) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id** | **str**| Identificerend kenmerk van de put waarin de container is geplaatst | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **ind_bevat_container** | **bool**| Indicatie dat de containerlocatie een container bevat | [optional] 
 **ind_bevat_container_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **serienummer** | **str**| serienummer uitgegeven door de fabrikant | [optional] 
 **serienummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **serienummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **serienummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **serienummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **serienummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **int**| Status van de container, 0 - inactief, 1 - actief, 2 - gepland | [optional] 
 **status_gt** | **int**| Greater than; number | [optional] 
 **status_gte** | **int**| Greater than or equal to; number | [optional] 
 **status_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_lt** | **int**| Less than; number | [optional] 
 **status_lte** | **int**| Less than or equal to; number | [optional] 
 **status_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **verwijderd_dp** | **bool**| Indicatie of het object verwijderd is bij de bronhouder | [optional] 
 **verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp** | **datetime**| Datum waarop het object is gewijzigd | [optional] 
 **wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalcontainerlocatieList**](PaginatedHuishoudelijkafvalcontainerlocatieList.md)

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

# **huishoudelijkafval_containerlocatie_retrieve2**
> Huishoudelijkafvalcontainerlocatie huishoudelijkafval_containerlocatie_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bronadres=bronadres, bronadres_in=bronadres_in, bronadres_isempty=bronadres_isempty, bronadres_isnull=bronadres_isnull, bronadres_like=bronadres_like, bronadres_not=bronadres_not, containerlocatie_datum_wijziging=containerlocatie_datum_wijziging, containerlocatie_datum_wijziging_gt=containerlocatie_datum_wijziging_gt, containerlocatie_datum_wijziging_gte=containerlocatie_datum_wijziging_gte, containerlocatie_datum_wijziging_in=containerlocatie_datum_wijziging_in, containerlocatie_datum_wijziging_isnull=containerlocatie_datum_wijziging_isnull, containerlocatie_datum_wijziging_lt=containerlocatie_datum_wijziging_lt, containerlocatie_datum_wijziging_lte=containerlocatie_datum_wijziging_lte, containerlocatie_datum_wijziging_not=containerlocatie_datum_wijziging_not, containerlocatie_eigenaarschap=containerlocatie_eigenaarschap, containerlocatie_eigenaarschap_opmerking=containerlocatie_eigenaarschap_opmerking, containerlocatie_eigenaarschap_opmerking_in=containerlocatie_eigenaarschap_opmerking_in, containerlocatie_eigenaarschap_opmerking_isempty=containerlocatie_eigenaarschap_opmerking_isempty, containerlocatie_eigenaarschap_opmerking_isnull=containerlocatie_eigenaarschap_opmerking_isnull, containerlocatie_eigenaarschap_opmerking_like=containerlocatie_eigenaarschap_opmerking_like, containerlocatie_eigenaarschap_opmerking_not=containerlocatie_eigenaarschap_opmerking_not, containerlocatie_eigenaarschap_in=containerlocatie_eigenaarschap_in, containerlocatie_eigenaarschap_isempty=containerlocatie_eigenaarschap_isempty, containerlocatie_eigenaarschap_isnull=containerlocatie_eigenaarschap_isnull, containerlocatie_eigenaarschap_like=containerlocatie_eigenaarschap_like, containerlocatie_eigenaarschap_not=containerlocatie_eigenaarschap_not, containerlocatie_end_of_life=containerlocatie_end_of_life, containerlocatie_end_of_life_gt=containerlocatie_end_of_life_gt, containerlocatie_end_of_life_gte=containerlocatie_end_of_life_gte, containerlocatie_end_of_life_in=containerlocatie_end_of_life_in, containerlocatie_end_of_life_isnull=containerlocatie_end_of_life_isnull, containerlocatie_end_of_life_lt=containerlocatie_end_of_life_lt, containerlocatie_end_of_life_lte=containerlocatie_end_of_life_lte, containerlocatie_end_of_life_not=containerlocatie_end_of_life_not, containerlocatie_id_nummer=containerlocatie_id_nummer, containerlocatie_id_nummer_in=containerlocatie_id_nummer_in, containerlocatie_id_nummer_isempty=containerlocatie_id_nummer_isempty, containerlocatie_id_nummer_isnull=containerlocatie_id_nummer_isnull, containerlocatie_id_nummer_like=containerlocatie_id_nummer_like, containerlocatie_id_nummer_not=containerlocatie_id_nummer_not, containerlocatie_opmerking=containerlocatie_opmerking, containerlocatie_opmerking_in=containerlocatie_opmerking_in, containerlocatie_opmerking_isempty=containerlocatie_opmerking_isempty, containerlocatie_opmerking_isnull=containerlocatie_opmerking_isnull, containerlocatie_opmerking_like=containerlocatie_opmerking_like, containerlocatie_opmerking_not=containerlocatie_opmerking_not, containerlocatie_type_artikelcode=containerlocatie_type_artikelcode, containerlocatie_type_artikelcode_in=containerlocatie_type_artikelcode_in, containerlocatie_type_artikelcode_isempty=containerlocatie_type_artikelcode_isempty, containerlocatie_type_artikelcode_isnull=containerlocatie_type_artikelcode_isnull, containerlocatie_type_artikelcode_like=containerlocatie_type_artikelcode_like, containerlocatie_type_artikelcode_not=containerlocatie_type_artikelcode_not, containerlocatie_type_naam=containerlocatie_type_naam, containerlocatie_type_naam_in=containerlocatie_type_naam_in, containerlocatie_type_naam_isempty=containerlocatie_type_naam_isempty, containerlocatie_type_naam_isnull=containerlocatie_type_naam_isnull, containerlocatie_type_naam_like=containerlocatie_type_naam_like, containerlocatie_type_naam_not=containerlocatie_type_naam_not, datum_creatie=datum_creatie, datum_creatie_in=datum_creatie_in, datum_creatie_isempty=datum_creatie_isempty, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_like=datum_creatie_like, datum_creatie_not=datum_creatie_not, datum_einde_garantie=datum_einde_garantie, datum_einde_garantie_in=datum_einde_garantie_in, datum_einde_garantie_isempty=datum_einde_garantie_isempty, datum_einde_garantie_isnull=datum_einde_garantie_isnull, datum_einde_garantie_like=datum_einde_garantie_like, datum_einde_garantie_not=datum_einde_garantie_not, datum_operationeel=datum_operationeel, datum_operationeel_in=datum_operationeel_in, datum_operationeel_isempty=datum_operationeel_isempty, datum_operationeel_isnull=datum_operationeel_isnull, datum_operationeel_like=datum_operationeel_like, datum_operationeel_not=datum_operationeel_not, datum_oplevering=datum_oplevering, datum_oplevering_in=datum_oplevering_in, datum_oplevering_isempty=datum_oplevering_isempty, datum_oplevering_isnull=datum_oplevering_isnull, datum_oplevering_like=datum_oplevering_like, datum_oplevering_not=datum_oplevering_not, datum_plaatsing=datum_plaatsing, datum_plaatsing_in=datum_plaatsing_in, datum_plaatsing_isempty=datum_plaatsing_isempty, datum_plaatsing_isnull=datum_plaatsing_isnull, datum_plaatsing_like=datum_plaatsing_like, datum_plaatsing_not=datum_plaatsing_not, eigenaar_id=eigenaar_id, eigenaar_id_in=eigenaar_id_in, eigenaar_id_isempty=eigenaar_id_isempty, eigenaar_id_isnull=eigenaar_id_isnull, eigenaar_id_like=eigenaar_id_like, eigenaar_id_not=eigenaar_id_not, eigenaar_naam=eigenaar_naam, eigenaar_naam_in=eigenaar_naam_in, eigenaar_naam_isempty=eigenaar_naam_isempty, eigenaar_naam_isnull=eigenaar_naam_isnull, eigenaar_naam_like=eigenaar_naam_like, eigenaar_naam_not=eigenaar_naam_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, ind_bevat_container=ind_bevat_container, ind_bevat_container_isnull=ind_bevat_container_isnull, serienummer=serienummer, serienummer_in=serienummer_in, serienummer_isempty=serienummer_isempty, serienummer_isnull=serienummer_isnull, serienummer_like=serienummer_like, serienummer_not=serienummer_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalcontainerlocatie import Huishoudelijkafvalcontainerlocatie
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
    api_instance = huishoudelijkafval_api_client.ContainerlocatieApi(api_client)
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
    bronadres = 'bronadres_example' # str | Adres van de containerlocatie zoals die in bron geregistreerd is. (optional)
    bronadres_in = ['bronadres_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bronadres_isempty = True # bool | Whether the field is empty or not. (optional)
    bronadres_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bronadres_like = 'bronadres_like_example' # str | Matches text using wildcards (? and *). (optional)
    bronadres_not = ['bronadres_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_datum_wijziging = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop het object is gewijzigd. (optional)
    containerlocatie_datum_wijziging_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_datum_wijziging_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_datum_wijziging_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_datum_wijziging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_datum_wijziging_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_datum_wijziging_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_datum_wijziging_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    containerlocatie_eigenaarschap = 'containerlocatie_eigenaarschap_example' # str | Soort eigenaarschap (optional)
    containerlocatie_eigenaarschap_opmerking = 'containerlocatie_eigenaarschap_opmerking_example' # str | Beschrijving van het type eigenaarschap. (optional)
    containerlocatie_eigenaarschap_opmerking_in = ['containerlocatie_eigenaarschap_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_eigenaarschap_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_eigenaarschap_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_eigenaarschap_opmerking_like = 'containerlocatie_eigenaarschap_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_eigenaarschap_opmerking_not = ['containerlocatie_eigenaarschap_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_eigenaarschap_in = ['containerlocatie_eigenaarschap_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_eigenaarschap_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_eigenaarschap_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_eigenaarschap_like = 'containerlocatie_eigenaarschap_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_eigenaarschap_not = ['containerlocatie_eigenaarschap_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_end_of_life = '2013-10-20' # date | Datum waarop het object het einde van zijn levenscyclus heeft bereikt. (optional)
    containerlocatie_end_of_life_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    containerlocatie_end_of_life_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    containerlocatie_end_of_life_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_end_of_life_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_end_of_life_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    containerlocatie_end_of_life_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    containerlocatie_end_of_life_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    containerlocatie_id_nummer = 'containerlocatie_id_nummer_example' # str | Definitie volgt nog (optional)
    containerlocatie_id_nummer_in = ['containerlocatie_id_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_id_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_id_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_id_nummer_like = 'containerlocatie_id_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_id_nummer_not = ['containerlocatie_id_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_opmerking = 'containerlocatie_opmerking_example' # str | Opmerking over het object. (optional)
    containerlocatie_opmerking_in = ['containerlocatie_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_opmerking_like = 'containerlocatie_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_opmerking_not = ['containerlocatie_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_type_artikelcode = 'containerlocatie_type_artikelcode_example' # str | Artikelcode van het containerlocatietype. (optional)
    containerlocatie_type_artikelcode_in = ['containerlocatie_type_artikelcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_type_artikelcode_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_type_artikelcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_type_artikelcode_like = 'containerlocatie_type_artikelcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_type_artikelcode_not = ['containerlocatie_type_artikelcode_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_type_naam = 'containerlocatie_type_naam_example' # str | Het type van de containerlocatie (optional)
    containerlocatie_type_naam_in = ['containerlocatie_type_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_type_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_type_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_type_naam_like = 'containerlocatie_type_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_type_naam_not = ['containerlocatie_type_naam_not_example'] # List[str] | Exclude matches; text (optional)
    datum_creatie = 'datum_creatie_example' # str | Datum waarop het object is gecreëerd in container management systeem (optional)
    datum_creatie_in = ['datum_creatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_creatie_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_creatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_creatie_like = 'datum_creatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_creatie_not = ['datum_creatie_not_example'] # List[str] | Exclude matches; text (optional)
    datum_einde_garantie = 'datum_einde_garantie_example' # str | Datum waarop de garantie verloopt (optional)
    datum_einde_garantie_in = ['datum_einde_garantie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_einde_garantie_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_einde_garantie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_einde_garantie_like = 'datum_einde_garantie_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_einde_garantie_not = ['datum_einde_garantie_not_example'] # List[str] | Exclude matches; text (optional)
    datum_operationeel = 'datum_operationeel_example' # str | Datum waarop het object is operationeel gezet (optional)
    datum_operationeel_in = ['datum_operationeel_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_operationeel_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_operationeel_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_operationeel_like = 'datum_operationeel_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_operationeel_not = ['datum_operationeel_not_example'] # List[str] | Exclude matches; text (optional)
    datum_oplevering = 'datum_oplevering_example' # str | Datum waarop het object is opgeleleverd (optional)
    datum_oplevering_in = ['datum_oplevering_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_oplevering_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_oplevering_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_oplevering_like = 'datum_oplevering_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_oplevering_not = ['datum_oplevering_not_example'] # List[str] | Exclude matches; text (optional)
    datum_plaatsing = 'datum_plaatsing_example' # str | Datum waarop het object op de locatie is geplaatst (optional)
    datum_plaatsing_in = ['datum_plaatsing_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_plaatsing_isempty = True # bool | Whether the field is empty or not. (optional)
    datum_plaatsing_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_plaatsing_like = 'datum_plaatsing_like_example' # str | Matches text using wildcards (? and *). (optional)
    datum_plaatsing_not = ['datum_plaatsing_not_example'] # List[str] | Exclude matches; text (optional)
    eigenaar_id = 'eigenaar_id_example' # str | Identificerend kenmerk eigenaar (optional)
    eigenaar_id_in = ['eigenaar_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    eigenaar_id_isempty = True # bool | Whether the field is empty or not. (optional)
    eigenaar_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    eigenaar_id_like = 'eigenaar_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    eigenaar_id_not = ['eigenaar_id_not_example'] # List[str] | Exclude matches; text (optional)
    eigenaar_naam = 'eigenaar_naam_example' # str | Naam eigenaar (optional)
    eigenaar_naam_in = ['eigenaar_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    eigenaar_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    eigenaar_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    eigenaar_naam_like = 'eigenaar_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    eigenaar_naam_not = ['eigenaar_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de containerlocatie RD (epsg:28992) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id2 = 'id_example' # str | Identificerend kenmerk van de put waarin de container is geplaatst (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    ind_bevat_container = True # bool | Indicatie dat de containerlocatie een container bevat (optional)
    ind_bevat_container_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    serienummer = 'serienummer_example' # str | serienummer uitgegeven door de fabrikant (optional)
    serienummer_in = ['serienummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    serienummer_isempty = True # bool | Whether the field is empty or not. (optional)
    serienummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    serienummer_like = 'serienummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    serienummer_not = ['serienummer_not_example'] # List[str] | Exclude matches; text (optional)
    status = 56 # int | Status van de container, 0 - inactief, 1 - actief, 2 - gepland (optional)
    status_gt = 56 # int | Greater than; number (optional)
    status_gte = 56 # int | Greater than or equal to; number (optional)
    status_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_lt = 56 # int | Less than; number (optional)
    status_lte = 56 # int | Less than or equal to; number (optional)
    status_not = [56] # List[int] | Exclude matches; number (optional)
    verwijderd_dp = True # bool | Indicatie of het object verwijderd is bij de bronhouder (optional)
    verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop het object is gewijzigd (optional)
    wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_containerlocatie_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bronadres=bronadres, bronadres_in=bronadres_in, bronadres_isempty=bronadres_isempty, bronadres_isnull=bronadres_isnull, bronadres_like=bronadres_like, bronadres_not=bronadres_not, containerlocatie_datum_wijziging=containerlocatie_datum_wijziging, containerlocatie_datum_wijziging_gt=containerlocatie_datum_wijziging_gt, containerlocatie_datum_wijziging_gte=containerlocatie_datum_wijziging_gte, containerlocatie_datum_wijziging_in=containerlocatie_datum_wijziging_in, containerlocatie_datum_wijziging_isnull=containerlocatie_datum_wijziging_isnull, containerlocatie_datum_wijziging_lt=containerlocatie_datum_wijziging_lt, containerlocatie_datum_wijziging_lte=containerlocatie_datum_wijziging_lte, containerlocatie_datum_wijziging_not=containerlocatie_datum_wijziging_not, containerlocatie_eigenaarschap=containerlocatie_eigenaarschap, containerlocatie_eigenaarschap_opmerking=containerlocatie_eigenaarschap_opmerking, containerlocatie_eigenaarschap_opmerking_in=containerlocatie_eigenaarschap_opmerking_in, containerlocatie_eigenaarschap_opmerking_isempty=containerlocatie_eigenaarschap_opmerking_isempty, containerlocatie_eigenaarschap_opmerking_isnull=containerlocatie_eigenaarschap_opmerking_isnull, containerlocatie_eigenaarschap_opmerking_like=containerlocatie_eigenaarschap_opmerking_like, containerlocatie_eigenaarschap_opmerking_not=containerlocatie_eigenaarschap_opmerking_not, containerlocatie_eigenaarschap_in=containerlocatie_eigenaarschap_in, containerlocatie_eigenaarschap_isempty=containerlocatie_eigenaarschap_isempty, containerlocatie_eigenaarschap_isnull=containerlocatie_eigenaarschap_isnull, containerlocatie_eigenaarschap_like=containerlocatie_eigenaarschap_like, containerlocatie_eigenaarschap_not=containerlocatie_eigenaarschap_not, containerlocatie_end_of_life=containerlocatie_end_of_life, containerlocatie_end_of_life_gt=containerlocatie_end_of_life_gt, containerlocatie_end_of_life_gte=containerlocatie_end_of_life_gte, containerlocatie_end_of_life_in=containerlocatie_end_of_life_in, containerlocatie_end_of_life_isnull=containerlocatie_end_of_life_isnull, containerlocatie_end_of_life_lt=containerlocatie_end_of_life_lt, containerlocatie_end_of_life_lte=containerlocatie_end_of_life_lte, containerlocatie_end_of_life_not=containerlocatie_end_of_life_not, containerlocatie_id_nummer=containerlocatie_id_nummer, containerlocatie_id_nummer_in=containerlocatie_id_nummer_in, containerlocatie_id_nummer_isempty=containerlocatie_id_nummer_isempty, containerlocatie_id_nummer_isnull=containerlocatie_id_nummer_isnull, containerlocatie_id_nummer_like=containerlocatie_id_nummer_like, containerlocatie_id_nummer_not=containerlocatie_id_nummer_not, containerlocatie_opmerking=containerlocatie_opmerking, containerlocatie_opmerking_in=containerlocatie_opmerking_in, containerlocatie_opmerking_isempty=containerlocatie_opmerking_isempty, containerlocatie_opmerking_isnull=containerlocatie_opmerking_isnull, containerlocatie_opmerking_like=containerlocatie_opmerking_like, containerlocatie_opmerking_not=containerlocatie_opmerking_not, containerlocatie_type_artikelcode=containerlocatie_type_artikelcode, containerlocatie_type_artikelcode_in=containerlocatie_type_artikelcode_in, containerlocatie_type_artikelcode_isempty=containerlocatie_type_artikelcode_isempty, containerlocatie_type_artikelcode_isnull=containerlocatie_type_artikelcode_isnull, containerlocatie_type_artikelcode_like=containerlocatie_type_artikelcode_like, containerlocatie_type_artikelcode_not=containerlocatie_type_artikelcode_not, containerlocatie_type_naam=containerlocatie_type_naam, containerlocatie_type_naam_in=containerlocatie_type_naam_in, containerlocatie_type_naam_isempty=containerlocatie_type_naam_isempty, containerlocatie_type_naam_isnull=containerlocatie_type_naam_isnull, containerlocatie_type_naam_like=containerlocatie_type_naam_like, containerlocatie_type_naam_not=containerlocatie_type_naam_not, datum_creatie=datum_creatie, datum_creatie_in=datum_creatie_in, datum_creatie_isempty=datum_creatie_isempty, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_like=datum_creatie_like, datum_creatie_not=datum_creatie_not, datum_einde_garantie=datum_einde_garantie, datum_einde_garantie_in=datum_einde_garantie_in, datum_einde_garantie_isempty=datum_einde_garantie_isempty, datum_einde_garantie_isnull=datum_einde_garantie_isnull, datum_einde_garantie_like=datum_einde_garantie_like, datum_einde_garantie_not=datum_einde_garantie_not, datum_operationeel=datum_operationeel, datum_operationeel_in=datum_operationeel_in, datum_operationeel_isempty=datum_operationeel_isempty, datum_operationeel_isnull=datum_operationeel_isnull, datum_operationeel_like=datum_operationeel_like, datum_operationeel_not=datum_operationeel_not, datum_oplevering=datum_oplevering, datum_oplevering_in=datum_oplevering_in, datum_oplevering_isempty=datum_oplevering_isempty, datum_oplevering_isnull=datum_oplevering_isnull, datum_oplevering_like=datum_oplevering_like, datum_oplevering_not=datum_oplevering_not, datum_plaatsing=datum_plaatsing, datum_plaatsing_in=datum_plaatsing_in, datum_plaatsing_isempty=datum_plaatsing_isempty, datum_plaatsing_isnull=datum_plaatsing_isnull, datum_plaatsing_like=datum_plaatsing_like, datum_plaatsing_not=datum_plaatsing_not, eigenaar_id=eigenaar_id, eigenaar_id_in=eigenaar_id_in, eigenaar_id_isempty=eigenaar_id_isempty, eigenaar_id_isnull=eigenaar_id_isnull, eigenaar_id_like=eigenaar_id_like, eigenaar_id_not=eigenaar_id_not, eigenaar_naam=eigenaar_naam, eigenaar_naam_in=eigenaar_naam_in, eigenaar_naam_isempty=eigenaar_naam_isempty, eigenaar_naam_isnull=eigenaar_naam_isnull, eigenaar_naam_like=eigenaar_naam_like, eigenaar_naam_not=eigenaar_naam_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, ind_bevat_container=ind_bevat_container, ind_bevat_container_isnull=ind_bevat_container_isnull, serienummer=serienummer, serienummer_in=serienummer_in, serienummer_isempty=serienummer_isempty, serienummer_isnull=serienummer_isnull, serienummer_like=serienummer_like, serienummer_not=serienummer_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ContainerlocatieApi->huishoudelijkafval_containerlocatie_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContainerlocatieApi->huishoudelijkafval_containerlocatie_retrieve2: %s\n" % e)
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
 **bronadres** | **str**| Adres van de containerlocatie zoals die in bron geregistreerd is. | [optional] 
 **bronadres_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bronadres_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bronadres_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bronadres_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bronadres_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_datum_wijziging** | **datetime**| Datum waarop het object is gewijzigd. | [optional] 
 **containerlocatie_datum_wijziging_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_datum_wijziging_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_datum_wijziging_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_datum_wijziging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_datum_wijziging_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_datum_wijziging_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_datum_wijziging_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **containerlocatie_eigenaarschap** | **str**| Soort eigenaarschap | [optional] 
 **containerlocatie_eigenaarschap_opmerking** | **str**| Beschrijving van het type eigenaarschap. | [optional] 
 **containerlocatie_eigenaarschap_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_eigenaarschap_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_eigenaarschap_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_eigenaarschap_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_eigenaarschap_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_eigenaarschap_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_eigenaarschap_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_eigenaarschap_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_eigenaarschap_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_eigenaarschap_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_end_of_life** | **date**| Datum waarop het object het einde van zijn levenscyclus heeft bereikt. | [optional] 
 **containerlocatie_end_of_life_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **containerlocatie_end_of_life_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **containerlocatie_end_of_life_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_end_of_life_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_end_of_life_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **containerlocatie_end_of_life_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **containerlocatie_end_of_life_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **containerlocatie_id_nummer** | **str**| Definitie volgt nog | [optional] 
 **containerlocatie_id_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_id_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_id_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_id_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_id_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_opmerking** | **str**| Opmerking over het object. | [optional] 
 **containerlocatie_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_type_artikelcode** | **str**| Artikelcode van het containerlocatietype. | [optional] 
 **containerlocatie_type_artikelcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_type_artikelcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_type_artikelcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_type_artikelcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_type_artikelcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_type_naam** | **str**| Het type van de containerlocatie | [optional] 
 **containerlocatie_type_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_type_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_type_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_type_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_type_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_creatie** | **str**| Datum waarop het object is gecreëerd in container management systeem | [optional] 
 **datum_creatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_creatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_creatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_creatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_creatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_einde_garantie** | **str**| Datum waarop de garantie verloopt | [optional] 
 **datum_einde_garantie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_einde_garantie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_einde_garantie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_einde_garantie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_einde_garantie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_operationeel** | **str**| Datum waarop het object is operationeel gezet | [optional] 
 **datum_operationeel_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_operationeel_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_operationeel_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_operationeel_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_operationeel_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_oplevering** | **str**| Datum waarop het object is opgeleleverd | [optional] 
 **datum_oplevering_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_oplevering_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_oplevering_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_oplevering_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_oplevering_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_plaatsing** | **str**| Datum waarop het object op de locatie is geplaatst | [optional] 
 **datum_plaatsing_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_plaatsing_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **datum_plaatsing_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_plaatsing_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **datum_plaatsing_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **eigenaar_id** | **str**| Identificerend kenmerk eigenaar | [optional] 
 **eigenaar_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **eigenaar_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **eigenaar_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **eigenaar_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **eigenaar_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **eigenaar_naam** | **str**| Naam eigenaar | [optional] 
 **eigenaar_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **eigenaar_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **eigenaar_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **eigenaar_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **eigenaar_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de containerlocatie RD (epsg:28992) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id2** | **str**| Identificerend kenmerk van de put waarin de container is geplaatst | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **ind_bevat_container** | **bool**| Indicatie dat de containerlocatie een container bevat | [optional] 
 **ind_bevat_container_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **serienummer** | **str**| serienummer uitgegeven door de fabrikant | [optional] 
 **serienummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **serienummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **serienummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **serienummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **serienummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **int**| Status van de container, 0 - inactief, 1 - actief, 2 - gepland | [optional] 
 **status_gt** | **int**| Greater than; number | [optional] 
 **status_gte** | **int**| Greater than or equal to; number | [optional] 
 **status_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_lt** | **int**| Less than; number | [optional] 
 **status_lte** | **int**| Less than or equal to; number | [optional] 
 **status_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **verwijderd_dp** | **bool**| Indicatie of het object verwijderd is bij de bronhouder | [optional] 
 **verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp** | **datetime**| Datum waarop het object is gewijzigd | [optional] 
 **wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**Huishoudelijkafvalcontainerlocatie**](Huishoudelijkafvalcontainerlocatie.md)

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

