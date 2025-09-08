# huishoudelijkafval_api_client.ClusterApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_cluster_list_slash**](ClusterApi.md#huishoudelijkafval_cluster_list_slash) | **GET** /cluster | 
[**huishoudelijkafval_cluster_retrieve_slash**](ClusterApi.md#huishoudelijkafval_cluster_retrieve_slash) | **GET** /cluster/{id} | 


# **huishoudelijkafval_cluster_list_slash**
> PaginatedHuishoudelijkafvalclusterList huishoudelijkafval_cluster_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bronadres=bronadres, bronadres_in=bronadres_in, bronadres_isempty=bronadres_isempty, bronadres_isnull=bronadres_isnull, bronadres_like=bronadres_like, bronadres_not=bronadres_not, datum_einde=datum_einde, datum_einde_gt=datum_einde_gt, datum_einde_gte=datum_einde_gte, datum_einde_in=datum_einde_in, datum_einde_isnull=datum_einde_isnull, datum_einde_lt=datum_einde_lt, datum_einde_lte=datum_einde_lte, datum_einde_not=datum_einde_not, datum_ontstaan=datum_ontstaan, datum_ontstaan_gt=datum_ontstaan_gt, datum_ontstaan_gte=datum_ontstaan_gte, datum_ontstaan_in=datum_ontstaan_in, datum_ontstaan_isnull=datum_ontstaan_isnull, datum_ontstaan_lt=datum_ontstaan_lt, datum_ontstaan_lte=datum_ontstaan_lte, datum_ontstaan_not=datum_ontstaan_not, datum_opvoer=datum_opvoer, datum_opvoer_gt=datum_opvoer_gt, datum_opvoer_gte=datum_opvoer_gte, datum_opvoer_in=datum_opvoer_in, datum_opvoer_isnull=datum_opvoer_isnull, datum_opvoer_lt=datum_opvoer_lt, datum_opvoer_lte=datum_opvoer_lte, datum_opvoer_not=datum_opvoer_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, opmerking=opmerking, opmerking_in=opmerking_in, opmerking_isempty=opmerking_isempty, opmerking_isnull=opmerking_isnull, opmerking_like=opmerking_like, opmerking_not=opmerking_not, page=page, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, subcluster_indicatie=subcluster_indicatie, subcluster_indicatie_isnull=subcluster_indicatie_isnull, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalcluster_list import PaginatedHuishoudelijkafvalclusterList
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
    api_instance = huishoudelijkafval_api_client.ClusterApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
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
    bag_openbareruimte_identificatie = 'bag_openbareruimte_identificatie_example' # str | Unieke identificatie van een openbare ruimte (optional)
    bag_openbareruimte_identificatie_in = ['bag_openbareruimte_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_openbareruimte_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_openbareruimte_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_openbareruimte_identificatie_like = 'bag_openbareruimte_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_openbareruimte_identificatie_not = ['bag_openbareruimte_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bronadres = 'bronadres_example' # str | Adres van het cluster zoals die in bron geregistreerd is. (optional)
    bronadres_in = ['bronadres_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bronadres_isempty = True # bool | Whether the field is empty or not. (optional)
    bronadres_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bronadres_like = 'bronadres_like_example' # str | Matches text using wildcards (? and *). (optional)
    bronadres_not = ['bronadres_not_example'] # List[str] | Exclude matches; text (optional)
    datum_einde = '2013-10-20' # date | Datum wanneer het cluster geen relaties meer heeft met containers met status=1. (optional)
    datum_einde_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_einde_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_einde_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_einde_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_einde_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_einde_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_einde_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_ontstaan = '2013-10-20' # date | Datum ontstaan van het cluster. Dit is afgeleid van de plaatsingsdatum van de oudste container ,wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 (optional)
    datum_ontstaan_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_ontstaan_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_ontstaan_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_ontstaan_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_ontstaan_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_ontstaan_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_ontstaan_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_opvoer = '2013-10-20T19:20:30+01:00' # datetime | Datum opvoer van het cluster. Dit is afgeleid van wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 (optional)
    datum_opvoer_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_opvoer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_opvoer_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de het zwaartepunt van het cluster in RD (epsg:28992)) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id = 'id_example' # str | Uniek identificerend kenmerk van cluster (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    opmerking = 'opmerking_example' # str | Extra aanwijzing van de locatie voor de bestuurder. (optional)
    opmerking_in = ['opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    opmerking_like = 'opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    opmerking_not = ['opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    status = 56 # int | Status van het cluster (0 - inactief , 1 - actief) (optional)
    status_gt = 56 # int | Greater than; number (optional)
    status_gte = 56 # int | Greater than or equal to; number (optional)
    status_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_lt = 56 # int | Less than; number (optional)
    status_lte = 56 # int | Less than or equal to; number (optional)
    status_not = [56] # List[int] | Exclude matches; number (optional)
    subcluster_indicatie = True # bool | Indicatie of het een cluster betreft dat is gesplitst door een weg (optional)
    subcluster_indicatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
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
        api_response = await api_instance.huishoudelijkafval_cluster_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bronadres=bronadres, bronadres_in=bronadres_in, bronadres_isempty=bronadres_isempty, bronadres_isnull=bronadres_isnull, bronadres_like=bronadres_like, bronadres_not=bronadres_not, datum_einde=datum_einde, datum_einde_gt=datum_einde_gt, datum_einde_gte=datum_einde_gte, datum_einde_in=datum_einde_in, datum_einde_isnull=datum_einde_isnull, datum_einde_lt=datum_einde_lt, datum_einde_lte=datum_einde_lte, datum_einde_not=datum_einde_not, datum_ontstaan=datum_ontstaan, datum_ontstaan_gt=datum_ontstaan_gt, datum_ontstaan_gte=datum_ontstaan_gte, datum_ontstaan_in=datum_ontstaan_in, datum_ontstaan_isnull=datum_ontstaan_isnull, datum_ontstaan_lt=datum_ontstaan_lt, datum_ontstaan_lte=datum_ontstaan_lte, datum_ontstaan_not=datum_ontstaan_not, datum_opvoer=datum_opvoer, datum_opvoer_gt=datum_opvoer_gt, datum_opvoer_gte=datum_opvoer_gte, datum_opvoer_in=datum_opvoer_in, datum_opvoer_isnull=datum_opvoer_isnull, datum_opvoer_lt=datum_opvoer_lt, datum_opvoer_lte=datum_opvoer_lte, datum_opvoer_not=datum_opvoer_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, opmerking=opmerking, opmerking_in=opmerking_in, opmerking_isempty=opmerking_isempty, opmerking_isnull=opmerking_isnull, opmerking_like=opmerking_like, opmerking_not=opmerking_not, page=page, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, subcluster_indicatie=subcluster_indicatie, subcluster_indicatie_isnull=subcluster_indicatie_isnull, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ClusterApi->huishoudelijkafval_cluster_list_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClusterApi->huishoudelijkafval_cluster_list_slash: %s\n" % e)
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
 **bag_openbareruimte_identificatie** | **str**| Unieke identificatie van een openbare ruimte | [optional] 
 **bag_openbareruimte_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_openbareruimte_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_openbareruimte_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_openbareruimte_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_openbareruimte_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bronadres** | **str**| Adres van het cluster zoals die in bron geregistreerd is. | [optional] 
 **bronadres_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bronadres_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bronadres_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bronadres_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bronadres_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_einde** | **date**| Datum wanneer het cluster geen relaties meer heeft met containers met status&#x3D;1. | [optional] 
 **datum_einde_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_einde_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_einde_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_einde_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_einde_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_einde_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_einde_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_ontstaan** | **date**| Datum ontstaan van het cluster. Dit is afgeleid van de plaatsingsdatum van de oudste container ,wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 | [optional] 
 **datum_ontstaan_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_ontstaan_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_ontstaan_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_ontstaan_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_ontstaan_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_ontstaan_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_ontstaan_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_opvoer** | **datetime**| Datum opvoer van het cluster. Dit is afgeleid van wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 | [optional] 
 **datum_opvoer_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_opvoer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_opvoer_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de het zwaartepunt van het cluster in RD (epsg:28992)) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id** | **str**| Uniek identificerend kenmerk van cluster | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **opmerking** | **str**| Extra aanwijzing van de locatie voor de bestuurder. | [optional] 
 **opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **status** | **int**| Status van het cluster (0 - inactief , 1 - actief) | [optional] 
 **status_gt** | **int**| Greater than; number | [optional] 
 **status_gte** | **int**| Greater than or equal to; number | [optional] 
 **status_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_lt** | **int**| Less than; number | [optional] 
 **status_lte** | **int**| Less than or equal to; number | [optional] 
 **status_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **subcluster_indicatie** | **bool**| Indicatie of het een cluster betreft dat is gesplitst door een weg | [optional] 
 **subcluster_indicatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
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

[**PaginatedHuishoudelijkafvalclusterList**](PaginatedHuishoudelijkafvalclusterList.md)

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

# **huishoudelijkafval_cluster_retrieve_slash**
> Huishoudelijkafvalcluster huishoudelijkafval_cluster_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bronadres=bronadres, bronadres_in=bronadres_in, bronadres_isempty=bronadres_isempty, bronadres_isnull=bronadres_isnull, bronadres_like=bronadres_like, bronadres_not=bronadres_not, datum_einde=datum_einde, datum_einde_gt=datum_einde_gt, datum_einde_gte=datum_einde_gte, datum_einde_in=datum_einde_in, datum_einde_isnull=datum_einde_isnull, datum_einde_lt=datum_einde_lt, datum_einde_lte=datum_einde_lte, datum_einde_not=datum_einde_not, datum_ontstaan=datum_ontstaan, datum_ontstaan_gt=datum_ontstaan_gt, datum_ontstaan_gte=datum_ontstaan_gte, datum_ontstaan_in=datum_ontstaan_in, datum_ontstaan_isnull=datum_ontstaan_isnull, datum_ontstaan_lt=datum_ontstaan_lt, datum_ontstaan_lte=datum_ontstaan_lte, datum_ontstaan_not=datum_ontstaan_not, datum_opvoer=datum_opvoer, datum_opvoer_gt=datum_opvoer_gt, datum_opvoer_gte=datum_opvoer_gte, datum_opvoer_in=datum_opvoer_in, datum_opvoer_isnull=datum_opvoer_isnull, datum_opvoer_lt=datum_opvoer_lt, datum_opvoer_lte=datum_opvoer_lte, datum_opvoer_not=datum_opvoer_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, opmerking=opmerking, opmerking_in=opmerking_in, opmerking_isempty=opmerking_isempty, opmerking_isnull=opmerking_isnull, opmerking_like=opmerking_like, opmerking_not=opmerking_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, subcluster_indicatie=subcluster_indicatie, subcluster_indicatie_isnull=subcluster_indicatie_isnull, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalcluster import Huishoudelijkafvalcluster
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
    api_instance = huishoudelijkafval_api_client.ClusterApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
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
    bag_openbareruimte_identificatie = 'bag_openbareruimte_identificatie_example' # str | Unieke identificatie van een openbare ruimte (optional)
    bag_openbareruimte_identificatie_in = ['bag_openbareruimte_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_openbareruimte_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_openbareruimte_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_openbareruimte_identificatie_like = 'bag_openbareruimte_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_openbareruimte_identificatie_not = ['bag_openbareruimte_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bronadres = 'bronadres_example' # str | Adres van het cluster zoals die in bron geregistreerd is. (optional)
    bronadres_in = ['bronadres_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bronadres_isempty = True # bool | Whether the field is empty or not. (optional)
    bronadres_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bronadres_like = 'bronadres_like_example' # str | Matches text using wildcards (? and *). (optional)
    bronadres_not = ['bronadres_not_example'] # List[str] | Exclude matches; text (optional)
    datum_einde = '2013-10-20' # date | Datum wanneer het cluster geen relaties meer heeft met containers met status=1. (optional)
    datum_einde_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_einde_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_einde_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_einde_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_einde_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_einde_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_einde_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_ontstaan = '2013-10-20' # date | Datum ontstaan van het cluster. Dit is afgeleid van de plaatsingsdatum van de oudste container ,wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 (optional)
    datum_ontstaan_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_ontstaan_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_ontstaan_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_ontstaan_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_ontstaan_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_ontstaan_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_ontstaan_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_opvoer = '2013-10-20T19:20:30+01:00' # datetime | Datum opvoer van het cluster. Dit is afgeleid van wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 (optional)
    datum_opvoer_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_opvoer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_opvoer_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de het zwaartepunt van het cluster in RD (epsg:28992)) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id2 = 'id_example' # str | Uniek identificerend kenmerk van cluster (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    opmerking = 'opmerking_example' # str | Extra aanwijzing van de locatie voor de bestuurder. (optional)
    opmerking_in = ['opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    opmerking_like = 'opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    opmerking_not = ['opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    status = 56 # int | Status van het cluster (0 - inactief , 1 - actief) (optional)
    status_gt = 56 # int | Greater than; number (optional)
    status_gte = 56 # int | Greater than or equal to; number (optional)
    status_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_lt = 56 # int | Less than; number (optional)
    status_lte = 56 # int | Less than or equal to; number (optional)
    status_not = [56] # List[int] | Exclude matches; number (optional)
    subcluster_indicatie = True # bool | Indicatie of het een cluster betreft dat is gesplitst door een weg (optional)
    subcluster_indicatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
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
        api_response = await api_instance.huishoudelijkafval_cluster_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_hoofdadres_verblijfsobject_identificatie=bag_hoofdadres_verblijfsobject_identificatie, bag_hoofdadres_verblijfsobject_identificatie_in=bag_hoofdadres_verblijfsobject_identificatie_in, bag_hoofdadres_verblijfsobject_identificatie_isempty=bag_hoofdadres_verblijfsobject_identificatie_isempty, bag_hoofdadres_verblijfsobject_identificatie_isnull=bag_hoofdadres_verblijfsobject_identificatie_isnull, bag_hoofdadres_verblijfsobject_identificatie_like=bag_hoofdadres_verblijfsobject_identificatie_like, bag_hoofdadres_verblijfsobject_identificatie_not=bag_hoofdadres_verblijfsobject_identificatie_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_openbareruimte_identificatie=bag_openbareruimte_identificatie, bag_openbareruimte_identificatie_in=bag_openbareruimte_identificatie_in, bag_openbareruimte_identificatie_isempty=bag_openbareruimte_identificatie_isempty, bag_openbareruimte_identificatie_isnull=bag_openbareruimte_identificatie_isnull, bag_openbareruimte_identificatie_like=bag_openbareruimte_identificatie_like, bag_openbareruimte_identificatie_not=bag_openbareruimte_identificatie_not, bronadres=bronadres, bronadres_in=bronadres_in, bronadres_isempty=bronadres_isempty, bronadres_isnull=bronadres_isnull, bronadres_like=bronadres_like, bronadres_not=bronadres_not, datum_einde=datum_einde, datum_einde_gt=datum_einde_gt, datum_einde_gte=datum_einde_gte, datum_einde_in=datum_einde_in, datum_einde_isnull=datum_einde_isnull, datum_einde_lt=datum_einde_lt, datum_einde_lte=datum_einde_lte, datum_einde_not=datum_einde_not, datum_ontstaan=datum_ontstaan, datum_ontstaan_gt=datum_ontstaan_gt, datum_ontstaan_gte=datum_ontstaan_gte, datum_ontstaan_in=datum_ontstaan_in, datum_ontstaan_isnull=datum_ontstaan_isnull, datum_ontstaan_lt=datum_ontstaan_lt, datum_ontstaan_lte=datum_ontstaan_lte, datum_ontstaan_not=datum_ontstaan_not, datum_opvoer=datum_opvoer, datum_opvoer_gt=datum_opvoer_gt, datum_opvoer_gte=datum_opvoer_gte, datum_opvoer_in=datum_opvoer_in, datum_opvoer_isnull=datum_opvoer_isnull, datum_opvoer_lt=datum_opvoer_lt, datum_opvoer_lte=datum_opvoer_lte, datum_opvoer_not=datum_opvoer_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, opmerking=opmerking, opmerking_in=opmerking_in, opmerking_isempty=opmerking_isempty, opmerking_isnull=opmerking_isnull, opmerking_like=opmerking_like, opmerking_not=opmerking_not, status=status, status_gt=status_gt, status_gte=status_gte, status_in=status_in, status_isnull=status_isnull, status_lt=status_lt, status_lte=status_lte, status_not=status_not, subcluster_indicatie=subcluster_indicatie, subcluster_indicatie_isnull=subcluster_indicatie_isnull, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ClusterApi->huishoudelijkafval_cluster_retrieve_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClusterApi->huishoudelijkafval_cluster_retrieve_slash: %s\n" % e)
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
 **bag_openbareruimte_identificatie** | **str**| Unieke identificatie van een openbare ruimte | [optional] 
 **bag_openbareruimte_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_openbareruimte_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_openbareruimte_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_openbareruimte_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_openbareruimte_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bronadres** | **str**| Adres van het cluster zoals die in bron geregistreerd is. | [optional] 
 **bronadres_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bronadres_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bronadres_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bronadres_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bronadres_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_einde** | **date**| Datum wanneer het cluster geen relaties meer heeft met containers met status&#x3D;1. | [optional] 
 **datum_einde_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_einde_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_einde_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_einde_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_einde_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_einde_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_einde_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_ontstaan** | **date**| Datum ontstaan van het cluster. Dit is afgeleid van de plaatsingsdatum van de oudste container ,wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 | [optional] 
 **datum_ontstaan_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_ontstaan_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_ontstaan_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_ontstaan_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_ontstaan_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_ontstaan_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_ontstaan_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_opvoer** | **datetime**| Datum opvoer van het cluster. Dit is afgeleid van wanneer het gegeven bij het systeem bekend is of peildatum 01-01-2016 | [optional] 
 **datum_opvoer_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_opvoer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_opvoer_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de het zwaartepunt van het cluster in RD (epsg:28992)) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id2** | **str**| Uniek identificerend kenmerk van cluster | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **opmerking** | **str**| Extra aanwijzing van de locatie voor de bestuurder. | [optional] 
 **opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **int**| Status van het cluster (0 - inactief , 1 - actief) | [optional] 
 **status_gt** | **int**| Greater than; number | [optional] 
 **status_gte** | **int**| Greater than or equal to; number | [optional] 
 **status_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_lt** | **int**| Less than; number | [optional] 
 **status_lte** | **int**| Less than or equal to; number | [optional] 
 **status_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **subcluster_indicatie** | **bool**| Indicatie of het een cluster betreft dat is gesplitst door een weg | [optional] 
 **subcluster_indicatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
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

[**Huishoudelijkafvalcluster**](Huishoudelijkafvalcluster.md)

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

