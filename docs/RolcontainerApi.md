# huishoudelijkafval_api_client.RolcontainerApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_rolcontainer_list_slash**](RolcontainerApi.md#huishoudelijkafval_rolcontainer_list_slash) | **GET** /rolcontainer | 
[**huishoudelijkafval_rolcontainer_retrieve_slash**](RolcontainerApi.md#huishoudelijkafval_rolcontainer_retrieve_slash) | **GET** /rolcontainer/{id} | 


# **huishoudelijkafval_rolcontainer_list_slash**
> PaginatedHuishoudelijkafvalrolcontainerList huishoudelijkafval_rolcontainer_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bag_woonplaats_identificatie=bag_woonplaats_identificatie, bag_woonplaats_identificatie_in=bag_woonplaats_identificatie_in, bag_woonplaats_identificatie_isempty=bag_woonplaats_identificatie_isempty, bag_woonplaats_identificatie_isnull=bag_woonplaats_identificatie_isnull, bag_woonplaats_identificatie_like=bag_woonplaats_identificatie_like, bag_woonplaats_identificatie_not=bag_woonplaats_identificatie_not, barcode=barcode, barcode_in=barcode_in, barcode_isempty=barcode_isempty, barcode_isnull=barcode_isnull, barcode_like=barcode_like, barcode_not=barcode_not, chip_nummer=chip_nummer, chip_nummer_in=chip_nummer_in, chip_nummer_isempty=chip_nummer_isempty, chip_nummer_isnull=chip_nummer_isnull, chip_nummer_like=chip_nummer_like, chip_nummer_not=chip_nummer_not, chip_type=chip_type, chip_type_in=chip_type_in, chip_type_isempty=chip_type_isempty, chip_type_isnull=chip_type_isnull, chip_type_like=chip_type_like, chip_type_not=chip_type_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gebied_buurt_identificatie=gebied_buurt_identificatie, gebied_buurt_identificatie_in=gebied_buurt_identificatie_in, gebied_buurt_identificatie_isempty=gebied_buurt_identificatie_isempty, gebied_buurt_identificatie_isnull=gebied_buurt_identificatie_isnull, gebied_buurt_identificatie_like=gebied_buurt_identificatie_like, gebied_buurt_identificatie_not=gebied_buurt_identificatie_not, gebied_buurt_code=gebied_buurt_code, gebied_buurt_code_in=gebied_buurt_code_in, gebied_buurt_code_isempty=gebied_buurt_code_isempty, gebied_buurt_code_isnull=gebied_buurt_code_isnull, gebied_buurt_code_like=gebied_buurt_code_like, gebied_buurt_code_not=gebied_buurt_code_not, gebied_buurt_naam=gebied_buurt_naam, gebied_buurt_naam_in=gebied_buurt_naam_in, gebied_buurt_naam_isempty=gebied_buurt_naam_isempty, gebied_buurt_naam_isnull=gebied_buurt_naam_isnull, gebied_buurt_naam_like=gebied_buurt_naam_like, gebied_buurt_naam_not=gebied_buurt_naam_not, gebied_ggw_identificatie=gebied_ggw_identificatie, gebied_ggw_identificatie_in=gebied_ggw_identificatie_in, gebied_ggw_identificatie_isempty=gebied_ggw_identificatie_isempty, gebied_ggw_identificatie_isnull=gebied_ggw_identificatie_isnull, gebied_ggw_identificatie_like=gebied_ggw_identificatie_like, gebied_ggw_identificatie_not=gebied_ggw_identificatie_not, gebied_ggw_code=gebied_ggw_code, gebied_ggw_code_in=gebied_ggw_code_in, gebied_ggw_code_isempty=gebied_ggw_code_isempty, gebied_ggw_code_isnull=gebied_ggw_code_isnull, gebied_ggw_code_like=gebied_ggw_code_like, gebied_ggw_code_not=gebied_ggw_code_not, gebied_ggw_naam=gebied_ggw_naam, gebied_ggw_naam_in=gebied_ggw_naam_in, gebied_ggw_naam_isempty=gebied_ggw_naam_isempty, gebied_ggw_naam_isnull=gebied_ggw_naam_isnull, gebied_ggw_naam_like=gebied_ggw_naam_like, gebied_ggw_naam_not=gebied_ggw_naam_not, gebied_stadsdeel_identificatie=gebied_stadsdeel_identificatie, gebied_stadsdeel_identificatie_in=gebied_stadsdeel_identificatie_in, gebied_stadsdeel_identificatie_isempty=gebied_stadsdeel_identificatie_isempty, gebied_stadsdeel_identificatie_isnull=gebied_stadsdeel_identificatie_isnull, gebied_stadsdeel_identificatie_like=gebied_stadsdeel_identificatie_like, gebied_stadsdeel_identificatie_not=gebied_stadsdeel_identificatie_not, gebied_stadsdeel_code=gebied_stadsdeel_code, gebied_stadsdeel_code_in=gebied_stadsdeel_code_in, gebied_stadsdeel_code_isempty=gebied_stadsdeel_code_isempty, gebied_stadsdeel_code_isnull=gebied_stadsdeel_code_isnull, gebied_stadsdeel_code_like=gebied_stadsdeel_code_like, gebied_stadsdeel_code_not=gebied_stadsdeel_code_not, gebied_stadsdeel_naam=gebied_stadsdeel_naam, gebied_stadsdeel_naam_in=gebied_stadsdeel_naam_in, gebied_stadsdeel_naam_isempty=gebied_stadsdeel_naam_isempty, gebied_stadsdeel_naam_isnull=gebied_stadsdeel_naam_isnull, gebied_stadsdeel_naam_like=gebied_stadsdeel_naam_like, gebied_stadsdeel_naam_not=gebied_stadsdeel_naam_not, gebied_wijk_identificatie=gebied_wijk_identificatie, gebied_wijk_identificatie_in=gebied_wijk_identificatie_in, gebied_wijk_identificatie_isempty=gebied_wijk_identificatie_isempty, gebied_wijk_identificatie_isnull=gebied_wijk_identificatie_isnull, gebied_wijk_identificatie_like=gebied_wijk_identificatie_like, gebied_wijk_identificatie_not=gebied_wijk_identificatie_not, gebied_wijk_code=gebied_wijk_code, gebied_wijk_code_in=gebied_wijk_code_in, gebied_wijk_code_isempty=gebied_wijk_code_isempty, gebied_wijk_code_isnull=gebied_wijk_code_isnull, gebied_wijk_code_like=gebied_wijk_code_like, gebied_wijk_code_not=gebied_wijk_code_not, gebied_wijk_naam=gebied_wijk_naam, gebied_wijk_naam_in=gebied_wijk_naam_in, gebied_wijk_naam_isempty=gebied_wijk_naam_isempty, gebied_wijk_naam_isnull=gebied_wijk_naam_isnull, gebied_wijk_naam_like=gebied_wijk_naam_like, gebied_wijk_naam_not=gebied_wijk_naam_not, gebruiksdoel=gebruiksdoel, gebruiksdoel_in=gebruiksdoel_in, gebruiksdoel_isempty=gebruiksdoel_isempty, gebruiksdoel_isnull=gebruiksdoel_isnull, gebruiksdoel_like=gebruiksdoel_like, gebruiksdoel_not=gebruiksdoel_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, heeft_barcode_sinds=heeft_barcode_sinds, heeft_barcode_sinds_gt=heeft_barcode_sinds_gt, heeft_barcode_sinds_gte=heeft_barcode_sinds_gte, heeft_barcode_sinds_in=heeft_barcode_sinds_in, heeft_barcode_sinds_isnull=heeft_barcode_sinds_isnull, heeft_barcode_sinds_lt=heeft_barcode_sinds_lt, heeft_barcode_sinds_lte=heeft_barcode_sinds_lte, heeft_barcode_sinds_not=heeft_barcode_sinds_not, heeft_chip_sinds=heeft_chip_sinds, heeft_chip_sinds_gt=heeft_chip_sinds_gt, heeft_chip_sinds_gte=heeft_chip_sinds_gte, heeft_chip_sinds_in=heeft_chip_sinds_in, heeft_chip_sinds_isnull=heeft_chip_sinds_isnull, heeft_chip_sinds_lt=heeft_chip_sinds_lt, heeft_chip_sinds_lte=heeft_chip_sinds_lte, heeft_chip_sinds_not=heeft_chip_sinds_not, huisletter=huisletter, huisletter_in=huisletter_in, huisletter_isempty=huisletter_isempty, huisletter_isnull=huisletter_isnull, huisletter_like=huisletter_like, huisletter_not=huisletter_not, huisnummer=huisnummer, huisnummer_gt=huisnummer_gt, huisnummer_gte=huisnummer_gte, huisnummer_in=huisnummer_in, huisnummer_isnull=huisnummer_isnull, huisnummer_lt=huisnummer_lt, huisnummer_lte=huisnummer_lte, huisnummer_not=huisnummer_not, huisnummertoevoeging=huisnummertoevoeging, huisnummertoevoeging_in=huisnummertoevoeging_in, huisnummertoevoeging_isempty=huisnummertoevoeging_isempty, huisnummertoevoeging_isnull=huisnummertoevoeging_isnull, huisnummertoevoeging_like=huisnummertoevoeging_like, huisnummertoevoeging_not=huisnummertoevoeging_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, page=page, postcode=postcode, postcode_in=postcode_in, postcode_isempty=postcode_isempty, postcode_isnull=postcode_isnull, postcode_like=postcode_like, postcode_not=postcode_not, soort_container=soort_container, soort_container_in=soort_container_in, soort_container_isempty=soort_container_isempty, soort_container_isnull=soort_container_isnull, soort_container_like=soort_container_like, soort_container_not=soort_container_not, status=status, status_sinds=status_sinds, status_sinds_gt=status_sinds_gt, status_sinds_gte=status_sinds_gte, status_sinds_in=status_sinds_in, status_sinds_isnull=status_sinds_isnull, status_sinds_lt=status_sinds_lt, status_sinds_lte=status_sinds_lte, status_sinds_not=status_sinds_not, status_in=status_in, status_isempty=status_isempty, status_isnull=status_isnull, status_like=status_like, status_not=status_not, straatnaam=straatnaam, straatnaam_in=straatnaam_in, straatnaam_isempty=straatnaam_isempty, straatnaam_isnull=straatnaam_isnull, straatnaam_like=straatnaam_like, straatnaam_not=straatnaam_not, typeadresseerbaarobject=typeadresseerbaarobject, typeadresseerbaarobject_in=typeadresseerbaarobject_in, typeadresseerbaarobject_isempty=typeadresseerbaarobject_isempty, typeadresseerbaarobject_isnull=typeadresseerbaarobject_isnull, typeadresseerbaarobject_like=typeadresseerbaarobject_like, typeadresseerbaarobject_not=typeadresseerbaarobject_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not, woonplaats_naam=woonplaats_naam, woonplaats_naam_in=woonplaats_naam_in, woonplaats_naam_isempty=woonplaats_naam_isempty, woonplaats_naam_isnull=woonplaats_naam_isnull, woonplaats_naam_like=woonplaats_naam_like, woonplaats_naam_not=woonplaats_naam_not)

