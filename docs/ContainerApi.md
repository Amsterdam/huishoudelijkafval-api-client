# huishoudelijkafval_api_client.ContainerApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_container_list2**](ContainerApi.md#huishoudelijkafval_container_list2) | **GET** /container | 
[**huishoudelijkafval_container_retrieve2**](ContainerApi.md#huishoudelijkafval_container_retrieve2) | **GET** /container/{id} | 


# **huishoudelijkafval_container_list2**
> PaginatedHuishoudelijkafvalcontainerList huishoudelijkafval_container_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, container_chip_nummber=container_chip_nummber, container_chip_nummber_in=container_chip_nummber_in, container_chip_nummber_isempty=container_chip_nummber_isempty, container_chip_nummber_isnull=container_chip_nummber_isnull, container_chip_nummber_like=container_chip_nummber_like, container_chip_nummber_not=container_chip_nummber_not, container_datum_vervanging=container_datum_vervanging, container_datum_vervanging_gt=container_datum_vervanging_gt, container_datum_vervanging_gte=container_datum_vervanging_gte, container_datum_vervanging_in=container_datum_vervanging_in, container_datum_vervanging_isnull=container_datum_vervanging_isnull, container_datum_vervanging_lt=container_datum_vervanging_lt, container_datum_vervanging_lte=container_datum_vervanging_lte, container_datum_vervanging_not=container_datum_vervanging_not, container_datum_wijziging=container_datum_wijziging, container_datum_wijziging_gt=container_datum_wijziging_gt, container_datum_wijziging_gte=container_datum_wijziging_gte, container_datum_wijziging_in=container_datum_wijziging_in, container_datum_wijziging_isnull=container_datum_wijziging_isnull, container_datum_wijziging_lt=container_datum_wijziging_lt, container_datum_wijziging_lte=container_datum_wijziging_lte, container_datum_wijziging_not=container_datum_wijziging_not, container_eigenaarschap=container_eigenaarschap, container_eigenaarschap_opmerking=container_eigenaarschap_opmerking, container_eigenaarschap_opmerking_in=container_eigenaarschap_opmerking_in, container_eigenaarschap_opmerking_isempty=container_eigenaarschap_opmerking_isempty, container_eigenaarschap_opmerking_isnull=container_eigenaarschap_opmerking_isnull, container_eigenaarschap_opmerking_like=container_eigenaarschap_opmerking_like, container_eigenaarschap_opmerking_not=container_eigenaarschap_opmerking_not, container_eigenaarschap_in=container_eigenaarschap_in, container_eigenaarschap_isempty=container_eigenaarschap_isempty, container_eigenaarschap_isnull=container_eigenaarschap_isnull, container_eigenaarschap_like=container_eigenaarschap_like, container_eigenaarschap_not=container_eigenaarschap_not, container_end_of_life=container_end_of_life, container_end_of_life_gt=container_end_of_life_gt, container_end_of_life_gte=container_end_of_life_gte, container_end_of_life_in=container_end_of_life_in, container_end_of_life_isnull=container_end_of_life_isnull, container_end_of_life_lt=container_end_of_life_lt, container_end_of_life_lte=container_end_of_life_lte, container_end_of_life_not=container_end_of_life_not, container_kleur=container_kleur, container_kleur_in=container_kleur_in, container_kleur_isempty=container_kleur_isempty, container_kleur_isnull=container_kleur_isnull, container_kleur_like=container_kleur_like, container_kleur_not=container_kleur_not, container_mark=container_mark, container_mark_gt=container_mark_gt, container_mark_gte=container_mark_gte, container_mark_in=container_mark_in, container_mark_isnull=container_mark_isnull, container_mark_lt=container_mark_lt, container_mark_lte=container_mark_lte, container_mark_not=container_mark_not, container_opmerking=container_opmerking, container_opmerking_in=container_opmerking_in, container_opmerking_isempty=container_opmerking_isempty, container_opmerking_isnull=container_opmerking_isnull, container_opmerking_like=container_opmerking_like, container_opmerking_not=container_opmerking_not, container_ral_kleur_code=container_ral_kleur_code, container_ral_kleur_code_in=container_ral_kleur_code_in, container_ral_kleur_code_isempty=container_ral_kleur_code_isempty, container_ral_kleur_code_isnull=container_ral_kleur_code_isnull, container_ral_kleur_code_like=container_ral_kleur_code_like, container_ral_kleur_code_not=container_ral_kleur_code_not, container_ral_kleur_hexcode=container_ral_kleur_hexcode, container_ral_kleur_hexcode_in=container_ral_kleur_hexcode_in, container_ral_kleur_hexcode_isempty=container_ral_kleur_hexcode_isempty, container_ral_kleur_hexcode_isnull=container_ral_kleur_hexcode_isnull, container_ral_kleur_hexcode_like=container_ral_kleur_hexcode_like, container_ral_kleur_hexcode_not=container_ral_kleur_hexcode_not, container_ral_kleur_naam=container_ral_kleur_naam, container_ral_kleur_naam_in=container_ral_kleur_naam_in, container_ral_kleur_naam_isempty=container_ral_kleur_naam_isempty, container_ral_kleur_naam_isnull=container_ral_kleur_naam_isnull, container_ral_kleur_naam_like=container_ral_kleur_naam_like, container_ral_kleur_naam_not=container_ral_kleur_naam_not, container_unit_card_lezer_id=container_unit_card_lezer_id, container_unit_card_lezer_id_in=container_unit_card_lezer_id_in, container_unit_card_lezer_id_isempty=container_unit_card_lezer_id_isempty, container_unit_card_lezer_id_isnull=container_unit_card_lezer_id_isnull, container_unit_card_lezer_id_like=container_unit_card_lezer_id_like, container_unit_card_lezer_id_not=container_unit_card_lezer_id_not, datum_aflopen_garantie=datum_aflopen_garantie, datum_aflopen_garantie_gt=datum_aflopen_garantie_gt, datum_aflopen_garantie_gte=datum_aflopen_garantie_gte, datum_aflopen_garantie_in=datum_aflopen_garantie_in, datum_aflopen_garantie_isnull=datum_aflopen_garantie_isnull, datum_aflopen_garantie_lt=datum_aflopen_garantie_lt, datum_aflopen_garantie_lte=datum_aflopen_garantie_lte, datum_aflopen_garantie_not=datum_aflopen_garantie_not, datum_creatie=datum_creatie, datum_creatie_gt=datum_creatie_gt, datum_creatie_gte=datum_creatie_gte, datum_creatie_in=datum_creatie_in, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_lt=datum_creatie_lt, datum_creatie_lte=datum_creatie_lte, datum_creatie_not=datum_creatie_not, datum_operationeel=datum_operationeel, datum_operationeel_gt=datum_operationeel_gt, datum_operationeel_gte=datum_operationeel_gte, datum_operationeel_in=datum_operationeel_in, datum_operationeel_isnull=datum_operationeel_isnull, datum_operationeel_lt=datum_operationeel_lt, datum_operationeel_lte=datum_operationeel_lte, datum_operationeel_not=datum_operationeel_not, datum_oplevering=datum_oplevering, datum_oplevering_gt=datum_oplevering_gt, datum_oplevering_gte=datum_oplevering_gte, datum_oplevering_in=datum_oplevering_in, datum_oplevering_isnull=datum_oplevering_isnull, datum_oplevering_lt=datum_oplevering_lt, datum_oplevering_lte=datum_oplevering_lte, datum_oplevering_not=datum_oplevering_not, datum_plaatsing=datum_plaatsing, datum_plaatsing_gt=datum_plaatsing_gt, datum_plaatsing_gte=datum_plaatsing_gte, datum_plaatsing_in=datum_plaatsing_in, datum_plaatsing_isnull=datum_plaatsing_isnull, datum_plaatsing_lt=datum_plaatsing_lt, datum_plaatsing_lte=datum_plaatsing_lte, datum_plaatsing_not=datum_plaatsing_not, eigenaar_id=eigenaar_id, eigenaar_id_in=eigenaar_id_in, eigenaar_id_isempty=eigenaar_id_isempty, eigenaar_id_isnull=eigenaar_id_isnull, eigenaar_id_like=eigenaar_id_like, eigenaar_id_not=eigenaar_id_not, eigenaar_naam=eigenaar_naam, eigenaar_naam_in=eigenaar_naam_in, eigenaar_naam_isempty=eigenaar_naam_isempty, eigenaar_naam_isnull=eigenaar_naam_isnull, eigenaar_naam_like=eigenaar_naam_like, eigenaar_naam_not=eigenaar_naam_not, fractie_code=fractie_code, fractie_code_in=fractie_code_in, fractie_code_isempty=fractie_code_isempty, fractie_code_isnull=fractie_code_isnull, fractie_code_like=fractie_code_like, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geadopteerd_ind=geadopteerd_ind, geadopteerd_ind_isnull=geadopteerd_ind_isnull, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_nummer=id_nummer, id_nummer_in=id_nummer_in, id_nummer_isempty=id_nummer_isempty, id_nummer_isnull=id_nummer_isnull, id_nummer_like=id_nummer_like, id_nummer_not=id_nummer_not, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, locatie_id=locatie_id, locatie_id_in=locatie_id_in, locatie_id_isempty=locatie_id_isempty, locatie_id_isnull=locatie_id_isnull, locatie_id_like=locatie_id_like, locatie_id_not=locatie_id_not, page=page, serienummer=serienummer, serienummer_in=serienummer_in, serienummer_isempty=serienummer_isempty, serienummer_isnull=serienummer_isnull, serienummer_like=serienummer_like, serienummer_not=serienummer_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, type_id=type_id, type_id_in=type_id_in, type_id_isempty=type_id_isempty, type_id_isnull=type_id_isnull, type_id_like=type_id_like, type_id_not=type_id_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

Bevat een overzicht van alle onder- en bovengronds afvalcontainers in Gemeente Amsterdam

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalcontainer_list import PaginatedHuishoudelijkafvalcontainerList
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
    api_instance = huishoudelijkafval_api_client.ContainerApi(api_client)
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
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
    container_chip_nummber = 'container_chip_nummber_example' # str | Het identificatienummer van de chip die registreert wanneer de container wordt geleegd. (optional)
    container_chip_nummber_in = ['container_chip_nummber_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_chip_nummber_isempty = True # bool | Whether the field is empty or not. (optional)
    container_chip_nummber_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_chip_nummber_like = 'container_chip_nummber_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_chip_nummber_not = ['container_chip_nummber_not_example'] # List[str] | Exclude matches; text (optional)
    container_datum_vervanging = '2013-10-20' # date | De datum waarop de container wordt vervangen. (optional)
    container_datum_vervanging_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    container_datum_vervanging_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    container_datum_vervanging_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_datum_vervanging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_datum_vervanging_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    container_datum_vervanging_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    container_datum_vervanging_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    container_datum_wijziging = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop de container is gewijzigd. (optional)
    container_datum_wijziging_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_datum_wijziging_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_datum_wijziging_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_datum_wijziging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_datum_wijziging_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_datum_wijziging_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_datum_wijziging_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_eigenaarschap = 'container_eigenaarschap_example' # str | De soort eigenaarschap van het object. (optional)
    container_eigenaarschap_opmerking = 'container_eigenaarschap_opmerking_example' # str | Beschrijving van  het type eigenaarschap. (optional)
    container_eigenaarschap_opmerking_in = ['container_eigenaarschap_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_eigenaarschap_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    container_eigenaarschap_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_eigenaarschap_opmerking_like = 'container_eigenaarschap_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_eigenaarschap_opmerking_not = ['container_eigenaarschap_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    container_eigenaarschap_in = ['container_eigenaarschap_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_eigenaarschap_isempty = True # bool | Whether the field is empty or not. (optional)
    container_eigenaarschap_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_eigenaarschap_like = 'container_eigenaarschap_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_eigenaarschap_not = ['container_eigenaarschap_not_example'] # List[str] | Exclude matches; text (optional)
    container_end_of_life = '2013-10-20' # date | Datum waarop het object het einde van zijn levenscyclus heeft bereikt. (optional)
    container_end_of_life_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    container_end_of_life_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    container_end_of_life_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_end_of_life_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_end_of_life_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    container_end_of_life_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    container_end_of_life_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    container_kleur = 'container_kleur_example' # str | De naam van de kleur (optional)
    container_kleur_in = ['container_kleur_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_kleur_isempty = True # bool | Whether the field is empty or not. (optional)
    container_kleur_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_kleur_like = 'container_kleur_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_kleur_not = ['container_kleur_not_example'] # List[str] | Exclude matches; text (optional)
    container_mark = 56 # int | Definitie volgt nog (optional)
    container_mark_gt = 56 # int | Greater than; number (optional)
    container_mark_gte = 56 # int | Greater than or equal to; number (optional)
    container_mark_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_mark_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_mark_lt = 56 # int | Less than; number (optional)
    container_mark_lte = 56 # int | Less than or equal to; number (optional)
    container_mark_not = [56] # List[int] | Exclude matches; number (optional)
    container_opmerking = 'container_opmerking_example' # str | Opmerking over het object door de betrokken medewerker. (optional)
    container_opmerking_in = ['container_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    container_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_opmerking_like = 'container_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_opmerking_not = ['container_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    container_ral_kleur_code = 'container_ral_kleur_code_example' # str | De internationale ralkleurcode. (optional)
    container_ral_kleur_code_in = ['container_ral_kleur_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_ral_kleur_code_isempty = True # bool | Whether the field is empty or not. (optional)
    container_ral_kleur_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_ral_kleur_code_like = 'container_ral_kleur_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_ral_kleur_code_not = ['container_ral_kleur_code_not_example'] # List[str] | Exclude matches; text (optional)
    container_ral_kleur_hexcode = 'container_ral_kleur_hexcode_example' # str | De hexcode van de ralkleur. (optional)
    container_ral_kleur_hexcode_in = ['container_ral_kleur_hexcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_ral_kleur_hexcode_isempty = True # bool | Whether the field is empty or not. (optional)
    container_ral_kleur_hexcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_ral_kleur_hexcode_like = 'container_ral_kleur_hexcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_ral_kleur_hexcode_not = ['container_ral_kleur_hexcode_not_example'] # List[str] | Exclude matches; text (optional)
    container_ral_kleur_naam = 'container_ral_kleur_naam_example' # str | De naam van de ralkleur (optional)
    container_ral_kleur_naam_in = ['container_ral_kleur_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_ral_kleur_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    container_ral_kleur_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_ral_kleur_naam_like = 'container_ral_kleur_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_ral_kleur_naam_not = ['container_ral_kleur_naam_not_example'] # List[str] | Exclude matches; text (optional)
    container_unit_card_lezer_id = 'container_unit_card_lezer_id_example' # str | Het identificatienummer van de kaartlezer. (optional)
    container_unit_card_lezer_id_in = ['container_unit_card_lezer_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_unit_card_lezer_id_isempty = True # bool | Whether the field is empty or not. (optional)
    container_unit_card_lezer_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_unit_card_lezer_id_like = 'container_unit_card_lezer_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_unit_card_lezer_id_not = ['container_unit_card_lezer_id_not_example'] # List[str] | Exclude matches; text (optional)
    datum_aflopen_garantie = '2013-10-20' # date | Datum waarop de garantie verloopt (optional)
    datum_aflopen_garantie_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_aflopen_garantie_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_aflopen_garantie_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_aflopen_garantie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_aflopen_garantie_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_aflopen_garantie_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_aflopen_garantie_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_creatie = '2013-10-20' # date | Datum waarop het object is gecreëerd in container management systeem (optional)
    datum_creatie_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_creatie_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_creatie_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_creatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_creatie_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_creatie_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_creatie_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_operationeel = '2013-10-20' # date | Datum dat de container operationeel is voor het aanbieden van afval (optional)
    datum_operationeel_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_operationeel_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_operationeel_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_operationeel_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_operationeel_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_operationeel_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_operationeel_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_oplevering = '2013-10-20' # date | Datum waarop het object is geleverd (optional)
    datum_oplevering_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_oplevering_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_oplevering_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_oplevering_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_oplevering_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_oplevering_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_oplevering_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_plaatsing = '2013-10-20' # date | Datum waarop het object op de locatie is geplaatst (optional)
    datum_plaatsing_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_plaatsing_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_plaatsing_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_plaatsing_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_plaatsing_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_plaatsing_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_plaatsing_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
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
    fractie_code = 'fractie_code_example' # str | Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood (optional)
    fractie_code_in = ['fractie_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_code_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_code_like = 'fractie_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_code_not = ['fractie_code_not_example'] # List[str] | Exclude matches; text (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Container fractieomschrijving zoals door leverancier is geleverd. (optional)
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
    geadopteerd_ind = True # bool | indicatie of het object door een bewoner geadopteerd is (optional)
    geadopteerd_ind_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de container RD (epsg:28992) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id = 'id_example' # str | Unieke aanduiding objecttype (optional)
    id_nummer = 'id_nummer_example' # str | Identificatie dat door de fabrikant aan het object is gegeven (optional)
    id_nummer_in = ['id_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    id_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_nummer_like = 'id_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_nummer_not = ['id_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    locatie_id = 'locatie_id_example' # str | Identificerend kenmerk van de put waarin de container is geplaatst (optional)
    locatie_id_in = ['locatie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    locatie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    locatie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    locatie_id_like = 'locatie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    locatie_id_not = ['locatie_id_not_example'] # List[str] | Exclude matches; text (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    serienummer = 'serienummer_example' # str | serienummer uitgegeven door de fabrikant (optional)
    serienummer_in = ['serienummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    serienummer_isempty = True # bool | Whether the field is empty or not. (optional)
    serienummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    serienummer_like = 'serienummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    serienummer_not = ['serienummer_not_example'] # List[str] | Exclude matches; text (optional)
    status = 56 # int | Status van de container,0 - inactief, 1 - actief, 2 - gepland (optional)
    status_gt = 56 # int | Greater than; number (optional)
    status_gte = 56 # int | Greater than or equal to; number (optional)
    status_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_lt = 56 # int | Less than; number (optional)
    status_lte = 56 # int | Less than or equal to; number (optional)
    status_not = [56] # List[int] | Exclude matches; number (optional)
    type_id = 'type_id_example' # str | Unieke aanduiding objecttype (optional)
    type_id_in = ['type_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    type_id_isempty = True # bool | Whether the field is empty or not. (optional)
    type_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    type_id_like = 'type_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    type_id_not = ['type_id_not_example'] # List[str] | Exclude matches; text (optional)
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
        api_response = await api_instance.huishoudelijkafval_container_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, container_chip_nummber=container_chip_nummber, container_chip_nummber_in=container_chip_nummber_in, container_chip_nummber_isempty=container_chip_nummber_isempty, container_chip_nummber_isnull=container_chip_nummber_isnull, container_chip_nummber_like=container_chip_nummber_like, container_chip_nummber_not=container_chip_nummber_not, container_datum_vervanging=container_datum_vervanging, container_datum_vervanging_gt=container_datum_vervanging_gt, container_datum_vervanging_gte=container_datum_vervanging_gte, container_datum_vervanging_in=container_datum_vervanging_in, container_datum_vervanging_isnull=container_datum_vervanging_isnull, container_datum_vervanging_lt=container_datum_vervanging_lt, container_datum_vervanging_lte=container_datum_vervanging_lte, container_datum_vervanging_not=container_datum_vervanging_not, container_datum_wijziging=container_datum_wijziging, container_datum_wijziging_gt=container_datum_wijziging_gt, container_datum_wijziging_gte=container_datum_wijziging_gte, container_datum_wijziging_in=container_datum_wijziging_in, container_datum_wijziging_isnull=container_datum_wijziging_isnull, container_datum_wijziging_lt=container_datum_wijziging_lt, container_datum_wijziging_lte=container_datum_wijziging_lte, container_datum_wijziging_not=container_datum_wijziging_not, container_eigenaarschap=container_eigenaarschap, container_eigenaarschap_opmerking=container_eigenaarschap_opmerking, container_eigenaarschap_opmerking_in=container_eigenaarschap_opmerking_in, container_eigenaarschap_opmerking_isempty=container_eigenaarschap_opmerking_isempty, container_eigenaarschap_opmerking_isnull=container_eigenaarschap_opmerking_isnull, container_eigenaarschap_opmerking_like=container_eigenaarschap_opmerking_like, container_eigenaarschap_opmerking_not=container_eigenaarschap_opmerking_not, container_eigenaarschap_in=container_eigenaarschap_in, container_eigenaarschap_isempty=container_eigenaarschap_isempty, container_eigenaarschap_isnull=container_eigenaarschap_isnull, container_eigenaarschap_like=container_eigenaarschap_like, container_eigenaarschap_not=container_eigenaarschap_not, container_end_of_life=container_end_of_life, container_end_of_life_gt=container_end_of_life_gt, container_end_of_life_gte=container_end_of_life_gte, container_end_of_life_in=container_end_of_life_in, container_end_of_life_isnull=container_end_of_life_isnull, container_end_of_life_lt=container_end_of_life_lt, container_end_of_life_lte=container_end_of_life_lte, container_end_of_life_not=container_end_of_life_not, container_kleur=container_kleur, container_kleur_in=container_kleur_in, container_kleur_isempty=container_kleur_isempty, container_kleur_isnull=container_kleur_isnull, container_kleur_like=container_kleur_like, container_kleur_not=container_kleur_not, container_mark=container_mark, container_mark_gt=container_mark_gt, container_mark_gte=container_mark_gte, container_mark_in=container_mark_in, container_mark_isnull=container_mark_isnull, container_mark_lt=container_mark_lt, container_mark_lte=container_mark_lte, container_mark_not=container_mark_not, container_opmerking=container_opmerking, container_opmerking_in=container_opmerking_in, container_opmerking_isempty=container_opmerking_isempty, container_opmerking_isnull=container_opmerking_isnull, container_opmerking_like=container_opmerking_like, container_opmerking_not=container_opmerking_not, container_ral_kleur_code=container_ral_kleur_code, container_ral_kleur_code_in=container_ral_kleur_code_in, container_ral_kleur_code_isempty=container_ral_kleur_code_isempty, container_ral_kleur_code_isnull=container_ral_kleur_code_isnull, container_ral_kleur_code_like=container_ral_kleur_code_like, container_ral_kleur_code_not=container_ral_kleur_code_not, container_ral_kleur_hexcode=container_ral_kleur_hexcode, container_ral_kleur_hexcode_in=container_ral_kleur_hexcode_in, container_ral_kleur_hexcode_isempty=container_ral_kleur_hexcode_isempty, container_ral_kleur_hexcode_isnull=container_ral_kleur_hexcode_isnull, container_ral_kleur_hexcode_like=container_ral_kleur_hexcode_like, container_ral_kleur_hexcode_not=container_ral_kleur_hexcode_not, container_ral_kleur_naam=container_ral_kleur_naam, container_ral_kleur_naam_in=container_ral_kleur_naam_in, container_ral_kleur_naam_isempty=container_ral_kleur_naam_isempty, container_ral_kleur_naam_isnull=container_ral_kleur_naam_isnull, container_ral_kleur_naam_like=container_ral_kleur_naam_like, container_ral_kleur_naam_not=container_ral_kleur_naam_not, container_unit_card_lezer_id=container_unit_card_lezer_id, container_unit_card_lezer_id_in=container_unit_card_lezer_id_in, container_unit_card_lezer_id_isempty=container_unit_card_lezer_id_isempty, container_unit_card_lezer_id_isnull=container_unit_card_lezer_id_isnull, container_unit_card_lezer_id_like=container_unit_card_lezer_id_like, container_unit_card_lezer_id_not=container_unit_card_lezer_id_not, datum_aflopen_garantie=datum_aflopen_garantie, datum_aflopen_garantie_gt=datum_aflopen_garantie_gt, datum_aflopen_garantie_gte=datum_aflopen_garantie_gte, datum_aflopen_garantie_in=datum_aflopen_garantie_in, datum_aflopen_garantie_isnull=datum_aflopen_garantie_isnull, datum_aflopen_garantie_lt=datum_aflopen_garantie_lt, datum_aflopen_garantie_lte=datum_aflopen_garantie_lte, datum_aflopen_garantie_not=datum_aflopen_garantie_not, datum_creatie=datum_creatie, datum_creatie_gt=datum_creatie_gt, datum_creatie_gte=datum_creatie_gte, datum_creatie_in=datum_creatie_in, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_lt=datum_creatie_lt, datum_creatie_lte=datum_creatie_lte, datum_creatie_not=datum_creatie_not, datum_operationeel=datum_operationeel, datum_operationeel_gt=datum_operationeel_gt, datum_operationeel_gte=datum_operationeel_gte, datum_operationeel_in=datum_operationeel_in, datum_operationeel_isnull=datum_operationeel_isnull, datum_operationeel_lt=datum_operationeel_lt, datum_operationeel_lte=datum_operationeel_lte, datum_operationeel_not=datum_operationeel_not, datum_oplevering=datum_oplevering, datum_oplevering_gt=datum_oplevering_gt, datum_oplevering_gte=datum_oplevering_gte, datum_oplevering_in=datum_oplevering_in, datum_oplevering_isnull=datum_oplevering_isnull, datum_oplevering_lt=datum_oplevering_lt, datum_oplevering_lte=datum_oplevering_lte, datum_oplevering_not=datum_oplevering_not, datum_plaatsing=datum_plaatsing, datum_plaatsing_gt=datum_plaatsing_gt, datum_plaatsing_gte=datum_plaatsing_gte, datum_plaatsing_in=datum_plaatsing_in, datum_plaatsing_isnull=datum_plaatsing_isnull, datum_plaatsing_lt=datum_plaatsing_lt, datum_plaatsing_lte=datum_plaatsing_lte, datum_plaatsing_not=datum_plaatsing_not, eigenaar_id=eigenaar_id, eigenaar_id_in=eigenaar_id_in, eigenaar_id_isempty=eigenaar_id_isempty, eigenaar_id_isnull=eigenaar_id_isnull, eigenaar_id_like=eigenaar_id_like, eigenaar_id_not=eigenaar_id_not, eigenaar_naam=eigenaar_naam, eigenaar_naam_in=eigenaar_naam_in, eigenaar_naam_isempty=eigenaar_naam_isempty, eigenaar_naam_isnull=eigenaar_naam_isnull, eigenaar_naam_like=eigenaar_naam_like, eigenaar_naam_not=eigenaar_naam_not, fractie_code=fractie_code, fractie_code_in=fractie_code_in, fractie_code_isempty=fractie_code_isempty, fractie_code_isnull=fractie_code_isnull, fractie_code_like=fractie_code_like, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geadopteerd_ind=geadopteerd_ind, geadopteerd_ind_isnull=geadopteerd_ind_isnull, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_nummer=id_nummer, id_nummer_in=id_nummer_in, id_nummer_isempty=id_nummer_isempty, id_nummer_isnull=id_nummer_isnull, id_nummer_like=id_nummer_like, id_nummer_not=id_nummer_not, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, locatie_id=locatie_id, locatie_id_in=locatie_id_in, locatie_id_isempty=locatie_id_isempty, locatie_id_isnull=locatie_id_isnull, locatie_id_like=locatie_id_like, locatie_id_not=locatie_id_not, page=page, serienummer=serienummer, serienummer_in=serienummer_in, serienummer_isempty=serienummer_isempty, serienummer_isnull=serienummer_isnull, serienummer_like=serienummer_like, serienummer_not=serienummer_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, type_id=type_id, type_id_in=type_id_in, type_id_isempty=type_id_isempty, type_id_isnull=type_id_isnull, type_id_like=type_id_like, type_id_not=type_id_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ContainerApi->huishoudelijkafval_container_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContainerApi->huishoudelijkafval_container_list2: %s\n" % e)
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
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_chip_nummber** | **str**| Het identificatienummer van de chip die registreert wanneer de container wordt geleegd. | [optional] 
 **container_chip_nummber_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_chip_nummber_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_chip_nummber_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_chip_nummber_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_chip_nummber_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_datum_vervanging** | **date**| De datum waarop de container wordt vervangen. | [optional] 
 **container_datum_vervanging_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **container_datum_vervanging_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **container_datum_vervanging_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_datum_vervanging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_datum_vervanging_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **container_datum_vervanging_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **container_datum_vervanging_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **container_datum_wijziging** | **datetime**| Datum waarop de container is gewijzigd. | [optional] 
 **container_datum_wijziging_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_datum_wijziging_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_datum_wijziging_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_datum_wijziging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_datum_wijziging_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_datum_wijziging_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_datum_wijziging_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_eigenaarschap** | **str**| De soort eigenaarschap van het object. | [optional] 
 **container_eigenaarschap_opmerking** | **str**| Beschrijving van  het type eigenaarschap. | [optional] 
 **container_eigenaarschap_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_eigenaarschap_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_eigenaarschap_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_eigenaarschap_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_eigenaarschap_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_eigenaarschap_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_eigenaarschap_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_eigenaarschap_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_eigenaarschap_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_eigenaarschap_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_end_of_life** | **date**| Datum waarop het object het einde van zijn levenscyclus heeft bereikt. | [optional] 
 **container_end_of_life_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **container_end_of_life_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **container_end_of_life_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_end_of_life_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_end_of_life_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **container_end_of_life_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **container_end_of_life_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **container_kleur** | **str**| De naam van de kleur | [optional] 
 **container_kleur_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_kleur_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_kleur_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_kleur_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_kleur_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_mark** | **int**| Definitie volgt nog | [optional] 
 **container_mark_gt** | **int**| Greater than; number | [optional] 
 **container_mark_gte** | **int**| Greater than or equal to; number | [optional] 
 **container_mark_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_mark_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_mark_lt** | **int**| Less than; number | [optional] 
 **container_mark_lte** | **int**| Less than or equal to; number | [optional] 
 **container_mark_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **container_opmerking** | **str**| Opmerking over het object door de betrokken medewerker. | [optional] 
 **container_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_ral_kleur_code** | **str**| De internationale ralkleurcode. | [optional] 
 **container_ral_kleur_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_ral_kleur_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_ral_kleur_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_ral_kleur_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_ral_kleur_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_ral_kleur_hexcode** | **str**| De hexcode van de ralkleur. | [optional] 
 **container_ral_kleur_hexcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_ral_kleur_hexcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_ral_kleur_hexcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_ral_kleur_hexcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_ral_kleur_hexcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_ral_kleur_naam** | **str**| De naam van de ralkleur | [optional] 
 **container_ral_kleur_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_ral_kleur_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_ral_kleur_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_ral_kleur_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_ral_kleur_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_unit_card_lezer_id** | **str**| Het identificatienummer van de kaartlezer. | [optional] 
 **container_unit_card_lezer_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_unit_card_lezer_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_unit_card_lezer_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_unit_card_lezer_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_unit_card_lezer_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_aflopen_garantie** | **date**| Datum waarop de garantie verloopt | [optional] 
 **datum_aflopen_garantie_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_aflopen_garantie_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_aflopen_garantie_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_aflopen_garantie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_aflopen_garantie_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_aflopen_garantie_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_aflopen_garantie_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_creatie** | **date**| Datum waarop het object is gecreëerd in container management systeem | [optional] 
 **datum_creatie_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_creatie_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_creatie_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_creatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_creatie_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_creatie_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_creatie_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_operationeel** | **date**| Datum dat de container operationeel is voor het aanbieden van afval | [optional] 
 **datum_operationeel_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_operationeel_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_operationeel_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_operationeel_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_operationeel_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_operationeel_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_operationeel_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_oplevering** | **date**| Datum waarop het object is geleverd | [optional] 
 **datum_oplevering_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_oplevering_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_oplevering_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_oplevering_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_oplevering_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_oplevering_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_oplevering_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_plaatsing** | **date**| Datum waarop het object op de locatie is geplaatst | [optional] 
 **datum_plaatsing_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_plaatsing_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_plaatsing_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_plaatsing_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_plaatsing_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_plaatsing_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_plaatsing_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
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
 **fractie_code** | **str**| Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood | [optional] 
 **fractie_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **fractie_omschrijving** | **str**| Container fractieomschrijving zoals door leverancier is geleverd. | [optional] 
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
 **geadopteerd_ind** | **bool**| indicatie of het object door een bewoner geadopteerd is | [optional] 
 **geadopteerd_ind_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de container RD (epsg:28992) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id** | **str**| Unieke aanduiding objecttype | [optional] 
 **id_nummer** | **str**| Identificatie dat door de fabrikant aan het object is gegeven | [optional] 
 **id_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **locatie_id** | **str**| Identificerend kenmerk van de put waarin de container is geplaatst | [optional] 
 **locatie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **locatie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **locatie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **locatie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **locatie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **serienummer** | **str**| serienummer uitgegeven door de fabrikant | [optional] 
 **serienummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **serienummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **serienummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **serienummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **serienummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **int**| Status van de container,0 - inactief, 1 - actief, 2 - gepland | [optional] 
 **status_gt** | **int**| Greater than; number | [optional] 
 **status_gte** | **int**| Greater than or equal to; number | [optional] 
 **status_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_lt** | **int**| Less than; number | [optional] 
 **status_lte** | **int**| Less than or equal to; number | [optional] 
 **status_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **type_id** | **str**| Unieke aanduiding objecttype | [optional] 
 **type_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **type_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **type_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **type_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **type_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
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

[**PaginatedHuishoudelijkafvalcontainerList**](PaginatedHuishoudelijkafvalcontainerList.md)

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

# **huishoudelijkafval_container_retrieve2**
> Huishoudelijkafvalcontainer huishoudelijkafval_container_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, container_chip_nummber=container_chip_nummber, container_chip_nummber_in=container_chip_nummber_in, container_chip_nummber_isempty=container_chip_nummber_isempty, container_chip_nummber_isnull=container_chip_nummber_isnull, container_chip_nummber_like=container_chip_nummber_like, container_chip_nummber_not=container_chip_nummber_not, container_datum_vervanging=container_datum_vervanging, container_datum_vervanging_gt=container_datum_vervanging_gt, container_datum_vervanging_gte=container_datum_vervanging_gte, container_datum_vervanging_in=container_datum_vervanging_in, container_datum_vervanging_isnull=container_datum_vervanging_isnull, container_datum_vervanging_lt=container_datum_vervanging_lt, container_datum_vervanging_lte=container_datum_vervanging_lte, container_datum_vervanging_not=container_datum_vervanging_not, container_datum_wijziging=container_datum_wijziging, container_datum_wijziging_gt=container_datum_wijziging_gt, container_datum_wijziging_gte=container_datum_wijziging_gte, container_datum_wijziging_in=container_datum_wijziging_in, container_datum_wijziging_isnull=container_datum_wijziging_isnull, container_datum_wijziging_lt=container_datum_wijziging_lt, container_datum_wijziging_lte=container_datum_wijziging_lte, container_datum_wijziging_not=container_datum_wijziging_not, container_eigenaarschap=container_eigenaarschap, container_eigenaarschap_opmerking=container_eigenaarschap_opmerking, container_eigenaarschap_opmerking_in=container_eigenaarschap_opmerking_in, container_eigenaarschap_opmerking_isempty=container_eigenaarschap_opmerking_isempty, container_eigenaarschap_opmerking_isnull=container_eigenaarschap_opmerking_isnull, container_eigenaarschap_opmerking_like=container_eigenaarschap_opmerking_like, container_eigenaarschap_opmerking_not=container_eigenaarschap_opmerking_not, container_eigenaarschap_in=container_eigenaarschap_in, container_eigenaarschap_isempty=container_eigenaarschap_isempty, container_eigenaarschap_isnull=container_eigenaarschap_isnull, container_eigenaarschap_like=container_eigenaarschap_like, container_eigenaarschap_not=container_eigenaarschap_not, container_end_of_life=container_end_of_life, container_end_of_life_gt=container_end_of_life_gt, container_end_of_life_gte=container_end_of_life_gte, container_end_of_life_in=container_end_of_life_in, container_end_of_life_isnull=container_end_of_life_isnull, container_end_of_life_lt=container_end_of_life_lt, container_end_of_life_lte=container_end_of_life_lte, container_end_of_life_not=container_end_of_life_not, container_kleur=container_kleur, container_kleur_in=container_kleur_in, container_kleur_isempty=container_kleur_isempty, container_kleur_isnull=container_kleur_isnull, container_kleur_like=container_kleur_like, container_kleur_not=container_kleur_not, container_mark=container_mark, container_mark_gt=container_mark_gt, container_mark_gte=container_mark_gte, container_mark_in=container_mark_in, container_mark_isnull=container_mark_isnull, container_mark_lt=container_mark_lt, container_mark_lte=container_mark_lte, container_mark_not=container_mark_not, container_opmerking=container_opmerking, container_opmerking_in=container_opmerking_in, container_opmerking_isempty=container_opmerking_isempty, container_opmerking_isnull=container_opmerking_isnull, container_opmerking_like=container_opmerking_like, container_opmerking_not=container_opmerking_not, container_ral_kleur_code=container_ral_kleur_code, container_ral_kleur_code_in=container_ral_kleur_code_in, container_ral_kleur_code_isempty=container_ral_kleur_code_isempty, container_ral_kleur_code_isnull=container_ral_kleur_code_isnull, container_ral_kleur_code_like=container_ral_kleur_code_like, container_ral_kleur_code_not=container_ral_kleur_code_not, container_ral_kleur_hexcode=container_ral_kleur_hexcode, container_ral_kleur_hexcode_in=container_ral_kleur_hexcode_in, container_ral_kleur_hexcode_isempty=container_ral_kleur_hexcode_isempty, container_ral_kleur_hexcode_isnull=container_ral_kleur_hexcode_isnull, container_ral_kleur_hexcode_like=container_ral_kleur_hexcode_like, container_ral_kleur_hexcode_not=container_ral_kleur_hexcode_not, container_ral_kleur_naam=container_ral_kleur_naam, container_ral_kleur_naam_in=container_ral_kleur_naam_in, container_ral_kleur_naam_isempty=container_ral_kleur_naam_isempty, container_ral_kleur_naam_isnull=container_ral_kleur_naam_isnull, container_ral_kleur_naam_like=container_ral_kleur_naam_like, container_ral_kleur_naam_not=container_ral_kleur_naam_not, container_unit_card_lezer_id=container_unit_card_lezer_id, container_unit_card_lezer_id_in=container_unit_card_lezer_id_in, container_unit_card_lezer_id_isempty=container_unit_card_lezer_id_isempty, container_unit_card_lezer_id_isnull=container_unit_card_lezer_id_isnull, container_unit_card_lezer_id_like=container_unit_card_lezer_id_like, container_unit_card_lezer_id_not=container_unit_card_lezer_id_not, datum_aflopen_garantie=datum_aflopen_garantie, datum_aflopen_garantie_gt=datum_aflopen_garantie_gt, datum_aflopen_garantie_gte=datum_aflopen_garantie_gte, datum_aflopen_garantie_in=datum_aflopen_garantie_in, datum_aflopen_garantie_isnull=datum_aflopen_garantie_isnull, datum_aflopen_garantie_lt=datum_aflopen_garantie_lt, datum_aflopen_garantie_lte=datum_aflopen_garantie_lte, datum_aflopen_garantie_not=datum_aflopen_garantie_not, datum_creatie=datum_creatie, datum_creatie_gt=datum_creatie_gt, datum_creatie_gte=datum_creatie_gte, datum_creatie_in=datum_creatie_in, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_lt=datum_creatie_lt, datum_creatie_lte=datum_creatie_lte, datum_creatie_not=datum_creatie_not, datum_operationeel=datum_operationeel, datum_operationeel_gt=datum_operationeel_gt, datum_operationeel_gte=datum_operationeel_gte, datum_operationeel_in=datum_operationeel_in, datum_operationeel_isnull=datum_operationeel_isnull, datum_operationeel_lt=datum_operationeel_lt, datum_operationeel_lte=datum_operationeel_lte, datum_operationeel_not=datum_operationeel_not, datum_oplevering=datum_oplevering, datum_oplevering_gt=datum_oplevering_gt, datum_oplevering_gte=datum_oplevering_gte, datum_oplevering_in=datum_oplevering_in, datum_oplevering_isnull=datum_oplevering_isnull, datum_oplevering_lt=datum_oplevering_lt, datum_oplevering_lte=datum_oplevering_lte, datum_oplevering_not=datum_oplevering_not, datum_plaatsing=datum_plaatsing, datum_plaatsing_gt=datum_plaatsing_gt, datum_plaatsing_gte=datum_plaatsing_gte, datum_plaatsing_in=datum_plaatsing_in, datum_plaatsing_isnull=datum_plaatsing_isnull, datum_plaatsing_lt=datum_plaatsing_lt, datum_plaatsing_lte=datum_plaatsing_lte, datum_plaatsing_not=datum_plaatsing_not, eigenaar_id=eigenaar_id, eigenaar_id_in=eigenaar_id_in, eigenaar_id_isempty=eigenaar_id_isempty, eigenaar_id_isnull=eigenaar_id_isnull, eigenaar_id_like=eigenaar_id_like, eigenaar_id_not=eigenaar_id_not, eigenaar_naam=eigenaar_naam, eigenaar_naam_in=eigenaar_naam_in, eigenaar_naam_isempty=eigenaar_naam_isempty, eigenaar_naam_isnull=eigenaar_naam_isnull, eigenaar_naam_like=eigenaar_naam_like, eigenaar_naam_not=eigenaar_naam_not, fractie_code=fractie_code, fractie_code_in=fractie_code_in, fractie_code_isempty=fractie_code_isempty, fractie_code_isnull=fractie_code_isnull, fractie_code_like=fractie_code_like, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geadopteerd_ind=geadopteerd_ind, geadopteerd_ind_isnull=geadopteerd_ind_isnull, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_nummer=id_nummer, id_nummer_in=id_nummer_in, id_nummer_isempty=id_nummer_isempty, id_nummer_isnull=id_nummer_isnull, id_nummer_like=id_nummer_like, id_nummer_not=id_nummer_not, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, locatie_id=locatie_id, locatie_id_in=locatie_id_in, locatie_id_isempty=locatie_id_isempty, locatie_id_isnull=locatie_id_isnull, locatie_id_like=locatie_id_like, locatie_id_not=locatie_id_not, serienummer=serienummer, serienummer_in=serienummer_in, serienummer_isempty=serienummer_isempty, serienummer_isnull=serienummer_isnull, serienummer_like=serienummer_like, serienummer_not=serienummer_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, type_id=type_id, type_id_in=type_id_in, type_id_isempty=type_id_isempty, type_id_isnull=type_id_isnull, type_id_like=type_id_like, type_id_not=type_id_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalcontainer import Huishoudelijkafvalcontainer
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
    api_instance = huishoudelijkafval_api_client.ContainerApi(api_client)
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
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
    container_chip_nummber = 'container_chip_nummber_example' # str | Het identificatienummer van de chip die registreert wanneer de container wordt geleegd. (optional)
    container_chip_nummber_in = ['container_chip_nummber_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_chip_nummber_isempty = True # bool | Whether the field is empty or not. (optional)
    container_chip_nummber_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_chip_nummber_like = 'container_chip_nummber_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_chip_nummber_not = ['container_chip_nummber_not_example'] # List[str] | Exclude matches; text (optional)
    container_datum_vervanging = '2013-10-20' # date | De datum waarop de container wordt vervangen. (optional)
    container_datum_vervanging_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    container_datum_vervanging_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    container_datum_vervanging_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_datum_vervanging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_datum_vervanging_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    container_datum_vervanging_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    container_datum_vervanging_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    container_datum_wijziging = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop de container is gewijzigd. (optional)
    container_datum_wijziging_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_datum_wijziging_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_datum_wijziging_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_datum_wijziging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_datum_wijziging_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_datum_wijziging_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_datum_wijziging_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    container_eigenaarschap = 'container_eigenaarschap_example' # str | De soort eigenaarschap van het object. (optional)
    container_eigenaarschap_opmerking = 'container_eigenaarschap_opmerking_example' # str | Beschrijving van  het type eigenaarschap. (optional)
    container_eigenaarschap_opmerking_in = ['container_eigenaarschap_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_eigenaarschap_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    container_eigenaarschap_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_eigenaarschap_opmerking_like = 'container_eigenaarschap_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_eigenaarschap_opmerking_not = ['container_eigenaarschap_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    container_eigenaarschap_in = ['container_eigenaarschap_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_eigenaarschap_isempty = True # bool | Whether the field is empty or not. (optional)
    container_eigenaarschap_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_eigenaarschap_like = 'container_eigenaarschap_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_eigenaarschap_not = ['container_eigenaarschap_not_example'] # List[str] | Exclude matches; text (optional)
    container_end_of_life = '2013-10-20' # date | Datum waarop het object het einde van zijn levenscyclus heeft bereikt. (optional)
    container_end_of_life_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    container_end_of_life_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    container_end_of_life_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_end_of_life_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_end_of_life_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    container_end_of_life_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    container_end_of_life_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    container_kleur = 'container_kleur_example' # str | De naam van de kleur (optional)
    container_kleur_in = ['container_kleur_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_kleur_isempty = True # bool | Whether the field is empty or not. (optional)
    container_kleur_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_kleur_like = 'container_kleur_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_kleur_not = ['container_kleur_not_example'] # List[str] | Exclude matches; text (optional)
    container_mark = 56 # int | Definitie volgt nog (optional)
    container_mark_gt = 56 # int | Greater than; number (optional)
    container_mark_gte = 56 # int | Greater than or equal to; number (optional)
    container_mark_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_mark_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_mark_lt = 56 # int | Less than; number (optional)
    container_mark_lte = 56 # int | Less than or equal to; number (optional)
    container_mark_not = [56] # List[int] | Exclude matches; number (optional)
    container_opmerking = 'container_opmerking_example' # str | Opmerking over het object door de betrokken medewerker. (optional)
    container_opmerking_in = ['container_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    container_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_opmerking_like = 'container_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_opmerking_not = ['container_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    container_ral_kleur_code = 'container_ral_kleur_code_example' # str | De internationale ralkleurcode. (optional)
    container_ral_kleur_code_in = ['container_ral_kleur_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_ral_kleur_code_isempty = True # bool | Whether the field is empty or not. (optional)
    container_ral_kleur_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_ral_kleur_code_like = 'container_ral_kleur_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_ral_kleur_code_not = ['container_ral_kleur_code_not_example'] # List[str] | Exclude matches; text (optional)
    container_ral_kleur_hexcode = 'container_ral_kleur_hexcode_example' # str | De hexcode van de ralkleur. (optional)
    container_ral_kleur_hexcode_in = ['container_ral_kleur_hexcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_ral_kleur_hexcode_isempty = True # bool | Whether the field is empty or not. (optional)
    container_ral_kleur_hexcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_ral_kleur_hexcode_like = 'container_ral_kleur_hexcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_ral_kleur_hexcode_not = ['container_ral_kleur_hexcode_not_example'] # List[str] | Exclude matches; text (optional)
    container_ral_kleur_naam = 'container_ral_kleur_naam_example' # str | De naam van de ralkleur (optional)
    container_ral_kleur_naam_in = ['container_ral_kleur_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_ral_kleur_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    container_ral_kleur_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_ral_kleur_naam_like = 'container_ral_kleur_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_ral_kleur_naam_not = ['container_ral_kleur_naam_not_example'] # List[str] | Exclude matches; text (optional)
    container_unit_card_lezer_id = 'container_unit_card_lezer_id_example' # str | Het identificatienummer van de kaartlezer. (optional)
    container_unit_card_lezer_id_in = ['container_unit_card_lezer_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_unit_card_lezer_id_isempty = True # bool | Whether the field is empty or not. (optional)
    container_unit_card_lezer_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_unit_card_lezer_id_like = 'container_unit_card_lezer_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_unit_card_lezer_id_not = ['container_unit_card_lezer_id_not_example'] # List[str] | Exclude matches; text (optional)
    datum_aflopen_garantie = '2013-10-20' # date | Datum waarop de garantie verloopt (optional)
    datum_aflopen_garantie_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_aflopen_garantie_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_aflopen_garantie_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_aflopen_garantie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_aflopen_garantie_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_aflopen_garantie_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_aflopen_garantie_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_creatie = '2013-10-20' # date | Datum waarop het object is gecreëerd in container management systeem (optional)
    datum_creatie_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_creatie_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_creatie_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_creatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_creatie_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_creatie_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_creatie_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_operationeel = '2013-10-20' # date | Datum dat de container operationeel is voor het aanbieden van afval (optional)
    datum_operationeel_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_operationeel_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_operationeel_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_operationeel_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_operationeel_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_operationeel_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_operationeel_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_oplevering = '2013-10-20' # date | Datum waarop het object is geleverd (optional)
    datum_oplevering_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_oplevering_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_oplevering_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_oplevering_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_oplevering_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_oplevering_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_oplevering_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_plaatsing = '2013-10-20' # date | Datum waarop het object op de locatie is geplaatst (optional)
    datum_plaatsing_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_plaatsing_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_plaatsing_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_plaatsing_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_plaatsing_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_plaatsing_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_plaatsing_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
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
    fractie_code = 'fractie_code_example' # str | Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood (optional)
    fractie_code_in = ['fractie_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_code_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_code_like = 'fractie_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_code_not = ['fractie_code_not_example'] # List[str] | Exclude matches; text (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Container fractieomschrijving zoals door leverancier is geleverd. (optional)
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
    geadopteerd_ind = True # bool | indicatie of het object door een bewoner geadopteerd is (optional)
    geadopteerd_ind_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de container RD (epsg:28992) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id2 = 'id_example' # str | Unieke aanduiding objecttype (optional)
    id_nummer = 'id_nummer_example' # str | Identificatie dat door de fabrikant aan het object is gegeven (optional)
    id_nummer_in = ['id_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    id_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_nummer_like = 'id_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_nummer_not = ['id_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    locatie_id = 'locatie_id_example' # str | Identificerend kenmerk van de put waarin de container is geplaatst (optional)
    locatie_id_in = ['locatie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    locatie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    locatie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    locatie_id_like = 'locatie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    locatie_id_not = ['locatie_id_not_example'] # List[str] | Exclude matches; text (optional)
    serienummer = 'serienummer_example' # str | serienummer uitgegeven door de fabrikant (optional)
    serienummer_in = ['serienummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    serienummer_isempty = True # bool | Whether the field is empty or not. (optional)
    serienummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    serienummer_like = 'serienummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    serienummer_not = ['serienummer_not_example'] # List[str] | Exclude matches; text (optional)
    status = 56 # int | Status van de container,0 - inactief, 1 - actief, 2 - gepland (optional)
    status_gt = 56 # int | Greater than; number (optional)
    status_gte = 56 # int | Greater than or equal to; number (optional)
    status_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_lt = 56 # int | Less than; number (optional)
    status_lte = 56 # int | Less than or equal to; number (optional)
    status_not = [56] # List[int] | Exclude matches; number (optional)
    type_id = 'type_id_example' # str | Unieke aanduiding objecttype (optional)
    type_id_in = ['type_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    type_id_isempty = True # bool | Whether the field is empty or not. (optional)
    type_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    type_id_like = 'type_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    type_id_not = ['type_id_not_example'] # List[str] | Exclude matches; text (optional)
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
        api_response = await api_instance.huishoudelijkafval_container_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, container_chip_nummber=container_chip_nummber, container_chip_nummber_in=container_chip_nummber_in, container_chip_nummber_isempty=container_chip_nummber_isempty, container_chip_nummber_isnull=container_chip_nummber_isnull, container_chip_nummber_like=container_chip_nummber_like, container_chip_nummber_not=container_chip_nummber_not, container_datum_vervanging=container_datum_vervanging, container_datum_vervanging_gt=container_datum_vervanging_gt, container_datum_vervanging_gte=container_datum_vervanging_gte, container_datum_vervanging_in=container_datum_vervanging_in, container_datum_vervanging_isnull=container_datum_vervanging_isnull, container_datum_vervanging_lt=container_datum_vervanging_lt, container_datum_vervanging_lte=container_datum_vervanging_lte, container_datum_vervanging_not=container_datum_vervanging_not, container_datum_wijziging=container_datum_wijziging, container_datum_wijziging_gt=container_datum_wijziging_gt, container_datum_wijziging_gte=container_datum_wijziging_gte, container_datum_wijziging_in=container_datum_wijziging_in, container_datum_wijziging_isnull=container_datum_wijziging_isnull, container_datum_wijziging_lt=container_datum_wijziging_lt, container_datum_wijziging_lte=container_datum_wijziging_lte, container_datum_wijziging_not=container_datum_wijziging_not, container_eigenaarschap=container_eigenaarschap, container_eigenaarschap_opmerking=container_eigenaarschap_opmerking, container_eigenaarschap_opmerking_in=container_eigenaarschap_opmerking_in, container_eigenaarschap_opmerking_isempty=container_eigenaarschap_opmerking_isempty, container_eigenaarschap_opmerking_isnull=container_eigenaarschap_opmerking_isnull, container_eigenaarschap_opmerking_like=container_eigenaarschap_opmerking_like, container_eigenaarschap_opmerking_not=container_eigenaarschap_opmerking_not, container_eigenaarschap_in=container_eigenaarschap_in, container_eigenaarschap_isempty=container_eigenaarschap_isempty, container_eigenaarschap_isnull=container_eigenaarschap_isnull, container_eigenaarschap_like=container_eigenaarschap_like, container_eigenaarschap_not=container_eigenaarschap_not, container_end_of_life=container_end_of_life, container_end_of_life_gt=container_end_of_life_gt, container_end_of_life_gte=container_end_of_life_gte, container_end_of_life_in=container_end_of_life_in, container_end_of_life_isnull=container_end_of_life_isnull, container_end_of_life_lt=container_end_of_life_lt, container_end_of_life_lte=container_end_of_life_lte, container_end_of_life_not=container_end_of_life_not, container_kleur=container_kleur, container_kleur_in=container_kleur_in, container_kleur_isempty=container_kleur_isempty, container_kleur_isnull=container_kleur_isnull, container_kleur_like=container_kleur_like, container_kleur_not=container_kleur_not, container_mark=container_mark, container_mark_gt=container_mark_gt, container_mark_gte=container_mark_gte, container_mark_in=container_mark_in, container_mark_isnull=container_mark_isnull, container_mark_lt=container_mark_lt, container_mark_lte=container_mark_lte, container_mark_not=container_mark_not, container_opmerking=container_opmerking, container_opmerking_in=container_opmerking_in, container_opmerking_isempty=container_opmerking_isempty, container_opmerking_isnull=container_opmerking_isnull, container_opmerking_like=container_opmerking_like, container_opmerking_not=container_opmerking_not, container_ral_kleur_code=container_ral_kleur_code, container_ral_kleur_code_in=container_ral_kleur_code_in, container_ral_kleur_code_isempty=container_ral_kleur_code_isempty, container_ral_kleur_code_isnull=container_ral_kleur_code_isnull, container_ral_kleur_code_like=container_ral_kleur_code_like, container_ral_kleur_code_not=container_ral_kleur_code_not, container_ral_kleur_hexcode=container_ral_kleur_hexcode, container_ral_kleur_hexcode_in=container_ral_kleur_hexcode_in, container_ral_kleur_hexcode_isempty=container_ral_kleur_hexcode_isempty, container_ral_kleur_hexcode_isnull=container_ral_kleur_hexcode_isnull, container_ral_kleur_hexcode_like=container_ral_kleur_hexcode_like, container_ral_kleur_hexcode_not=container_ral_kleur_hexcode_not, container_ral_kleur_naam=container_ral_kleur_naam, container_ral_kleur_naam_in=container_ral_kleur_naam_in, container_ral_kleur_naam_isempty=container_ral_kleur_naam_isempty, container_ral_kleur_naam_isnull=container_ral_kleur_naam_isnull, container_ral_kleur_naam_like=container_ral_kleur_naam_like, container_ral_kleur_naam_not=container_ral_kleur_naam_not, container_unit_card_lezer_id=container_unit_card_lezer_id, container_unit_card_lezer_id_in=container_unit_card_lezer_id_in, container_unit_card_lezer_id_isempty=container_unit_card_lezer_id_isempty, container_unit_card_lezer_id_isnull=container_unit_card_lezer_id_isnull, container_unit_card_lezer_id_like=container_unit_card_lezer_id_like, container_unit_card_lezer_id_not=container_unit_card_lezer_id_not, datum_aflopen_garantie=datum_aflopen_garantie, datum_aflopen_garantie_gt=datum_aflopen_garantie_gt, datum_aflopen_garantie_gte=datum_aflopen_garantie_gte, datum_aflopen_garantie_in=datum_aflopen_garantie_in, datum_aflopen_garantie_isnull=datum_aflopen_garantie_isnull, datum_aflopen_garantie_lt=datum_aflopen_garantie_lt, datum_aflopen_garantie_lte=datum_aflopen_garantie_lte, datum_aflopen_garantie_not=datum_aflopen_garantie_not, datum_creatie=datum_creatie, datum_creatie_gt=datum_creatie_gt, datum_creatie_gte=datum_creatie_gte, datum_creatie_in=datum_creatie_in, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_lt=datum_creatie_lt, datum_creatie_lte=datum_creatie_lte, datum_creatie_not=datum_creatie_not, datum_operationeel=datum_operationeel, datum_operationeel_gt=datum_operationeel_gt, datum_operationeel_gte=datum_operationeel_gte, datum_operationeel_in=datum_operationeel_in, datum_operationeel_isnull=datum_operationeel_isnull, datum_operationeel_lt=datum_operationeel_lt, datum_operationeel_lte=datum_operationeel_lte, datum_operationeel_not=datum_operationeel_not, datum_oplevering=datum_oplevering, datum_oplevering_gt=datum_oplevering_gt, datum_oplevering_gte=datum_oplevering_gte, datum_oplevering_in=datum_oplevering_in, datum_oplevering_isnull=datum_oplevering_isnull, datum_oplevering_lt=datum_oplevering_lt, datum_oplevering_lte=datum_oplevering_lte, datum_oplevering_not=datum_oplevering_not, datum_plaatsing=datum_plaatsing, datum_plaatsing_gt=datum_plaatsing_gt, datum_plaatsing_gte=datum_plaatsing_gte, datum_plaatsing_in=datum_plaatsing_in, datum_plaatsing_isnull=datum_plaatsing_isnull, datum_plaatsing_lt=datum_plaatsing_lt, datum_plaatsing_lte=datum_plaatsing_lte, datum_plaatsing_not=datum_plaatsing_not, eigenaar_id=eigenaar_id, eigenaar_id_in=eigenaar_id_in, eigenaar_id_isempty=eigenaar_id_isempty, eigenaar_id_isnull=eigenaar_id_isnull, eigenaar_id_like=eigenaar_id_like, eigenaar_id_not=eigenaar_id_not, eigenaar_naam=eigenaar_naam, eigenaar_naam_in=eigenaar_naam_in, eigenaar_naam_isempty=eigenaar_naam_isempty, eigenaar_naam_isnull=eigenaar_naam_isnull, eigenaar_naam_like=eigenaar_naam_like, eigenaar_naam_not=eigenaar_naam_not, fractie_code=fractie_code, fractie_code_in=fractie_code_in, fractie_code_isempty=fractie_code_isempty, fractie_code_isnull=fractie_code_isnull, fractie_code_like=fractie_code_like, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geadopteerd_ind=geadopteerd_ind, geadopteerd_ind_isnull=geadopteerd_ind_isnull, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_nummer=id_nummer, id_nummer_in=id_nummer_in, id_nummer_isempty=id_nummer_isempty, id_nummer_isnull=id_nummer_isnull, id_nummer_like=id_nummer_like, id_nummer_not=id_nummer_not, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, locatie_id=locatie_id, locatie_id_in=locatie_id_in, locatie_id_isempty=locatie_id_isempty, locatie_id_isnull=locatie_id_isnull, locatie_id_like=locatie_id_like, locatie_id_not=locatie_id_not, serienummer=serienummer, serienummer_in=serienummer_in, serienummer_isempty=serienummer_isempty, serienummer_isnull=serienummer_isnull, serienummer_like=serienummer_like, serienummer_not=serienummer_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, type_id=type_id, type_id_in=type_id_in, type_id_isempty=type_id_isempty, type_id_isnull=type_id_isnull, type_id_like=type_id_like, type_id_not=type_id_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ContainerApi->huishoudelijkafval_container_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContainerApi->huishoudelijkafval_container_retrieve2: %s\n" % e)
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
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_chip_nummber** | **str**| Het identificatienummer van de chip die registreert wanneer de container wordt geleegd. | [optional] 
 **container_chip_nummber_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_chip_nummber_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_chip_nummber_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_chip_nummber_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_chip_nummber_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_datum_vervanging** | **date**| De datum waarop de container wordt vervangen. | [optional] 
 **container_datum_vervanging_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **container_datum_vervanging_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **container_datum_vervanging_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_datum_vervanging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_datum_vervanging_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **container_datum_vervanging_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **container_datum_vervanging_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **container_datum_wijziging** | **datetime**| Datum waarop de container is gewijzigd. | [optional] 
 **container_datum_wijziging_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_datum_wijziging_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_datum_wijziging_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_datum_wijziging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_datum_wijziging_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_datum_wijziging_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_datum_wijziging_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **container_eigenaarschap** | **str**| De soort eigenaarschap van het object. | [optional] 
 **container_eigenaarschap_opmerking** | **str**| Beschrijving van  het type eigenaarschap. | [optional] 
 **container_eigenaarschap_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_eigenaarschap_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_eigenaarschap_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_eigenaarschap_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_eigenaarschap_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_eigenaarschap_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_eigenaarschap_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_eigenaarschap_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_eigenaarschap_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_eigenaarschap_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_end_of_life** | **date**| Datum waarop het object het einde van zijn levenscyclus heeft bereikt. | [optional] 
 **container_end_of_life_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **container_end_of_life_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **container_end_of_life_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_end_of_life_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_end_of_life_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **container_end_of_life_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **container_end_of_life_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **container_kleur** | **str**| De naam van de kleur | [optional] 
 **container_kleur_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_kleur_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_kleur_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_kleur_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_kleur_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_mark** | **int**| Definitie volgt nog | [optional] 
 **container_mark_gt** | **int**| Greater than; number | [optional] 
 **container_mark_gte** | **int**| Greater than or equal to; number | [optional] 
 **container_mark_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_mark_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_mark_lt** | **int**| Less than; number | [optional] 
 **container_mark_lte** | **int**| Less than or equal to; number | [optional] 
 **container_mark_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **container_opmerking** | **str**| Opmerking over het object door de betrokken medewerker. | [optional] 
 **container_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_ral_kleur_code** | **str**| De internationale ralkleurcode. | [optional] 
 **container_ral_kleur_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_ral_kleur_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_ral_kleur_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_ral_kleur_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_ral_kleur_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_ral_kleur_hexcode** | **str**| De hexcode van de ralkleur. | [optional] 
 **container_ral_kleur_hexcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_ral_kleur_hexcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_ral_kleur_hexcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_ral_kleur_hexcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_ral_kleur_hexcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_ral_kleur_naam** | **str**| De naam van de ralkleur | [optional] 
 **container_ral_kleur_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_ral_kleur_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_ral_kleur_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_ral_kleur_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_ral_kleur_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **container_unit_card_lezer_id** | **str**| Het identificatienummer van de kaartlezer. | [optional] 
 **container_unit_card_lezer_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_unit_card_lezer_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_unit_card_lezer_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_unit_card_lezer_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_unit_card_lezer_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_aflopen_garantie** | **date**| Datum waarop de garantie verloopt | [optional] 
 **datum_aflopen_garantie_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_aflopen_garantie_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_aflopen_garantie_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_aflopen_garantie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_aflopen_garantie_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_aflopen_garantie_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_aflopen_garantie_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_creatie** | **date**| Datum waarop het object is gecreëerd in container management systeem | [optional] 
 **datum_creatie_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_creatie_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_creatie_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_creatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_creatie_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_creatie_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_creatie_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_operationeel** | **date**| Datum dat de container operationeel is voor het aanbieden van afval | [optional] 
 **datum_operationeel_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_operationeel_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_operationeel_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_operationeel_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_operationeel_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_operationeel_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_operationeel_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_oplevering** | **date**| Datum waarop het object is geleverd | [optional] 
 **datum_oplevering_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_oplevering_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_oplevering_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_oplevering_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_oplevering_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_oplevering_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_oplevering_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_plaatsing** | **date**| Datum waarop het object op de locatie is geplaatst | [optional] 
 **datum_plaatsing_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_plaatsing_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_plaatsing_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_plaatsing_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_plaatsing_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_plaatsing_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_plaatsing_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
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
 **fractie_code** | **str**| Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood | [optional] 
 **fractie_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **fractie_omschrijving** | **str**| Container fractieomschrijving zoals door leverancier is geleverd. | [optional] 
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
 **geadopteerd_ind** | **bool**| indicatie of het object door een bewoner geadopteerd is | [optional] 
 **geadopteerd_ind_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de container RD (epsg:28992) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id2** | **str**| Unieke aanduiding objecttype | [optional] 
 **id_nummer** | **str**| Identificatie dat door de fabrikant aan het object is gegeven | [optional] 
 **id_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **locatie_id** | **str**| Identificerend kenmerk van de put waarin de container is geplaatst | [optional] 
 **locatie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **locatie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **locatie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **locatie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **locatie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **serienummer** | **str**| serienummer uitgegeven door de fabrikant | [optional] 
 **serienummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **serienummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **serienummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **serienummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **serienummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **int**| Status van de container,0 - inactief, 1 - actief, 2 - gepland | [optional] 
 **status_gt** | **int**| Greater than; number | [optional] 
 **status_gte** | **int**| Greater than or equal to; number | [optional] 
 **status_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_lt** | **int**| Less than; number | [optional] 
 **status_lte** | **int**| Less than or equal to; number | [optional] 
 **status_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **type_id** | **str**| Unieke aanduiding objecttype | [optional] 
 **type_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **type_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **type_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **type_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **type_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
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

[**Huishoudelijkafvalcontainer**](Huishoudelijkafvalcontainer.md)

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