Deze tabel bevat informatie over de stanmgegevens van de rolcontainers in Gemeente Amsterdam

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalrolcontainer_list import PaginatedHuishoudelijkafvalrolcontainerList
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
    api_instance = huishoudelijkafval_api_client.RolcontainerApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'bagNummeraanduiding' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    aanmaakdatum = '2013-10-20T19:20:30+01:00' # datetime | Datum tijd waarop de rolcontainer in het systeem is aangemaakt (optional)
    aanmaakdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aanmaakdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aanmaakdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    bag_nummeraanduiding_identificatie = 'bag_nummeraanduiding_identificatie_example' # str | De unieke aanduiding van een nummeraanduiding (optional)
    bag_nummeraanduiding_identificatie_in = ['bag_nummeraanduiding_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_nummeraanduiding_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_nummeraanduiding_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_nummeraanduiding_identificatie_like = 'bag_nummeraanduiding_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_nummeraanduiding_identificatie_not = ['bag_nummeraanduiding_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_openbareruimte_identificatie = 'bag_openbareruimte_identificatie_example' # str | Unieke identificatie van een openbare ruimte (optional)
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
    bag_woonplaats_identificatie = 'bag_woonplaats_identificatie_example' # str | Unieke aanduiding van een woonplaats (optional)
    bag_woonplaats_identificatie_in = ['bag_woonplaats_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_woonplaats_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_woonplaats_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_woonplaats_identificatie_like = 'bag_woonplaats_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_woonplaats_identificatie_not = ['bag_woonplaats_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    barcode = 'barcode_example' # str | De barcode van de chip dat van buitenaf leesbaar is. (optional)
    barcode_in = ['barcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    barcode_isempty = True # bool | Whether the field is empty or not. (optional)
    barcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    barcode_like = 'barcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    barcode_not = ['barcode_not_example'] # List[str] | Exclude matches; text (optional)
    chip_nummer = 'chip_nummer_example' # str | Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. (optional)
    chip_nummer_in = ['chip_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    chip_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    chip_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    chip_nummer_like = 'chip_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    chip_nummer_not = ['chip_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    chip_type = 'chip_type_example' # str | Het type van de chip dat aan de rolcontainer is bevestigd. (optional)
    chip_type_in = ['chip_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    chip_type_isempty = True # bool | Whether the field is empty or not. (optional)
    chip_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    chip_type_like = 'chip_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    chip_type_not = ['chip_type_not_example'] # List[str] | Exclude matches; text (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Container fractieomschrijving zoals door leverancier is geleverd. (optional)
    fractie_omschrijving_in = ['fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_omschrijving_like = 'fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_omschrijving_not = ['fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_buurt_identificatie = 'gebied_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gebied_buurt_identificatie_in = ['gebied_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_buurt_identificatie_like = 'gebied_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_buurt_identificatie_not = ['gebied_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_buurt_code = 'gebied_buurt_code_example' # str | Unieke code (hier in zie je de Stadsdeel- en Wijkcode terug) (optional)
    gebied_buurt_code_in = ['gebied_buurt_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_buurt_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_buurt_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_buurt_code_like = 'gebied_buurt_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_buurt_code_not = ['gebied_buurt_code_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_buurt_naam = 'gebied_buurt_naam_example' # str | De naam van het object (optional)
    gebied_buurt_naam_in = ['gebied_buurt_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_buurt_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_buurt_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_buurt_naam_like = 'gebied_buurt_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_buurt_naam_not = ['gebied_buurt_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_ggw_identificatie = 'gebied_ggw_identificatie_example' # str | Unieke identificatie van het object (optional)
    gebied_ggw_identificatie_in = ['gebied_ggw_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_ggw_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_ggw_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_ggw_identificatie_like = 'gebied_ggw_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_ggw_identificatie_not = ['gebied_ggw_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_ggw_code = 'gebied_ggw_code_example' # str | De unieke code van het gebiedsgericht werken gebied (optional)
    gebied_ggw_code_in = ['gebied_ggw_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_ggw_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_ggw_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_ggw_code_like = 'gebied_ggw_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_ggw_code_not = ['gebied_ggw_code_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_ggw_naam = 'gebied_ggw_naam_example' # str | De naam van het gebiedsgericht werken gebied (optional)
    gebied_ggw_naam_in = ['gebied_ggw_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_ggw_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_ggw_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_ggw_naam_like = 'gebied_ggw_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_ggw_naam_not = ['gebied_ggw_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_stadsdeel_identificatie = 'gebied_stadsdeel_identificatie_example' # str | Unieke identificatie van het object (optional)
    gebied_stadsdeel_identificatie_in = ['gebied_stadsdeel_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_stadsdeel_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_stadsdeel_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_stadsdeel_identificatie_like = 'gebied_stadsdeel_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_stadsdeel_identificatie_not = ['gebied_stadsdeel_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_stadsdeel_code = 'gebied_stadsdeel_code_example' # str | Officile code van het stadsdeel (optional)
    gebied_stadsdeel_code_in = ['gebied_stadsdeel_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_stadsdeel_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_stadsdeel_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_stadsdeel_code_like = 'gebied_stadsdeel_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_stadsdeel_code_not = ['gebied_stadsdeel_code_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_stadsdeel_naam = 'gebied_stadsdeel_naam_example' # str | De naam van het stadsdeel. (optional)
    gebied_stadsdeel_naam_in = ['gebied_stadsdeel_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_stadsdeel_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_stadsdeel_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_stadsdeel_naam_like = 'gebied_stadsdeel_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_stadsdeel_naam_not = ['gebied_stadsdeel_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_wijk_identificatie = 'gebied_wijk_identificatie_example' # str | Unieke identificatie van het object (optional)
    gebied_wijk_identificatie_in = ['gebied_wijk_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_wijk_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_wijk_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_wijk_identificatie_like = 'gebied_wijk_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_wijk_identificatie_not = ['gebied_wijk_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_wijk_code = 'gebied_wijk_code_example' # str | Volledige, samengestelde, code, bestaande uit stadsdeelcode en wijkcode (optional)
    gebied_wijk_code_in = ['gebied_wijk_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_wijk_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_wijk_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_wijk_code_like = 'gebied_wijk_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_wijk_code_not = ['gebied_wijk_code_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_wijk_naam = 'gebied_wijk_naam_example' # str | De naam van de wijk (optional)
    gebied_wijk_naam_in = ['gebied_wijk_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_wijk_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_wijk_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_wijk_naam_like = 'gebied_wijk_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_wijk_naam_not = ['gebied_wijk_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebruiksdoel = 'gebruiksdoel_example' # str | Een categorisering van de gebruiksdoelen van het betreffende adreseerbareobject, zoals dit door de overheid als zodanig is toegestaan (optional)
    gebruiksdoel_in = ['gebruiksdoel_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebruiksdoel_isempty = True # bool | Whether the field is empty or not. (optional)
    gebruiksdoel_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebruiksdoel_like = 'gebruiksdoel_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebruiksdoel_not = ['gebruiksdoel_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de rolcontainer RD (epsg:28992). De geometrieën zijn afkomstig uit BAG.  (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    heeft_barcode_sinds = '2013-10-20' # date | Dit attribuut, heeft_barcode_sinds, geeft de datum aan waarop de chip is voorzien van een barcode.. (optional)
    heeft_barcode_sinds_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    heeft_barcode_sinds_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    heeft_barcode_sinds_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    heeft_barcode_sinds_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    heeft_barcode_sinds_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    heeft_barcode_sinds_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    heeft_barcode_sinds_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    heeft_chip_sinds = '2013-10-20' # date | Datum waarop de chip aan de rolcontainer is bevestigd.  (optional)
    heeft_chip_sinds_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    heeft_chip_sinds_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    heeft_chip_sinds_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    heeft_chip_sinds_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    heeft_chip_sinds_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    heeft_chip_sinds_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    heeft_chip_sinds_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    huisletter = 'huisletter_example' # str | Een alfabetisch teken achter het huisnummer zoals dit door het gemeentebestuur is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende toevoeging aan een huisnummer in de vorm van een alfabetisch teken. (optional)
    huisletter_in = ['huisletter_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    huisletter_isempty = True # bool | Whether the field is empty or not. (optional)
    huisletter_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    huisletter_like = 'huisletter_like_example' # str | Matches text using wildcards (? and *). (optional)
    huisletter_not = ['huisletter_not_example'] # List[str] | Exclude matches; text (optional)
    huisnummer = 56 # int | De numerieke aanduiding zoals deze door het gemeente bestuur aan het object is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende nummering. (optional)
    huisnummer_gt = 56 # int | Greater than; number (optional)
    huisnummer_gte = 56 # int | Greater than or equal to; number (optional)
    huisnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    huisnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    huisnummer_lt = 56 # int | Less than; number (optional)
    huisnummer_lte = 56 # int | Less than or equal to; number (optional)
    huisnummer_not = [56] # List[int] | Exclude matches; number (optional)
    huisnummertoevoeging = 'huisnummertoevoeging_example' # str | Die let­ters of te­kens die nood­za­ke­lijk zijn om, naast huis­num­mer en -let­ter, de brie­ven­bus te vin­den dan wel een door of na­mens het be­voeg­de ge­meen­te­lij­ke or­gaan ten aan­zien van een adres­seer­baar ob­ject toe­ge­ken­de toe­voe­ging aan een huis­num­mer of een com­bi­na­tie van huis­let­ter en huis­num­mer (optional)
    huisnummertoevoeging_in = ['huisnummertoevoeging_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    huisnummertoevoeging_isempty = True # bool | Whether the field is empty or not. (optional)
    huisnummertoevoeging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    huisnummertoevoeging_like = 'huisnummertoevoeging_like_example' # str | Matches text using wildcards (? and *). (optional)
    huisnummertoevoeging_not = ['huisnummertoevoeging_not_example'] # List[str] | Exclude matches; text (optional)
    id = 56 # int | Unieke aanduiding van een rolcontainer (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    postcode = 'postcode_example' # str | De door de Post NL vast­ge­stel­de code be­ho­rend bij de straat­naam en het huis­num­mer dan wel de door Post NL vast­ge­stel­de code be­ho­ren­de bij een be­paal­de com­bi­na­tie van een naam open­ba­re ruim­te en een huis­num­mer. (optional)
    postcode_in = ['postcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    postcode_isempty = True # bool | Whether the field is empty or not. (optional)
    postcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    postcode_like = 'postcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    postcode_not = ['postcode_not_example'] # List[str] | Exclude matches; text (optional)
    soort_container = 'soort_container_example' # str | Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. (optional)
    soort_container_in = ['soort_container_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_container_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_container_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_container_like = 'soort_container_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_container_not = ['soort_container_not_example'] # List[str] | Exclude matches; text (optional)
    status = 'status_example' # str | Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. (optional)
    status_sinds = '2013-10-20' # date | Datum waarop de laatste status van een rolcontainer van toepassing is (optional)
    status_sinds_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    status_sinds_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    status_sinds_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_sinds_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_sinds_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    status_sinds_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    status_sinds_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    status_in = ['status_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isempty = True # bool | Whether the field is empty or not. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_like = 'status_like_example' # str | Matches text using wildcards (? and *). (optional)
    status_not = ['status_not_example'] # List[str] | Exclude matches; text (optional)
    straatnaam = 'straatnaam_example' # str | Naam van de straat (optional)
    straatnaam_in = ['straatnaam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    straatnaam_isempty = True # bool | Whether the field is empty or not. (optional)
    straatnaam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    straatnaam_like = 'straatnaam_like_example' # str | Matches text using wildcards (? and *). (optional)
    straatnaam_not = ['straatnaam_not_example'] # List[str] | Exclude matches; text (optional)
    typeadresseerbaarobject = 'typeadresseerbaarobject_example' # str | Een Adresseerbaar object is een (abstract) object waaraan adressen kunnen worden toegekend (optional)
    typeadresseerbaarobject_in = ['typeadresseerbaarobject_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    typeadresseerbaarobject_isempty = True # bool | Whether the field is empty or not. (optional)
    typeadresseerbaarobject_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    typeadresseerbaarobject_like = 'typeadresseerbaarobject_like_example' # str | Matches text using wildcards (? and *). (optional)
    typeadresseerbaarobject_not = ['typeadresseerbaarobject_not_example'] # List[str] | Exclude matches; text (optional)
    wijzigingsdatum = '2013-10-20T19:20:30+01:00' # datetime | Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast (optional)
    wijzigingsdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    woonplaats_naam = 'woonplaats_naam_example' # str | Een Woonplaats is een door het bevoegde gemeentelijke orgaan als zodanig aangewezen en van een naam voorzien gedeelte van het grondgebied van de gemeente. (optional)
    woonplaats_naam_in = ['woonplaats_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    woonplaats_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    woonplaats_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    woonplaats_naam_like = 'woonplaats_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    woonplaats_naam_not = ['woonplaats_naam_not_example'] # List[str] | Exclude matches; text (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_rolcontainer_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bag_woonplaats_identificatie=bag_woonplaats_identificatie, bag_woonplaats_identificatie_in=bag_woonplaats_identificatie_in, bag_woonplaats_identificatie_isempty=bag_woonplaats_identificatie_isempty, bag_woonplaats_identificatie_isnull=bag_woonplaats_identificatie_isnull, bag_woonplaats_identificatie_like=bag_woonplaats_identificatie_like, bag_woonplaats_identificatie_not=bag_woonplaats_identificatie_not, barcode=barcode, barcode_in=barcode_in, barcode_isempty=barcode_isempty, barcode_isnull=barcode_isnull, barcode_like=barcode_like, barcode_not=barcode_not, chip_nummer=chip_nummer, chip_nummer_in=chip_nummer_in, chip_nummer_isempty=chip_nummer_isempty, chip_nummer_isnull=chip_nummer_isnull, chip_nummer_like=chip_nummer_like, chip_nummer_not=chip_nummer_not, chip_type=chip_type, chip_type_in=chip_type_in, chip_type_isempty=chip_type_isempty, chip_type_isnull=chip_type_isnull, chip_type_like=chip_type_like, chip_type_not=chip_type_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gebied_buurt_identificatie=gebied_buurt_identificatie, gebied_buurt_identificatie_in=gebied_buurt_identificatie_in, gebied_buurt_identificatie_isempty=gebied_buurt_identificatie_isempty, gebied_buurt_identificatie_isnull=gebied_buurt_identificatie_isnull, gebied_buurt_identificatie_like=gebied_buurt_identificatie_like, gebied_buurt_identificatie_not=gebied_buurt_identificatie_not, gebied_buurt_code=gebied_buurt_code, gebied_buurt_code_in=gebied_buurt_code_in, gebied_buurt_code_isempty=gebied_buurt_code_isempty, gebied_buurt_code_isnull=gebied_buurt_code_isnull, gebied_buurt_code_like=gebied_buurt_code_like, gebied_buurt_code_not=gebied_buurt_code_not, gebied_buurt_naam=gebied_buurt_naam, gebied_buurt_naam_in=gebied_buurt_naam_in, gebied_buurt_naam_isempty=gebied_buurt_naam_isempty, gebied_buurt_naam_isnull=gebied_buurt_naam_isnull, gebied_buurt_naam_like=gebied_buurt_naam_like, gebied_buurt_naam_not=gebied_buurt_naam_not, gebied_ggw_identificatie=gebied_ggw_identificatie, gebied_ggw_identificatie_in=gebied_ggw_identificatie_in, gebied_ggw_identificatie_isempty=gebied_ggw_identificatie_isempty, gebied_ggw_identificatie_isnull=gebied_ggw_identificatie_isnull, gebied_ggw_identificatie_like=gebied_ggw_identificatie_like, gebied_ggw_identificatie_not=gebied_ggw_identificatie_not, gebied_ggw_code=gebied_ggw_code, gebied_ggw_code_in=gebied_ggw_code_in, gebied_ggw_code_isempty=gebied_ggw_code_isempty, gebied_ggw_code_isnull=gebied_ggw_code_isnull, gebied_ggw_code_like=gebied_ggw_code_like, gebied_ggw_code_not=gebied_ggw_code_not, gebied_ggw_naam=gebied_ggw_naam, gebied_ggw_naam_in=gebied_ggw_naam_in, gebied_ggw_naam_isempty=gebied_ggw_naam_isempty, gebied_ggw_naam_isnull=gebied_ggw_naam_isnull, gebied_ggw_naam_like=gebied_ggw_naam_like, gebied_ggw_naam_not=gebied_ggw_naam_not, gebied_stadsdeel_identificatie=gebied_stadsdeel_identificatie, gebied_stadsdeel_identificatie_in=gebied_stadsdeel_identificatie_in, gebied_stadsdeel_identificatie_isempty=gebied_stadsdeel_identificatie_isempty, gebied_stadsdeel_identificatie_isnull=gebied_stadsdeel_identificatie_isnull, gebied_stadsdeel_identificatie_like=gebied_stadsdeel_identificatie_like, gebied_stadsdeel_identificatie_not=gebied_stadsdeel_identificatie_not, gebied_stadsdeel_code=gebied_stadsdeel_code, gebied_stadsdeel_code_in=gebied_stadsdeel_code_in, gebied_stadsdeel_code_isempty=gebied_stadsdeel_code_isempty, gebied_stadsdeel_code_isnull=gebied_stadsdeel_code_isnull, gebied_stadsdeel_code_like=gebied_stadsdeel_code_like, gebied_stadsdeel_code_not=gebied_stadsdeel_code_not, gebied_stadsdeel_naam=gebied_stadsdeel_naam, gebied_stadsdeel_naam_in=gebied_stadsdeel_naam_in, gebied_stadsdeel_naam_isempty=gebied_stadsdeel_naam_isempty, gebied_stadsdeel_naam_isnull=gebied_stadsdeel_naam_isnull, gebied_stadsdeel_naam_like=gebied_stadsdeel_naam_like, gebied_stadsdeel_naam_not=gebied_stadsdeel_naam_not, gebied_wijk_identificatie=gebied_wijk_identificatie, gebied_wijk_identificatie_in=gebied_wijk_identificatie_in, gebied_wijk_identificatie_isempty=gebied_wijk_identificatie_isempty, gebied_wijk_identificatie_isnull=gebied_wijk_identificatie_isnull, gebied_wijk_identificatie_like=gebied_wijk_identificatie_like, gebied_wijk_identificatie_not=gebied_wijk_identificatie_not, gebied_wijk_code=gebied_wijk_code, gebied_wijk_code_in=gebied_wijk_code_in, gebied_wijk_code_isempty=gebied_wijk_code_isempty, gebied_wijk_code_isnull=gebied_wijk_code_isnull, gebied_wijk_code_like=gebied_wijk_code_like, gebied_wijk_code_not=gebied_wijk_code_not, gebied_wijk_naam=gebied_wijk_naam, gebied_wijk_naam_in=gebied_wijk_naam_in, gebied_wijk_naam_isempty=gebied_wijk_naam_isempty, gebied_wijk_naam_isnull=gebied_wijk_naam_isnull, gebied_wijk_naam_like=gebied_wijk_naam_like, gebied_wijk_naam_not=gebied_wijk_naam_not, gebruiksdoel=gebruiksdoel, gebruiksdoel_in=gebruiksdoel_in, gebruiksdoel_isempty=gebruiksdoel_isempty, gebruiksdoel_isnull=gebruiksdoel_isnull, gebruiksdoel_like=gebruiksdoel_like, gebruiksdoel_not=gebruiksdoel_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, heeft_barcode_sinds=heeft_barcode_sinds, heeft_barcode_sinds_gt=heeft_barcode_sinds_gt, heeft_barcode_sinds_gte=heeft_barcode_sinds_gte, heeft_barcode_sinds_in=heeft_barcode_sinds_in, heeft_barcode_sinds_isnull=heeft_barcode_sinds_isnull, heeft_barcode_sinds_lt=heeft_barcode_sinds_lt, heeft_barcode_sinds_lte=heeft_barcode_sinds_lte, heeft_barcode_sinds_not=heeft_barcode_sinds_not, heeft_chip_sinds=heeft_chip_sinds, heeft_chip_sinds_gt=heeft_chip_sinds_gt, heeft_chip_sinds_gte=heeft_chip_sinds_gte, heeft_chip_sinds_in=heeft_chip_sinds_in, heeft_chip_sinds_isnull=heeft_chip_sinds_isnull, heeft_chip_sinds_lt=heeft_chip_sinds_lt, heeft_chip_sinds_lte=heeft_chip_sinds_lte, heeft_chip_sinds_not=heeft_chip_sinds_not, huisletter=huisletter, huisletter_in=huisletter_in, huisletter_isempty=huisletter_isempty, huisletter_isnull=huisletter_isnull, huisletter_like=huisletter_like, huisletter_not=huisletter_not, huisnummer=huisnummer, huisnummer_gt=huisnummer_gt, huisnummer_gte=huisnummer_gte, huisnummer_in=huisnummer_in, huisnummer_isnull=huisnummer_isnull, huisnummer_lt=huisnummer_lt, huisnummer_lte=huisnummer_lte, huisnummer_not=huisnummer_not, huisnummertoevoeging=huisnummertoevoeging, huisnummertoevoeging_in=huisnummertoevoeging_in, huisnummertoevoeging_isempty=huisnummertoevoeging_isempty, huisnummertoevoeging_isnull=huisnummertoevoeging_isnull, huisnummertoevoeging_like=huisnummertoevoeging_like, huisnummertoevoeging_not=huisnummertoevoeging_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, page=page, postcode=postcode, postcode_in=postcode_in, postcode_isempty=postcode_isempty, postcode_isnull=postcode_isnull, postcode_like=postcode_like, postcode_not=postcode_not, soort_container=soort_container, soort_container_in=soort_container_in, soort_container_isempty=soort_container_isempty, soort_container_isnull=soort_container_isnull, soort_container_like=soort_container_like, soort_container_not=soort_container_not, status=status, status_sinds=status_sinds, status_sinds_gt=status_sinds_gt, status_sinds_gte=status_sinds_gte, status_sinds_in=status_sinds_in, status_sinds_isnull=status_sinds_isnull, status_sinds_lt=status_sinds_lt, status_sinds_lte=status_sinds_lte, status_sinds_not=status_sinds_not, status_in=status_in, status_isempty=status_isempty, status_isnull=status_isnull, status_like=status_like, status_not=status_not, straatnaam=straatnaam, straatnaam_in=straatnaam_in, straatnaam_isempty=straatnaam_isempty, straatnaam_isnull=straatnaam_isnull, straatnaam_like=straatnaam_like, straatnaam_not=straatnaam_not, typeadresseerbaarobject=typeadresseerbaarobject, typeadresseerbaarobject_in=typeadresseerbaarobject_in, typeadresseerbaarobject_isempty=typeadresseerbaarobject_isempty, typeadresseerbaarobject_isnull=typeadresseerbaarobject_isnull, typeadresseerbaarobject_like=typeadresseerbaarobject_like, typeadresseerbaarobject_not=typeadresseerbaarobject_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not, woonplaats_naam=woonplaats_naam, woonplaats_naam_in=woonplaats_naam_in, woonplaats_naam_isempty=woonplaats_naam_isempty, woonplaats_naam_isnull=woonplaats_naam_isnull, woonplaats_naam_like=woonplaats_naam_like, woonplaats_naam_not=woonplaats_naam_not)
        print("The response of RolcontainerApi->huishoudelijkafval_rolcontainer_list_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolcontainerApi->huishoudelijkafval_rolcontainer_list_slash: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accept_crs** | **str**| Accept-Crs header for Geo queries | [optional] 
 **content_crs** | **str**| Content-Crs header for Geo queries | [optional] 
 **x_api_key** | **str**| Api Key for statistical purposes, not for authentication | [optional] 
 **count** | **bool**| Include a count of the total result set and the number of pages.Only works for responses that return a page. | [optional] 
 **csv_header** | **str**| Specify type of header for csv file | [optional] 
 **csv_separator** | **str**| Specify type of separator for csv file | [optional] 
 **expand** | **bool**| Allow to expand relations. | [optional] 
 **expand_scope** | **str**| Comma separated list of named relations to expand. | [optional] 
 **fields** | **str**| Comma-separated list of fields to display | [optional] 
 **format** | **str**| Select the export format | [optional] 
 **page_size** | **int**| Number of results to return per page. | [optional] 
 **sort** | **str**| Which field to use when ordering the results. | [optional] 
 **aanmaakdatum** | **datetime**| Datum tijd waarop de rolcontainer in het systeem is aangemaakt | [optional] 
 **aanmaakdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aanmaakdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aanmaakdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **bag_nummeraanduiding_identificatie** | **str**| De unieke aanduiding van een nummeraanduiding | [optional] 
 **bag_nummeraanduiding_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_nummeraanduiding_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_nummeraanduiding_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_nummeraanduiding_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_nummeraanduiding_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_openbareruimte_identificatie** | **str**| Unieke identificatie van een openbare ruimte | [optional] 
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
 **bag_woonplaats_identificatie** | **str**| Unieke aanduiding van een woonplaats | [optional] 
 **bag_woonplaats_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_woonplaats_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_woonplaats_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_woonplaats_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_woonplaats_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **barcode** | **str**| De barcode van de chip dat van buitenaf leesbaar is. | [optional] 
 **barcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **barcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **barcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **barcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **barcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **chip_nummer** | **str**| Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. | [optional] 
 **chip_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **chip_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **chip_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **chip_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **chip_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **chip_type** | **str**| Het type van de chip dat aan de rolcontainer is bevestigd. | [optional] 
 **chip_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **chip_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **chip_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **chip_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **chip_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **fractie_omschrijving** | **str**| Container fractieomschrijving zoals door leverancier is geleverd. | [optional] 
 **fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gebied_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_buurt_code** | **str**| Unieke code (hier in zie je de Stadsdeel- en Wijkcode terug) | [optional] 
 **gebied_buurt_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_buurt_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_buurt_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_buurt_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_buurt_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_buurt_naam** | **str**| De naam van het object | [optional] 
 **gebied_buurt_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_buurt_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_buurt_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_buurt_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_buurt_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_ggw_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gebied_ggw_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_ggw_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_ggw_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_ggw_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_ggw_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_ggw_code** | **str**| De unieke code van het gebiedsgericht werken gebied | [optional] 
 **gebied_ggw_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_ggw_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_ggw_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_ggw_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_ggw_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_ggw_naam** | **str**| De naam van het gebiedsgericht werken gebied | [optional] 
 **gebied_ggw_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_ggw_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_ggw_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_ggw_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_ggw_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_stadsdeel_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gebied_stadsdeel_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_stadsdeel_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_stadsdeel_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_stadsdeel_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_stadsdeel_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_stadsdeel_code** | **str**| Officile code van het stadsdeel | [optional] 
 **gebied_stadsdeel_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_stadsdeel_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_stadsdeel_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_stadsdeel_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_stadsdeel_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_stadsdeel_naam** | **str**| De naam van het stadsdeel. | [optional] 
 **gebied_stadsdeel_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_stadsdeel_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_stadsdeel_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_stadsdeel_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_stadsdeel_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_wijk_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gebied_wijk_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_wijk_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_wijk_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_wijk_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_wijk_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_wijk_code** | **str**| Volledige, samengestelde, code, bestaande uit stadsdeelcode en wijkcode | [optional] 
 **gebied_wijk_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_wijk_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_wijk_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_wijk_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_wijk_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_wijk_naam** | **str**| De naam van de wijk | [optional] 
 **gebied_wijk_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_wijk_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_wijk_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_wijk_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_wijk_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebruiksdoel** | **str**| Een categorisering van de gebruiksdoelen van het betreffende adreseerbareobject, zoals dit door de overheid als zodanig is toegestaan | [optional] 
 **gebruiksdoel_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebruiksdoel_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebruiksdoel_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebruiksdoel_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebruiksdoel_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de rolcontainer RD (epsg:28992). De geometrieën zijn afkomstig uit BAG.  | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **heeft_barcode_sinds** | **date**| Dit attribuut, heeft_barcode_sinds, geeft de datum aan waarop de chip is voorzien van een barcode.. | [optional] 
 **heeft_barcode_sinds_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **heeft_barcode_sinds_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **heeft_barcode_sinds_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **heeft_barcode_sinds_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **heeft_barcode_sinds_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **heeft_barcode_sinds_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **heeft_barcode_sinds_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds** | **date**| Datum waarop de chip aan de rolcontainer is bevestigd.  | [optional] 
 **heeft_chip_sinds_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **heeft_chip_sinds_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **heeft_chip_sinds_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **huisletter** | **str**| Een alfabetisch teken achter het huisnummer zoals dit door het gemeentebestuur is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende toevoeging aan een huisnummer in de vorm van een alfabetisch teken. | [optional] 
 **huisletter_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **huisletter_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **huisletter_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **huisletter_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **huisletter_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **huisnummer** | **int**| De numerieke aanduiding zoals deze door het gemeente bestuur aan het object is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende nummering. | [optional] 
 **huisnummer_gt** | **int**| Greater than; number | [optional] 
 **huisnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **huisnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **huisnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **huisnummer_lt** | **int**| Less than; number | [optional] 
 **huisnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **huisnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **huisnummertoevoeging** | **str**| Die let­ters of te­kens die nood­za­ke­lijk zijn om, naast huis­num­mer en -let­ter, de brie­ven­bus te vin­den dan wel een door of na­mens het be­voeg­de ge­meen­te­lij­ke or­gaan ten aan­zien van een adres­seer­baar ob­ject toe­ge­ken­de toe­voe­ging aan een huis­num­mer of een com­bi­na­tie van huis­let­ter en huis­num­mer | [optional] 
 **huisnummertoevoeging_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **huisnummertoevoeging_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **huisnummertoevoeging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **huisnummertoevoeging_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **huisnummertoevoeging_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id** | **int**| Unieke aanduiding van een rolcontainer | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **postcode** | **str**| De door de Post NL vast­ge­stel­de code be­ho­rend bij de straat­naam en het huis­num­mer dan wel de door Post NL vast­ge­stel­de code be­ho­ren­de bij een be­paal­de com­bi­na­tie van een naam open­ba­re ruim­te en een huis­num­mer. | [optional] 
 **postcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **postcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **postcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **postcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **postcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **soort_container** | **str**| Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. | [optional] 
 **soort_container_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_container_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_container_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_container_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_container_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **str**| Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. | [optional] 
 **status_sinds** | **date**| Datum waarop de laatste status van een rolcontainer van toepassing is | [optional] 
 **status_sinds_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **status_sinds_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **status_sinds_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_sinds_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_sinds_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **status_sinds_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **status_sinds_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **status_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **status_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **straatnaam** | **str**| Naam van de straat | [optional] 
 **straatnaam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **straatnaam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **straatnaam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **straatnaam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **straatnaam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **typeadresseerbaarobject** | **str**| Een Adresseerbaar object is een (abstract) object waaraan adressen kunnen worden toegekend | [optional] 
 **typeadresseerbaarobject_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **typeadresseerbaarobject_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **typeadresseerbaarobject_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **typeadresseerbaarobject_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **typeadresseerbaarobject_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **wijzigingsdatum** | **datetime**| Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast | [optional] 
 **wijzigingsdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **woonplaats_naam** | **str**| Een Woonplaats is een door het bevoegde gemeentelijke orgaan als zodanig aangewezen en van een naam voorzien gedeelte van het grondgebied van de gemeente. | [optional] 
 **woonplaats_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **woonplaats_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **woonplaats_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **woonplaats_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **woonplaats_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalrolcontainerList**](PaginatedHuishoudelijkafvalrolcontainerList.md)

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

# **huishoudelijkafval_rolcontainer_retrieve_slash**
> Huishoudelijkafvalrolcontainer huishoudelijkafval_rolcontainer_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bag_woonplaats_identificatie=bag_woonplaats_identificatie, bag_woonplaats_identificatie_in=bag_woonplaats_identificatie_in, bag_woonplaats_identificatie_isempty=bag_woonplaats_identificatie_isempty, bag_woonplaats_identificatie_isnull=bag_woonplaats_identificatie_isnull, bag_woonplaats_identificatie_like=bag_woonplaats_identificatie_like, bag_woonplaats_identificatie_not=bag_woonplaats_identificatie_not, barcode=barcode, barcode_in=barcode_in, barcode_isempty=barcode_isempty, barcode_isnull=barcode_isnull, barcode_like=barcode_like, barcode_not=barcode_not, chip_nummer=chip_nummer, chip_nummer_in=chip_nummer_in, chip_nummer_isempty=chip_nummer_isempty, chip_nummer_isnull=chip_nummer_isnull, chip_nummer_like=chip_nummer_like, chip_nummer_not=chip_nummer_not, chip_type=chip_type, chip_type_in=chip_type_in, chip_type_isempty=chip_type_isempty, chip_type_isnull=chip_type_isnull, chip_type_like=chip_type_like, chip_type_not=chip_type_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gebied_buurt_identificatie=gebied_buurt_identificatie, gebied_buurt_identificatie_in=gebied_buurt_identificatie_in, gebied_buurt_identificatie_isempty=gebied_buurt_identificatie_isempty, gebied_buurt_identificatie_isnull=gebied_buurt_identificatie_isnull, gebied_buurt_identificatie_like=gebied_buurt_identificatie_like, gebied_buurt_identificatie_not=gebied_buurt_identificatie_not, gebied_buurt_code=gebied_buurt_code, gebied_buurt_code_in=gebied_buurt_code_in, gebied_buurt_code_isempty=gebied_buurt_code_isempty, gebied_buurt_code_isnull=gebied_buurt_code_isnull, gebied_buurt_code_like=gebied_buurt_code_like, gebied_buurt_code_not=gebied_buurt_code_not, gebied_buurt_naam=gebied_buurt_naam, gebied_buurt_naam_in=gebied_buurt_naam_in, gebied_buurt_naam_isempty=gebied_buurt_naam_isempty, gebied_buurt_naam_isnull=gebied_buurt_naam_isnull, gebied_buurt_naam_like=gebied_buurt_naam_like, gebied_buurt_naam_not=gebied_buurt_naam_not, gebied_ggw_identificatie=gebied_ggw_identificatie, gebied_ggw_identificatie_in=gebied_ggw_identificatie_in, gebied_ggw_identificatie_isempty=gebied_ggw_identificatie_isempty, gebied_ggw_identificatie_isnull=gebied_ggw_identificatie_isnull, gebied_ggw_identificatie_like=gebied_ggw_identificatie_like, gebied_ggw_identificatie_not=gebied_ggw_identificatie_not, gebied_ggw_code=gebied_ggw_code, gebied_ggw_code_in=gebied_ggw_code_in, gebied_ggw_code_isempty=gebied_ggw_code_isempty, gebied_ggw_code_isnull=gebied_ggw_code_isnull, gebied_ggw_code_like=gebied_ggw_code_like, gebied_ggw_code_not=gebied_ggw_code_not, gebied_ggw_naam=gebied_ggw_naam, gebied_ggw_naam_in=gebied_ggw_naam_in, gebied_ggw_naam_isempty=gebied_ggw_naam_isempty, gebied_ggw_naam_isnull=gebied_ggw_naam_isnull, gebied_ggw_naam_like=gebied_ggw_naam_like, gebied_ggw_naam_not=gebied_ggw_naam_not, gebied_stadsdeel_identificatie=gebied_stadsdeel_identificatie, gebied_stadsdeel_identificatie_in=gebied_stadsdeel_identificatie_in, gebied_stadsdeel_identificatie_isempty=gebied_stadsdeel_identificatie_isempty, gebied_stadsdeel_identificatie_isnull=gebied_stadsdeel_identificatie_isnull, gebied_stadsdeel_identificatie_like=gebied_stadsdeel_identificatie_like, gebied_stadsdeel_identificatie_not=gebied_stadsdeel_identificatie_not, gebied_stadsdeel_code=gebied_stadsdeel_code, gebied_stadsdeel_code_in=gebied_stadsdeel_code_in, gebied_stadsdeel_code_isempty=gebied_stadsdeel_code_isempty, gebied_stadsdeel_code_isnull=gebied_stadsdeel_code_isnull, gebied_stadsdeel_code_like=gebied_stadsdeel_code_like, gebied_stadsdeel_code_not=gebied_stadsdeel_code_not, gebied_stadsdeel_naam=gebied_stadsdeel_naam, gebied_stadsdeel_naam_in=gebied_stadsdeel_naam_in, gebied_stadsdeel_naam_isempty=gebied_stadsdeel_naam_isempty, gebied_stadsdeel_naam_isnull=gebied_stadsdeel_naam_isnull, gebied_stadsdeel_naam_like=gebied_stadsdeel_naam_like, gebied_stadsdeel_naam_not=gebied_stadsdeel_naam_not, gebied_wijk_identificatie=gebied_wijk_identificatie, gebied_wijk_identificatie_in=gebied_wijk_identificatie_in, gebied_wijk_identificatie_isempty=gebied_wijk_identificatie_isempty, gebied_wijk_identificatie_isnull=gebied_wijk_identificatie_isnull, gebied_wijk_identificatie_like=gebied_wijk_identificatie_like, gebied_wijk_identificatie_not=gebied_wijk_identificatie_not, gebied_wijk_code=gebied_wijk_code, gebied_wijk_code_in=gebied_wijk_code_in, gebied_wijk_code_isempty=gebied_wijk_code_isempty, gebied_wijk_code_isnull=gebied_wijk_code_isnull, gebied_wijk_code_like=gebied_wijk_code_like, gebied_wijk_code_not=gebied_wijk_code_not, gebied_wijk_naam=gebied_wijk_naam, gebied_wijk_naam_in=gebied_wijk_naam_in, gebied_wijk_naam_isempty=gebied_wijk_naam_isempty, gebied_wijk_naam_isnull=gebied_wijk_naam_isnull, gebied_wijk_naam_like=gebied_wijk_naam_like, gebied_wijk_naam_not=gebied_wijk_naam_not, gebruiksdoel=gebruiksdoel, gebruiksdoel_in=gebruiksdoel_in, gebruiksdoel_isempty=gebruiksdoel_isempty, gebruiksdoel_isnull=gebruiksdoel_isnull, gebruiksdoel_like=gebruiksdoel_like, gebruiksdoel_not=gebruiksdoel_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, heeft_barcode_sinds=heeft_barcode_sinds, heeft_barcode_sinds_gt=heeft_barcode_sinds_gt, heeft_barcode_sinds_gte=heeft_barcode_sinds_gte, heeft_barcode_sinds_in=heeft_barcode_sinds_in, heeft_barcode_sinds_isnull=heeft_barcode_sinds_isnull, heeft_barcode_sinds_lt=heeft_barcode_sinds_lt, heeft_barcode_sinds_lte=heeft_barcode_sinds_lte, heeft_barcode_sinds_not=heeft_barcode_sinds_not, heeft_chip_sinds=heeft_chip_sinds, heeft_chip_sinds_gt=heeft_chip_sinds_gt, heeft_chip_sinds_gte=heeft_chip_sinds_gte, heeft_chip_sinds_in=heeft_chip_sinds_in, heeft_chip_sinds_isnull=heeft_chip_sinds_isnull, heeft_chip_sinds_lt=heeft_chip_sinds_lt, heeft_chip_sinds_lte=heeft_chip_sinds_lte, heeft_chip_sinds_not=heeft_chip_sinds_not, huisletter=huisletter, huisletter_in=huisletter_in, huisletter_isempty=huisletter_isempty, huisletter_isnull=huisletter_isnull, huisletter_like=huisletter_like, huisletter_not=huisletter_not, huisnummer=huisnummer, huisnummer_gt=huisnummer_gt, huisnummer_gte=huisnummer_gte, huisnummer_in=huisnummer_in, huisnummer_isnull=huisnummer_isnull, huisnummer_lt=huisnummer_lt, huisnummer_lte=huisnummer_lte, huisnummer_not=huisnummer_not, huisnummertoevoeging=huisnummertoevoeging, huisnummertoevoeging_in=huisnummertoevoeging_in, huisnummertoevoeging_isempty=huisnummertoevoeging_isempty, huisnummertoevoeging_isnull=huisnummertoevoeging_isnull, huisnummertoevoeging_like=huisnummertoevoeging_like, huisnummertoevoeging_not=huisnummertoevoeging_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, postcode=postcode, postcode_in=postcode_in, postcode_isempty=postcode_isempty, postcode_isnull=postcode_isnull, postcode_like=postcode_like, postcode_not=postcode_not, soort_container=soort_container, soort_container_in=soort_container_in, soort_container_isempty=soort_container_isempty, soort_container_isnull=soort_container_isnull, soort_container_like=soort_container_like, soort_container_not=soort_container_not, status=status, status_sinds=status_sinds, status_sinds_gt=status_sinds_gt, status_sinds_gte=status_sinds_gte, status_sinds_in=status_sinds_in, status_sinds_isnull=status_sinds_isnull, status_sinds_lt=status_sinds_lt, status_sinds_lte=status_sinds_lte, status_sinds_not=status_sinds_not, status_in=status_in, status_isempty=status_isempty, status_isnull=status_isnull, status_like=status_like, status_not=status_not, straatnaam=straatnaam, straatnaam_in=straatnaam_in, straatnaam_isempty=straatnaam_isempty, straatnaam_isnull=straatnaam_isnull, straatnaam_like=straatnaam_like, straatnaam_not=straatnaam_not, typeadresseerbaarobject=typeadresseerbaarobject, typeadresseerbaarobject_in=typeadresseerbaarobject_in, typeadresseerbaarobject_isempty=typeadresseerbaarobject_isempty, typeadresseerbaarobject_isnull=typeadresseerbaarobject_isnull, typeadresseerbaarobject_like=typeadresseerbaarobject_like, typeadresseerbaarobject_not=typeadresseerbaarobject_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not, woonplaats_naam=woonplaats_naam, woonplaats_naam_in=woonplaats_naam_in, woonplaats_naam_isempty=woonplaats_naam_isempty, woonplaats_naam_isnull=woonplaats_naam_isnull, woonplaats_naam_like=woonplaats_naam_like, woonplaats_naam_not=woonplaats_naam_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalrolcontainer import Huishoudelijkafvalrolcontainer
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
    api_instance = huishoudelijkafval_api_client.RolcontainerApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'bagNummeraanduiding' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    aanmaakdatum = '2013-10-20T19:20:30+01:00' # datetime | Datum tijd waarop de rolcontainer in het systeem is aangemaakt (optional)
    aanmaakdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aanmaakdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aanmaakdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    bag_nummeraanduiding_identificatie = 'bag_nummeraanduiding_identificatie_example' # str | De unieke aanduiding van een nummeraanduiding (optional)
    bag_nummeraanduiding_identificatie_in = ['bag_nummeraanduiding_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_nummeraanduiding_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_nummeraanduiding_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_nummeraanduiding_identificatie_like = 'bag_nummeraanduiding_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_nummeraanduiding_identificatie_not = ['bag_nummeraanduiding_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_openbareruimte_identificatie = 'bag_openbareruimte_identificatie_example' # str | Unieke identificatie van een openbare ruimte (optional)
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
    bag_woonplaats_identificatie = 'bag_woonplaats_identificatie_example' # str | Unieke aanduiding van een woonplaats (optional)
    bag_woonplaats_identificatie_in = ['bag_woonplaats_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_woonplaats_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_woonplaats_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_woonplaats_identificatie_like = 'bag_woonplaats_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_woonplaats_identificatie_not = ['bag_woonplaats_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    barcode = 'barcode_example' # str | De barcode van de chip dat van buitenaf leesbaar is. (optional)
    barcode_in = ['barcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    barcode_isempty = True # bool | Whether the field is empty or not. (optional)
    barcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    barcode_like = 'barcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    barcode_not = ['barcode_not_example'] # List[str] | Exclude matches; text (optional)
    chip_nummer = 'chip_nummer_example' # str | Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. (optional)
    chip_nummer_in = ['chip_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    chip_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    chip_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    chip_nummer_like = 'chip_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    chip_nummer_not = ['chip_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    chip_type = 'chip_type_example' # str | Het type van de chip dat aan de rolcontainer is bevestigd. (optional)
    chip_type_in = ['chip_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    chip_type_isempty = True # bool | Whether the field is empty or not. (optional)
    chip_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    chip_type_like = 'chip_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    chip_type_not = ['chip_type_not_example'] # List[str] | Exclude matches; text (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Container fractieomschrijving zoals door leverancier is geleverd. (optional)
    fractie_omschrijving_in = ['fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_omschrijving_like = 'fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_omschrijving_not = ['fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_buurt_identificatie = 'gebied_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gebied_buurt_identificatie_in = ['gebied_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_buurt_identificatie_like = 'gebied_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_buurt_identificatie_not = ['gebied_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_buurt_code = 'gebied_buurt_code_example' # str | Unieke code (hier in zie je de Stadsdeel- en Wijkcode terug) (optional)
    gebied_buurt_code_in = ['gebied_buurt_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_buurt_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_buurt_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_buurt_code_like = 'gebied_buurt_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_buurt_code_not = ['gebied_buurt_code_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_buurt_naam = 'gebied_buurt_naam_example' # str | De naam van het object (optional)
    gebied_buurt_naam_in = ['gebied_buurt_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_buurt_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_buurt_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_buurt_naam_like = 'gebied_buurt_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_buurt_naam_not = ['gebied_buurt_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_ggw_identificatie = 'gebied_ggw_identificatie_example' # str | Unieke identificatie van het object (optional)
    gebied_ggw_identificatie_in = ['gebied_ggw_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_ggw_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_ggw_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_ggw_identificatie_like = 'gebied_ggw_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_ggw_identificatie_not = ['gebied_ggw_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_ggw_code = 'gebied_ggw_code_example' # str | De unieke code van het gebiedsgericht werken gebied (optional)
    gebied_ggw_code_in = ['gebied_ggw_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_ggw_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_ggw_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_ggw_code_like = 'gebied_ggw_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_ggw_code_not = ['gebied_ggw_code_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_ggw_naam = 'gebied_ggw_naam_example' # str | De naam van het gebiedsgericht werken gebied (optional)
    gebied_ggw_naam_in = ['gebied_ggw_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_ggw_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_ggw_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_ggw_naam_like = 'gebied_ggw_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_ggw_naam_not = ['gebied_ggw_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_stadsdeel_identificatie = 'gebied_stadsdeel_identificatie_example' # str | Unieke identificatie van het object (optional)
    gebied_stadsdeel_identificatie_in = ['gebied_stadsdeel_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_stadsdeel_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_stadsdeel_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_stadsdeel_identificatie_like = 'gebied_stadsdeel_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_stadsdeel_identificatie_not = ['gebied_stadsdeel_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_stadsdeel_code = 'gebied_stadsdeel_code_example' # str | Officile code van het stadsdeel (optional)
    gebied_stadsdeel_code_in = ['gebied_stadsdeel_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_stadsdeel_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_stadsdeel_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_stadsdeel_code_like = 'gebied_stadsdeel_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_stadsdeel_code_not = ['gebied_stadsdeel_code_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_stadsdeel_naam = 'gebied_stadsdeel_naam_example' # str | De naam van het stadsdeel. (optional)
    gebied_stadsdeel_naam_in = ['gebied_stadsdeel_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_stadsdeel_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_stadsdeel_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_stadsdeel_naam_like = 'gebied_stadsdeel_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_stadsdeel_naam_not = ['gebied_stadsdeel_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_wijk_identificatie = 'gebied_wijk_identificatie_example' # str | Unieke identificatie van het object (optional)
    gebied_wijk_identificatie_in = ['gebied_wijk_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_wijk_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_wijk_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_wijk_identificatie_like = 'gebied_wijk_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_wijk_identificatie_not = ['gebied_wijk_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_wijk_code = 'gebied_wijk_code_example' # str | Volledige, samengestelde, code, bestaande uit stadsdeelcode en wijkcode (optional)
    gebied_wijk_code_in = ['gebied_wijk_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_wijk_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_wijk_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_wijk_code_like = 'gebied_wijk_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_wijk_code_not = ['gebied_wijk_code_not_example'] # List[str] | Exclude matches; text (optional)
    gebied_wijk_naam = 'gebied_wijk_naam_example' # str | De naam van de wijk (optional)
    gebied_wijk_naam_in = ['gebied_wijk_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebied_wijk_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gebied_wijk_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebied_wijk_naam_like = 'gebied_wijk_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebied_wijk_naam_not = ['gebied_wijk_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gebruiksdoel = 'gebruiksdoel_example' # str | Een categorisering van de gebruiksdoelen van het betreffende adreseerbareobject, zoals dit door de overheid als zodanig is toegestaan (optional)
    gebruiksdoel_in = ['gebruiksdoel_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gebruiksdoel_isempty = True # bool | Whether the field is empty or not. (optional)
    gebruiksdoel_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gebruiksdoel_like = 'gebruiksdoel_like_example' # str | Matches text using wildcards (? and *). (optional)
    gebruiksdoel_not = ['gebruiksdoel_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de rolcontainer RD (epsg:28992). De geometrieën zijn afkomstig uit BAG.  (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    heeft_barcode_sinds = '2013-10-20' # date | Dit attribuut, heeft_barcode_sinds, geeft de datum aan waarop de chip is voorzien van een barcode.. (optional)
    heeft_barcode_sinds_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    heeft_barcode_sinds_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    heeft_barcode_sinds_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    heeft_barcode_sinds_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    heeft_barcode_sinds_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    heeft_barcode_sinds_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    heeft_barcode_sinds_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    heeft_chip_sinds = '2013-10-20' # date | Datum waarop de chip aan de rolcontainer is bevestigd.  (optional)
    heeft_chip_sinds_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    heeft_chip_sinds_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    heeft_chip_sinds_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    heeft_chip_sinds_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    heeft_chip_sinds_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    heeft_chip_sinds_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    heeft_chip_sinds_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    huisletter = 'huisletter_example' # str | Een alfabetisch teken achter het huisnummer zoals dit door het gemeentebestuur is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende toevoeging aan een huisnummer in de vorm van een alfabetisch teken. (optional)
    huisletter_in = ['huisletter_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    huisletter_isempty = True # bool | Whether the field is empty or not. (optional)
    huisletter_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    huisletter_like = 'huisletter_like_example' # str | Matches text using wildcards (? and *). (optional)
    huisletter_not = ['huisletter_not_example'] # List[str] | Exclude matches; text (optional)
    huisnummer = 56 # int | De numerieke aanduiding zoals deze door het gemeente bestuur aan het object is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende nummering. (optional)
    huisnummer_gt = 56 # int | Greater than; number (optional)
    huisnummer_gte = 56 # int | Greater than or equal to; number (optional)
    huisnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    huisnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    huisnummer_lt = 56 # int | Less than; number (optional)
    huisnummer_lte = 56 # int | Less than or equal to; number (optional)
    huisnummer_not = [56] # List[int] | Exclude matches; number (optional)
    huisnummertoevoeging = 'huisnummertoevoeging_example' # str | Die let­ters of te­kens die nood­za­ke­lijk zijn om, naast huis­num­mer en -let­ter, de brie­ven­bus te vin­den dan wel een door of na­mens het be­voeg­de ge­meen­te­lij­ke or­gaan ten aan­zien van een adres­seer­baar ob­ject toe­ge­ken­de toe­voe­ging aan een huis­num­mer of een com­bi­na­tie van huis­let­ter en huis­num­mer (optional)
    huisnummertoevoeging_in = ['huisnummertoevoeging_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    huisnummertoevoeging_isempty = True # bool | Whether the field is empty or not. (optional)
    huisnummertoevoeging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    huisnummertoevoeging_like = 'huisnummertoevoeging_like_example' # str | Matches text using wildcards (? and *). (optional)
    huisnummertoevoeging_not = ['huisnummertoevoeging_not_example'] # List[str] | Exclude matches; text (optional)
    id2 = 56 # int | Unieke aanduiding van een rolcontainer (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    postcode = 'postcode_example' # str | De door de Post NL vast­ge­stel­de code be­ho­rend bij de straat­naam en het huis­num­mer dan wel de door Post NL vast­ge­stel­de code be­ho­ren­de bij een be­paal­de com­bi­na­tie van een naam open­ba­re ruim­te en een huis­num­mer. (optional)
    postcode_in = ['postcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    postcode_isempty = True # bool | Whether the field is empty or not. (optional)
    postcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    postcode_like = 'postcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    postcode_not = ['postcode_not_example'] # List[str] | Exclude matches; text (optional)
    soort_container = 'soort_container_example' # str | Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. (optional)
    soort_container_in = ['soort_container_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_container_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_container_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_container_like = 'soort_container_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_container_not = ['soort_container_not_example'] # List[str] | Exclude matches; text (optional)
    status = 'status_example' # str | Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. (optional)
    status_sinds = '2013-10-20' # date | Datum waarop de laatste status van een rolcontainer van toepassing is (optional)
    status_sinds_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    status_sinds_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    status_sinds_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_sinds_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_sinds_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    status_sinds_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    status_sinds_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    status_in = ['status_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isempty = True # bool | Whether the field is empty or not. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_like = 'status_like_example' # str | Matches text using wildcards (? and *). (optional)
    status_not = ['status_not_example'] # List[str] | Exclude matches; text (optional)
    straatnaam = 'straatnaam_example' # str | Naam van de straat (optional)
    straatnaam_in = ['straatnaam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    straatnaam_isempty = True # bool | Whether the field is empty or not. (optional)
    straatnaam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    straatnaam_like = 'straatnaam_like_example' # str | Matches text using wildcards (? and *). (optional)
    straatnaam_not = ['straatnaam_not_example'] # List[str] | Exclude matches; text (optional)
    typeadresseerbaarobject = 'typeadresseerbaarobject_example' # str | Een Adresseerbaar object is een (abstract) object waaraan adressen kunnen worden toegekend (optional)
    typeadresseerbaarobject_in = ['typeadresseerbaarobject_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    typeadresseerbaarobject_isempty = True # bool | Whether the field is empty or not. (optional)
    typeadresseerbaarobject_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    typeadresseerbaarobject_like = 'typeadresseerbaarobject_like_example' # str | Matches text using wildcards (? and *). (optional)
    typeadresseerbaarobject_not = ['typeadresseerbaarobject_not_example'] # List[str] | Exclude matches; text (optional)
    wijzigingsdatum = '2013-10-20T19:20:30+01:00' # datetime | Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast (optional)
    wijzigingsdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    woonplaats_naam = 'woonplaats_naam_example' # str | Een Woonplaats is een door het bevoegde gemeentelijke orgaan als zodanig aangewezen en van een naam voorzien gedeelte van het grondgebied van de gemeente. (optional)
    woonplaats_naam_in = ['woonplaats_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    woonplaats_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    woonplaats_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    woonplaats_naam_like = 'woonplaats_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    woonplaats_naam_not = ['woonplaats_naam_not_example'] # List[str] | Exclude matches; text (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_rolcontainer_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bag_woonplaats_identificatie=bag_woonplaats_identificatie, bag_woonplaats_identificatie_in=bag_woonplaats_identificatie_in, bag_woonplaats_identificatie_isempty=bag_woonplaats_identificatie_isempty, bag_woonplaats_identificatie_isnull=bag_woonplaats_identificatie_isnull, bag_woonplaats_identificatie_like=bag_woonplaats_identificatie_like, bag_woonplaats_identificatie_not=bag_woonplaats_identificatie_not, barcode=barcode, barcode_in=barcode_in, barcode_isempty=barcode_isempty, barcode_isnull=barcode_isnull, barcode_like=barcode_like, barcode_not=barcode_not, chip_nummer=chip_nummer, chip_nummer_in=chip_nummer_in, chip_nummer_isempty=chip_nummer_isempty, chip_nummer_isnull=chip_nummer_isnull, chip_nummer_like=chip_nummer_like, chip_nummer_not=chip_nummer_not, chip_type=chip_type, chip_type_in=chip_type_in, chip_type_isempty=chip_type_isempty, chip_type_isnull=chip_type_isnull, chip_type_like=chip_type_like, chip_type_not=chip_type_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, gebied_buurt_identificatie=gebied_buurt_identificatie, gebied_buurt_identificatie_in=gebied_buurt_identificatie_in, gebied_buurt_identificatie_isempty=gebied_buurt_identificatie_isempty, gebied_buurt_identificatie_isnull=gebied_buurt_identificatie_isnull, gebied_buurt_identificatie_like=gebied_buurt_identificatie_like, gebied_buurt_identificatie_not=gebied_buurt_identificatie_not, gebied_buurt_code=gebied_buurt_code, gebied_buurt_code_in=gebied_buurt_code_in, gebied_buurt_code_isempty=gebied_buurt_code_isempty, gebied_buurt_code_isnull=gebied_buurt_code_isnull, gebied_buurt_code_like=gebied_buurt_code_like, gebied_buurt_code_not=gebied_buurt_code_not, gebied_buurt_naam=gebied_buurt_naam, gebied_buurt_naam_in=gebied_buurt_naam_in, gebied_buurt_naam_isempty=gebied_buurt_naam_isempty, gebied_buurt_naam_isnull=gebied_buurt_naam_isnull, gebied_buurt_naam_like=gebied_buurt_naam_like, gebied_buurt_naam_not=gebied_buurt_naam_not, gebied_ggw_identificatie=gebied_ggw_identificatie, gebied_ggw_identificatie_in=gebied_ggw_identificatie_in, gebied_ggw_identificatie_isempty=gebied_ggw_identificatie_isempty, gebied_ggw_identificatie_isnull=gebied_ggw_identificatie_isnull, gebied_ggw_identificatie_like=gebied_ggw_identificatie_like, gebied_ggw_identificatie_not=gebied_ggw_identificatie_not, gebied_ggw_code=gebied_ggw_code, gebied_ggw_code_in=gebied_ggw_code_in, gebied_ggw_code_isempty=gebied_ggw_code_isempty, gebied_ggw_code_isnull=gebied_ggw_code_isnull, gebied_ggw_code_like=gebied_ggw_code_like, gebied_ggw_code_not=gebied_ggw_code_not, gebied_ggw_naam=gebied_ggw_naam, gebied_ggw_naam_in=gebied_ggw_naam_in, gebied_ggw_naam_isempty=gebied_ggw_naam_isempty, gebied_ggw_naam_isnull=gebied_ggw_naam_isnull, gebied_ggw_naam_like=gebied_ggw_naam_like, gebied_ggw_naam_not=gebied_ggw_naam_not, gebied_stadsdeel_identificatie=gebied_stadsdeel_identificatie, gebied_stadsdeel_identificatie_in=gebied_stadsdeel_identificatie_in, gebied_stadsdeel_identificatie_isempty=gebied_stadsdeel_identificatie_isempty, gebied_stadsdeel_identificatie_isnull=gebied_stadsdeel_identificatie_isnull, gebied_stadsdeel_identificatie_like=gebied_stadsdeel_identificatie_like, gebied_stadsdeel_identificatie_not=gebied_stadsdeel_identificatie_not, gebied_stadsdeel_code=gebied_stadsdeel_code, gebied_stadsdeel_code_in=gebied_stadsdeel_code_in, gebied_stadsdeel_code_isempty=gebied_stadsdeel_code_isempty, gebied_stadsdeel_code_isnull=gebied_stadsdeel_code_isnull, gebied_stadsdeel_code_like=gebied_stadsdeel_code_like, gebied_stadsdeel_code_not=gebied_stadsdeel_code_not, gebied_stadsdeel_naam=gebied_stadsdeel_naam, gebied_stadsdeel_naam_in=gebied_stadsdeel_naam_in, gebied_stadsdeel_naam_isempty=gebied_stadsdeel_naam_isempty, gebied_stadsdeel_naam_isnull=gebied_stadsdeel_naam_isnull, gebied_stadsdeel_naam_like=gebied_stadsdeel_naam_like, gebied_stadsdeel_naam_not=gebied_stadsdeel_naam_not, gebied_wijk_identificatie=gebied_wijk_identificatie, gebied_wijk_identificatie_in=gebied_wijk_identificatie_in, gebied_wijk_identificatie_isempty=gebied_wijk_identificatie_isempty, gebied_wijk_identificatie_isnull=gebied_wijk_identificatie_isnull, gebied_wijk_identificatie_like=gebied_wijk_identificatie_like, gebied_wijk_identificatie_not=gebied_wijk_identificatie_not, gebied_wijk_code=gebied_wijk_code, gebied_wijk_code_in=gebied_wijk_code_in, gebied_wijk_code_isempty=gebied_wijk_code_isempty, gebied_wijk_code_isnull=gebied_wijk_code_isnull, gebied_wijk_code_like=gebied_wijk_code_like, gebied_wijk_code_not=gebied_wijk_code_not, gebied_wijk_naam=gebied_wijk_naam, gebied_wijk_naam_in=gebied_wijk_naam_in, gebied_wijk_naam_isempty=gebied_wijk_naam_isempty, gebied_wijk_naam_isnull=gebied_wijk_naam_isnull, gebied_wijk_naam_like=gebied_wijk_naam_like, gebied_wijk_naam_not=gebied_wijk_naam_not, gebruiksdoel=gebruiksdoel, gebruiksdoel_in=gebruiksdoel_in, gebruiksdoel_isempty=gebruiksdoel_isempty, gebruiksdoel_isnull=gebruiksdoel_isnull, gebruiksdoel_like=gebruiksdoel_like, gebruiksdoel_not=gebruiksdoel_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, heeft_barcode_sinds=heeft_barcode_sinds, heeft_barcode_sinds_gt=heeft_barcode_sinds_gt, heeft_barcode_sinds_gte=heeft_barcode_sinds_gte, heeft_barcode_sinds_in=heeft_barcode_sinds_in, heeft_barcode_sinds_isnull=heeft_barcode_sinds_isnull, heeft_barcode_sinds_lt=heeft_barcode_sinds_lt, heeft_barcode_sinds_lte=heeft_barcode_sinds_lte, heeft_barcode_sinds_not=heeft_barcode_sinds_not, heeft_chip_sinds=heeft_chip_sinds, heeft_chip_sinds_gt=heeft_chip_sinds_gt, heeft_chip_sinds_gte=heeft_chip_sinds_gte, heeft_chip_sinds_in=heeft_chip_sinds_in, heeft_chip_sinds_isnull=heeft_chip_sinds_isnull, heeft_chip_sinds_lt=heeft_chip_sinds_lt, heeft_chip_sinds_lte=heeft_chip_sinds_lte, heeft_chip_sinds_not=heeft_chip_sinds_not, huisletter=huisletter, huisletter_in=huisletter_in, huisletter_isempty=huisletter_isempty, huisletter_isnull=huisletter_isnull, huisletter_like=huisletter_like, huisletter_not=huisletter_not, huisnummer=huisnummer, huisnummer_gt=huisnummer_gt, huisnummer_gte=huisnummer_gte, huisnummer_in=huisnummer_in, huisnummer_isnull=huisnummer_isnull, huisnummer_lt=huisnummer_lt, huisnummer_lte=huisnummer_lte, huisnummer_not=huisnummer_not, huisnummertoevoeging=huisnummertoevoeging, huisnummertoevoeging_in=huisnummertoevoeging_in, huisnummertoevoeging_isempty=huisnummertoevoeging_isempty, huisnummertoevoeging_isnull=huisnummertoevoeging_isnull, huisnummertoevoeging_like=huisnummertoevoeging_like, huisnummertoevoeging_not=huisnummertoevoeging_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, postcode=postcode, postcode_in=postcode_in, postcode_isempty=postcode_isempty, postcode_isnull=postcode_isnull, postcode_like=postcode_like, postcode_not=postcode_not, soort_container=soort_container, soort_container_in=soort_container_in, soort_container_isempty=soort_container_isempty, soort_container_isnull=soort_container_isnull, soort_container_like=soort_container_like, soort_container_not=soort_container_not, status=status, status_sinds=status_sinds, status_sinds_gt=status_sinds_gt, status_sinds_gte=status_sinds_gte, status_sinds_in=status_sinds_in, status_sinds_isnull=status_sinds_isnull, status_sinds_lt=status_sinds_lt, status_sinds_lte=status_sinds_lte, status_sinds_not=status_sinds_not, status_in=status_in, status_isempty=status_isempty, status_isnull=status_isnull, status_like=status_like, status_not=status_not, straatnaam=straatnaam, straatnaam_in=straatnaam_in, straatnaam_isempty=straatnaam_isempty, straatnaam_isnull=straatnaam_isnull, straatnaam_like=straatnaam_like, straatnaam_not=straatnaam_not, typeadresseerbaarobject=typeadresseerbaarobject, typeadresseerbaarobject_in=typeadresseerbaarobject_in, typeadresseerbaarobject_isempty=typeadresseerbaarobject_isempty, typeadresseerbaarobject_isnull=typeadresseerbaarobject_isnull, typeadresseerbaarobject_like=typeadresseerbaarobject_like, typeadresseerbaarobject_not=typeadresseerbaarobject_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not, woonplaats_naam=woonplaats_naam, woonplaats_naam_in=woonplaats_naam_in, woonplaats_naam_isempty=woonplaats_naam_isempty, woonplaats_naam_isnull=woonplaats_naam_isnull, woonplaats_naam_like=woonplaats_naam_like, woonplaats_naam_not=woonplaats_naam_not)
        print("The response of RolcontainerApi->huishoudelijkafval_rolcontainer_retrieve_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolcontainerApi->huishoudelijkafval_rolcontainer_retrieve_slash: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**|  | 
 **accept_crs** | **str**| Accept-Crs header for Geo queries | [optional] 
 **content_crs** | **str**| Content-Crs header for Geo queries | [optional] 
 **x_api_key** | **str**| Api Key for statistical purposes, not for authentication | [optional] 
 **csv_header** | **str**| Specify type of header for csv file | [optional] 
 **csv_separator** | **str**| Specify type of separator for csv file | [optional] 
 **expand** | **bool**| Allow to expand relations. | [optional] 
 **expand_scope** | **str**| Comma separated list of named relations to expand. | [optional] 
 **fields** | **str**| Comma-separated list of fields to display | [optional] 
 **format** | **str**| Select the export format | [optional] 
 **sort** | **str**| Which field to use when ordering the results. | [optional] 
 **aanmaakdatum** | **datetime**| Datum tijd waarop de rolcontainer in het systeem is aangemaakt | [optional] 
 **aanmaakdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aanmaakdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aanmaakdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **bag_nummeraanduiding_identificatie** | **str**| De unieke aanduiding van een nummeraanduiding | [optional] 
 **bag_nummeraanduiding_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_nummeraanduiding_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_nummeraanduiding_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_nummeraanduiding_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_nummeraanduiding_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_openbareruimte_identificatie** | **str**| Unieke identificatie van een openbare ruimte | [optional] 
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
 **bag_woonplaats_identificatie** | **str**| Unieke aanduiding van een woonplaats | [optional] 
 **bag_woonplaats_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_woonplaats_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_woonplaats_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_woonplaats_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_woonplaats_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **barcode** | **str**| De barcode van de chip dat van buitenaf leesbaar is. | [optional] 
 **barcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **barcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **barcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **barcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **barcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **chip_nummer** | **str**| Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. | [optional] 
 **chip_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **chip_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **chip_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **chip_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **chip_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **chip_type** | **str**| Het type van de chip dat aan de rolcontainer is bevestigd. | [optional] 
 **chip_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **chip_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **chip_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **chip_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **chip_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **fractie_omschrijving** | **str**| Container fractieomschrijving zoals door leverancier is geleverd. | [optional] 
 **fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gebied_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_buurt_code** | **str**| Unieke code (hier in zie je de Stadsdeel- en Wijkcode terug) | [optional] 
 **gebied_buurt_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_buurt_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_buurt_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_buurt_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_buurt_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_buurt_naam** | **str**| De naam van het object | [optional] 
 **gebied_buurt_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_buurt_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_buurt_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_buurt_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_buurt_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_ggw_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gebied_ggw_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_ggw_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_ggw_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_ggw_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_ggw_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_ggw_code** | **str**| De unieke code van het gebiedsgericht werken gebied | [optional] 
 **gebied_ggw_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_ggw_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_ggw_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_ggw_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_ggw_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_ggw_naam** | **str**| De naam van het gebiedsgericht werken gebied | [optional] 
 **gebied_ggw_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_ggw_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_ggw_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_ggw_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_ggw_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_stadsdeel_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gebied_stadsdeel_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_stadsdeel_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_stadsdeel_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_stadsdeel_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_stadsdeel_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_stadsdeel_code** | **str**| Officile code van het stadsdeel | [optional] 
 **gebied_stadsdeel_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_stadsdeel_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_stadsdeel_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_stadsdeel_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_stadsdeel_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_stadsdeel_naam** | **str**| De naam van het stadsdeel. | [optional] 
 **gebied_stadsdeel_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_stadsdeel_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_stadsdeel_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_stadsdeel_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_stadsdeel_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_wijk_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gebied_wijk_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_wijk_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_wijk_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_wijk_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_wijk_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_wijk_code** | **str**| Volledige, samengestelde, code, bestaande uit stadsdeelcode en wijkcode | [optional] 
 **gebied_wijk_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_wijk_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_wijk_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_wijk_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_wijk_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebied_wijk_naam** | **str**| De naam van de wijk | [optional] 
 **gebied_wijk_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebied_wijk_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebied_wijk_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebied_wijk_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebied_wijk_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gebruiksdoel** | **str**| Een categorisering van de gebruiksdoelen van het betreffende adreseerbareobject, zoals dit door de overheid als zodanig is toegestaan | [optional] 
 **gebruiksdoel_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gebruiksdoel_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gebruiksdoel_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gebruiksdoel_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gebruiksdoel_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de rolcontainer RD (epsg:28992). De geometrieën zijn afkomstig uit BAG.  | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **heeft_barcode_sinds** | **date**| Dit attribuut, heeft_barcode_sinds, geeft de datum aan waarop de chip is voorzien van een barcode.. | [optional] 
 **heeft_barcode_sinds_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **heeft_barcode_sinds_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **heeft_barcode_sinds_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **heeft_barcode_sinds_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **heeft_barcode_sinds_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **heeft_barcode_sinds_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **heeft_barcode_sinds_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds** | **date**| Datum waarop de chip aan de rolcontainer is bevestigd.  | [optional] 
 **heeft_chip_sinds_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **heeft_chip_sinds_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **heeft_chip_sinds_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **heeft_chip_sinds_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **huisletter** | **str**| Een alfabetisch teken achter het huisnummer zoals dit door het gemeentebestuur is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende toevoeging aan een huisnummer in de vorm van een alfabetisch teken. | [optional] 
 **huisletter_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **huisletter_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **huisletter_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **huisletter_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **huisletter_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **huisnummer** | **int**| De numerieke aanduiding zoals deze door het gemeente bestuur aan het object is toegekend dan wel een door of namens het bevoegde gemeentelijke orgaan ten aanzien van een adresseerbaar object toegekende nummering. | [optional] 
 **huisnummer_gt** | **int**| Greater than; number | [optional] 
 **huisnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **huisnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **huisnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **huisnummer_lt** | **int**| Less than; number | [optional] 
 **huisnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **huisnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **huisnummertoevoeging** | **str**| Die let­ters of te­kens die nood­za­ke­lijk zijn om, naast huis­num­mer en -let­ter, de brie­ven­bus te vin­den dan wel een door of na­mens het be­voeg­de ge­meen­te­lij­ke or­gaan ten aan­zien van een adres­seer­baar ob­ject toe­ge­ken­de toe­voe­ging aan een huis­num­mer of een com­bi­na­tie van huis­let­ter en huis­num­mer | [optional] 
 **huisnummertoevoeging_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **huisnummertoevoeging_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **huisnummertoevoeging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **huisnummertoevoeging_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **huisnummertoevoeging_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id2** | **int**| Unieke aanduiding van een rolcontainer | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **postcode** | **str**| De door de Post NL vast­ge­stel­de code be­ho­rend bij de straat­naam en het huis­num­mer dan wel de door Post NL vast­ge­stel­de code be­ho­ren­de bij een be­paal­de com­bi­na­tie van een naam open­ba­re ruim­te en een huis­num­mer. | [optional] 
 **postcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **postcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **postcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **postcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **postcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **soort_container** | **str**| Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. | [optional] 
 **soort_container_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_container_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_container_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_container_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_container_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **str**| Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. | [optional] 
 **status_sinds** | **date**| Datum waarop de laatste status van een rolcontainer van toepassing is | [optional] 
 **status_sinds_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **status_sinds_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **status_sinds_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_sinds_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_sinds_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **status_sinds_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **status_sinds_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **status_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **status_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **straatnaam** | **str**| Naam van de straat | [optional] 
 **straatnaam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **straatnaam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **straatnaam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **straatnaam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **straatnaam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **typeadresseerbaarobject** | **str**| Een Adresseerbaar object is een (abstract) object waaraan adressen kunnen worden toegekend | [optional] 
 **typeadresseerbaarobject_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **typeadresseerbaarobject_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **typeadresseerbaarobject_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **typeadresseerbaarobject_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **typeadresseerbaarobject_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **wijzigingsdatum** | **datetime**| Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast | [optional] 
 **wijzigingsdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **woonplaats_naam** | **str**| Een Woonplaats is een door het bevoegde gemeentelijke orgaan als zodanig aangewezen en van een naam voorzien gedeelte van het grondgebied van de gemeente. | [optional] 
 **woonplaats_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **woonplaats_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **woonplaats_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **woonplaats_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **woonplaats_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 

### Return type

[**Huishoudelijkafvalrolcontainer**](Huishoudelijkafvalrolcontainer.md)

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

