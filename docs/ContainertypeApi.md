# huishoudelijkafval_api_client.ContainertypeApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_containertype_list_slash**](ContainertypeApi.md#huishoudelijkafval_containertype_list_slash) | **GET** /containertype | 
[**huishoudelijkafval_containertype_retrieve_slash**](ContainertypeApi.md#huishoudelijkafval_containertype_retrieve_slash) | **GET** /containertype/{id} | 


# **huishoudelijkafval_containertype_list_slash**
> PaginatedHuishoudelijkafvalcontainertypeList huishoudelijkafval_containertype_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, containertype_artikelcode=containertype_artikelcode, containertype_artikelcode_in=containertype_artikelcode_in, containertype_artikelcode_isempty=containertype_artikelcode_isempty, containertype_artikelcode_isnull=containertype_artikelcode_isnull, containertype_artikelcode_like=containertype_artikelcode_like, containertype_artikelcode_not=containertype_artikelcode_not, containertype_compressie_container_ind=containertype_compressie_container_ind, containertype_compressie_container_ind_isnull=containertype_compressie_container_ind_isnull, containertype_compressiefactor=containertype_compressiefactor, containertype_compressiefactor_in=containertype_compressiefactor_in, containertype_compressiefactor_isempty=containertype_compressiefactor_isempty, containertype_compressiefactor_isnull=containertype_compressiefactor_isnull, containertype_compressiefactor_like=containertype_compressiefactor_like, containertype_compressiefactor_not=containertype_compressiefactor_not, containertype_container_type=containertype_container_type, containertype_container_type_in=containertype_container_type_in, containertype_container_type_isempty=containertype_container_type_isempty, containertype_container_type_isnull=containertype_container_type_isnull, containertype_container_type_like=containertype_container_type_like, containertype_container_type_not=containertype_container_type_not, containertype_hijskraan_opmerking=containertype_hijskraan_opmerking, containertype_hijskraan_opmerking_in=containertype_hijskraan_opmerking_in, containertype_hijskraan_opmerking_isempty=containertype_hijskraan_opmerking_isempty, containertype_hijskraan_opmerking_isnull=containertype_hijskraan_opmerking_isnull, containertype_hijskraan_opmerking_like=containertype_hijskraan_opmerking_like, containertype_hijskraan_opmerking_not=containertype_hijskraan_opmerking_not, containertype_hijskraantype_naam=containertype_hijskraantype_naam, containertype_hijskraantype_naam_in=containertype_hijskraantype_naam_in, containertype_hijskraantype_naam_isempty=containertype_hijskraantype_naam_isempty, containertype_hijskraantype_naam_isnull=containertype_hijskraantype_naam_isnull, containertype_hijskraantype_naam_like=containertype_hijskraantype_naam_like, containertype_hijskraantype_naam_not=containertype_hijskraantype_naam_not, gewicht_kg=gewicht_kg, gewicht_kg_gt=gewicht_kg_gt, gewicht_kg_gte=gewicht_kg_gte, gewicht_kg_in=gewicht_kg_in, gewicht_kg_isnull=gewicht_kg_isnull, gewicht_kg_lt=gewicht_kg_lt, gewicht_kg_lte=gewicht_kg_lte, gewicht_kg_not=gewicht_kg_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, naam=naam, naam_in=naam_in, naam_isempty=naam_isempty, naam_isnull=naam_isnull, naam_like=naam_like, naam_not=naam_not, page=page, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volume_m3=volume_m3, volume_m3_gt=volume_m3_gt, volume_m3_gte=volume_m3_gte, volume_m3_in=volume_m3_in, volume_m3_isnull=volume_m3_isnull, volume_m3_lt=volume_m3_lt, volume_m3_lte=volume_m3_lte, volume_m3_not=volume_m3_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalcontainertype_list import PaginatedHuishoudelijkafvalcontainertypeList
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
    api_instance = huishoudelijkafval_api_client.ContainertypeApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'expand_scope_example' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    containertype_artikelcode = 'containertype_artikelcode_example' # str | Artikelcodevan het het containertype. (optional)
    containertype_artikelcode_in = ['containertype_artikelcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_artikelcode_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_artikelcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_artikelcode_like = 'containertype_artikelcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_artikelcode_not = ['containertype_artikelcode_not_example'] # List[str] | Exclude matches; text (optional)
    containertype_compressie_container_ind = True # bool | Indicatie voor aanwezigheid van compressie instrument. (optional)
    containertype_compressie_container_ind_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_compressiefactor = 'containertype_compressiefactor_example' # str | De compressiefactor van compressie instrument (optional)
    containertype_compressiefactor_in = ['containertype_compressiefactor_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_compressiefactor_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_compressiefactor_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_compressiefactor_like = 'containertype_compressiefactor_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_compressiefactor_not = ['containertype_compressiefactor_not_example'] # List[str] | Exclude matches; text (optional)
    containertype_container_type = 'containertype_container_type_example' # str | Het type van de container type (optional)
    containertype_container_type_in = ['containertype_container_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_container_type_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_container_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_container_type_like = 'containertype_container_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_container_type_not = ['containertype_container_type_not_example'] # List[str] | Exclude matches; text (optional)
    containertype_hijskraan_opmerking = 'containertype_hijskraan_opmerking_example' # str | Opmerking over het hijskraantype (optional)
    containertype_hijskraan_opmerking_in = ['containertype_hijskraan_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_hijskraan_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_hijskraan_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_hijskraan_opmerking_like = 'containertype_hijskraan_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_hijskraan_opmerking_not = ['containertype_hijskraan_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    containertype_hijskraantype_naam = 'containertype_hijskraantype_naam_example' # str | Naam van het type hijskraantype. (optional)
    containertype_hijskraantype_naam_in = ['containertype_hijskraantype_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_hijskraantype_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_hijskraantype_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_hijskraantype_naam_like = 'containertype_hijskraantype_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_hijskraantype_naam_not = ['containertype_hijskraantype_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gewicht_kg = 56 # int | Het volume (m3) aan afval wat de container kan bevatten (optional)
    gewicht_kg_gt = 56 # int | Greater than; number (optional)
    gewicht_kg_gte = 56 # int | Greater than or equal to; number (optional)
    gewicht_kg_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gewicht_kg_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gewicht_kg_lt = 56 # int | Less than; number (optional)
    gewicht_kg_lte = 56 # int | Less than or equal to; number (optional)
    gewicht_kg_not = [56] # List[int] | Exclude matches; number (optional)
    id = 'id_example' # str | Unieke aanduiding objecttype (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    naam = 'naam_example' # str | Naam van het containertype (optional)
    naam_in = ['naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    naam_isempty = True # bool | Whether the field is empty or not. (optional)
    naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    naam_like = 'naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    naam_not = ['naam_not_example'] # List[str] | Exclude matches; text (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    verwijderd_dp = True # bool | Indicatie of het object verwijderd is bij de bronhouder (optional)
    verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volume_m3 = 3.4 # float | Het volume (m3) aan afval wat de container kan bevatten (optional)
    volume_m3_gt = 3.4 # float | Greater than; number (optional)
    volume_m3_gte = 3.4 # float | Greater than or equal to; number (optional)
    volume_m3_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    volume_m3_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volume_m3_lt = 3.4 # float | Less than; number (optional)
    volume_m3_lte = 3.4 # float | Less than or equal to; number (optional)
    volume_m3_not = [3.4] # List[float] | Exclude matches; number (optional)
    wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop het object is gewijzigd (optional)
    wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_containertype_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, containertype_artikelcode=containertype_artikelcode, containertype_artikelcode_in=containertype_artikelcode_in, containertype_artikelcode_isempty=containertype_artikelcode_isempty, containertype_artikelcode_isnull=containertype_artikelcode_isnull, containertype_artikelcode_like=containertype_artikelcode_like, containertype_artikelcode_not=containertype_artikelcode_not, containertype_compressie_container_ind=containertype_compressie_container_ind, containertype_compressie_container_ind_isnull=containertype_compressie_container_ind_isnull, containertype_compressiefactor=containertype_compressiefactor, containertype_compressiefactor_in=containertype_compressiefactor_in, containertype_compressiefactor_isempty=containertype_compressiefactor_isempty, containertype_compressiefactor_isnull=containertype_compressiefactor_isnull, containertype_compressiefactor_like=containertype_compressiefactor_like, containertype_compressiefactor_not=containertype_compressiefactor_not, containertype_container_type=containertype_container_type, containertype_container_type_in=containertype_container_type_in, containertype_container_type_isempty=containertype_container_type_isempty, containertype_container_type_isnull=containertype_container_type_isnull, containertype_container_type_like=containertype_container_type_like, containertype_container_type_not=containertype_container_type_not, containertype_hijskraan_opmerking=containertype_hijskraan_opmerking, containertype_hijskraan_opmerking_in=containertype_hijskraan_opmerking_in, containertype_hijskraan_opmerking_isempty=containertype_hijskraan_opmerking_isempty, containertype_hijskraan_opmerking_isnull=containertype_hijskraan_opmerking_isnull, containertype_hijskraan_opmerking_like=containertype_hijskraan_opmerking_like, containertype_hijskraan_opmerking_not=containertype_hijskraan_opmerking_not, containertype_hijskraantype_naam=containertype_hijskraantype_naam, containertype_hijskraantype_naam_in=containertype_hijskraantype_naam_in, containertype_hijskraantype_naam_isempty=containertype_hijskraantype_naam_isempty, containertype_hijskraantype_naam_isnull=containertype_hijskraantype_naam_isnull, containertype_hijskraantype_naam_like=containertype_hijskraantype_naam_like, containertype_hijskraantype_naam_not=containertype_hijskraantype_naam_not, gewicht_kg=gewicht_kg, gewicht_kg_gt=gewicht_kg_gt, gewicht_kg_gte=gewicht_kg_gte, gewicht_kg_in=gewicht_kg_in, gewicht_kg_isnull=gewicht_kg_isnull, gewicht_kg_lt=gewicht_kg_lt, gewicht_kg_lte=gewicht_kg_lte, gewicht_kg_not=gewicht_kg_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, naam=naam, naam_in=naam_in, naam_isempty=naam_isempty, naam_isnull=naam_isnull, naam_like=naam_like, naam_not=naam_not, page=page, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volume_m3=volume_m3, volume_m3_gt=volume_m3_gt, volume_m3_gte=volume_m3_gte, volume_m3_in=volume_m3_in, volume_m3_isnull=volume_m3_isnull, volume_m3_lt=volume_m3_lt, volume_m3_lte=volume_m3_lte, volume_m3_not=volume_m3_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ContainertypeApi->huishoudelijkafval_containertype_list_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContainertypeApi->huishoudelijkafval_containertype_list_slash: %s\n" % e)
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
 **containertype_artikelcode** | **str**| Artikelcodevan het het containertype. | [optional] 
 **containertype_artikelcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_artikelcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_artikelcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_artikelcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_artikelcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containertype_compressie_container_ind** | **bool**| Indicatie voor aanwezigheid van compressie instrument. | [optional] 
 **containertype_compressie_container_ind_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_compressiefactor** | **str**| De compressiefactor van compressie instrument | [optional] 
 **containertype_compressiefactor_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_compressiefactor_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_compressiefactor_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_compressiefactor_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_compressiefactor_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containertype_container_type** | **str**| Het type van de container type | [optional] 
 **containertype_container_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_container_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_container_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_container_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_container_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containertype_hijskraan_opmerking** | **str**| Opmerking over het hijskraantype | [optional] 
 **containertype_hijskraan_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_hijskraan_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_hijskraan_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_hijskraan_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_hijskraan_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containertype_hijskraantype_naam** | **str**| Naam van het type hijskraantype. | [optional] 
 **containertype_hijskraantype_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_hijskraantype_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_hijskraantype_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_hijskraantype_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_hijskraantype_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gewicht_kg** | **int**| Het volume (m3) aan afval wat de container kan bevatten | [optional] 
 **gewicht_kg_gt** | **int**| Greater than; number | [optional] 
 **gewicht_kg_gte** | **int**| Greater than or equal to; number | [optional] 
 **gewicht_kg_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gewicht_kg_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gewicht_kg_lt** | **int**| Less than; number | [optional] 
 **gewicht_kg_lte** | **int**| Less than or equal to; number | [optional] 
 **gewicht_kg_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **id** | **str**| Unieke aanduiding objecttype | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **naam** | **str**| Naam van het containertype | [optional] 
 **naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **verwijderd_dp** | **bool**| Indicatie of het object verwijderd is bij de bronhouder | [optional] 
 **verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volume_m3** | **float**| Het volume (m3) aan afval wat de container kan bevatten | [optional] 
 **volume_m3_gt** | **float**| Greater than; number | [optional] 
 **volume_m3_gte** | **float**| Greater than or equal to; number | [optional] 
 **volume_m3_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **volume_m3_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volume_m3_lt** | **float**| Less than; number | [optional] 
 **volume_m3_lte** | **float**| Less than or equal to; number | [optional] 
 **volume_m3_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **wijzigingsdatum_dp** | **datetime**| Datum waarop het object is gewijzigd | [optional] 
 **wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalcontainertypeList**](PaginatedHuishoudelijkafvalcontainertypeList.md)

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

# **huishoudelijkafval_containertype_retrieve_slash**
> Huishoudelijkafvalcontainertype huishoudelijkafval_containertype_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, containertype_artikelcode=containertype_artikelcode, containertype_artikelcode_in=containertype_artikelcode_in, containertype_artikelcode_isempty=containertype_artikelcode_isempty, containertype_artikelcode_isnull=containertype_artikelcode_isnull, containertype_artikelcode_like=containertype_artikelcode_like, containertype_artikelcode_not=containertype_artikelcode_not, containertype_compressie_container_ind=containertype_compressie_container_ind, containertype_compressie_container_ind_isnull=containertype_compressie_container_ind_isnull, containertype_compressiefactor=containertype_compressiefactor, containertype_compressiefactor_in=containertype_compressiefactor_in, containertype_compressiefactor_isempty=containertype_compressiefactor_isempty, containertype_compressiefactor_isnull=containertype_compressiefactor_isnull, containertype_compressiefactor_like=containertype_compressiefactor_like, containertype_compressiefactor_not=containertype_compressiefactor_not, containertype_container_type=containertype_container_type, containertype_container_type_in=containertype_container_type_in, containertype_container_type_isempty=containertype_container_type_isempty, containertype_container_type_isnull=containertype_container_type_isnull, containertype_container_type_like=containertype_container_type_like, containertype_container_type_not=containertype_container_type_not, containertype_hijskraan_opmerking=containertype_hijskraan_opmerking, containertype_hijskraan_opmerking_in=containertype_hijskraan_opmerking_in, containertype_hijskraan_opmerking_isempty=containertype_hijskraan_opmerking_isempty, containertype_hijskraan_opmerking_isnull=containertype_hijskraan_opmerking_isnull, containertype_hijskraan_opmerking_like=containertype_hijskraan_opmerking_like, containertype_hijskraan_opmerking_not=containertype_hijskraan_opmerking_not, containertype_hijskraantype_naam=containertype_hijskraantype_naam, containertype_hijskraantype_naam_in=containertype_hijskraantype_naam_in, containertype_hijskraantype_naam_isempty=containertype_hijskraantype_naam_isempty, containertype_hijskraantype_naam_isnull=containertype_hijskraantype_naam_isnull, containertype_hijskraantype_naam_like=containertype_hijskraantype_naam_like, containertype_hijskraantype_naam_not=containertype_hijskraantype_naam_not, gewicht_kg=gewicht_kg, gewicht_kg_gt=gewicht_kg_gt, gewicht_kg_gte=gewicht_kg_gte, gewicht_kg_in=gewicht_kg_in, gewicht_kg_isnull=gewicht_kg_isnull, gewicht_kg_lt=gewicht_kg_lt, gewicht_kg_lte=gewicht_kg_lte, gewicht_kg_not=gewicht_kg_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, naam=naam, naam_in=naam_in, naam_isempty=naam_isempty, naam_isnull=naam_isnull, naam_like=naam_like, naam_not=naam_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volume_m3=volume_m3, volume_m3_gt=volume_m3_gt, volume_m3_gte=volume_m3_gte, volume_m3_in=volume_m3_in, volume_m3_isnull=volume_m3_isnull, volume_m3_lt=volume_m3_lt, volume_m3_lte=volume_m3_lte, volume_m3_not=volume_m3_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalcontainertype import Huishoudelijkafvalcontainertype
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
    api_instance = huishoudelijkafval_api_client.ContainertypeApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'expand_scope_example' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    containertype_artikelcode = 'containertype_artikelcode_example' # str | Artikelcodevan het het containertype. (optional)
    containertype_artikelcode_in = ['containertype_artikelcode_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_artikelcode_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_artikelcode_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_artikelcode_like = 'containertype_artikelcode_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_artikelcode_not = ['containertype_artikelcode_not_example'] # List[str] | Exclude matches; text (optional)
    containertype_compressie_container_ind = True # bool | Indicatie voor aanwezigheid van compressie instrument. (optional)
    containertype_compressie_container_ind_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_compressiefactor = 'containertype_compressiefactor_example' # str | De compressiefactor van compressie instrument (optional)
    containertype_compressiefactor_in = ['containertype_compressiefactor_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_compressiefactor_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_compressiefactor_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_compressiefactor_like = 'containertype_compressiefactor_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_compressiefactor_not = ['containertype_compressiefactor_not_example'] # List[str] | Exclude matches; text (optional)
    containertype_container_type = 'containertype_container_type_example' # str | Het type van de container type (optional)
    containertype_container_type_in = ['containertype_container_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_container_type_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_container_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_container_type_like = 'containertype_container_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_container_type_not = ['containertype_container_type_not_example'] # List[str] | Exclude matches; text (optional)
    containertype_hijskraan_opmerking = 'containertype_hijskraan_opmerking_example' # str | Opmerking over het hijskraantype (optional)
    containertype_hijskraan_opmerking_in = ['containertype_hijskraan_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_hijskraan_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_hijskraan_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_hijskraan_opmerking_like = 'containertype_hijskraan_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_hijskraan_opmerking_not = ['containertype_hijskraan_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    containertype_hijskraantype_naam = 'containertype_hijskraantype_naam_example' # str | Naam van het type hijskraantype. (optional)
    containertype_hijskraantype_naam_in = ['containertype_hijskraantype_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containertype_hijskraantype_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    containertype_hijskraantype_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containertype_hijskraantype_naam_like = 'containertype_hijskraantype_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    containertype_hijskraantype_naam_not = ['containertype_hijskraantype_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gewicht_kg = 56 # int | Het volume (m3) aan afval wat de container kan bevatten (optional)
    gewicht_kg_gt = 56 # int | Greater than; number (optional)
    gewicht_kg_gte = 56 # int | Greater than or equal to; number (optional)
    gewicht_kg_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gewicht_kg_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gewicht_kg_lt = 56 # int | Less than; number (optional)
    gewicht_kg_lte = 56 # int | Less than or equal to; number (optional)
    gewicht_kg_not = [56] # List[int] | Exclude matches; number (optional)
    id2 = 'id_example' # str | Unieke aanduiding objecttype (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    naam = 'naam_example' # str | Naam van het containertype (optional)
    naam_in = ['naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    naam_isempty = True # bool | Whether the field is empty or not. (optional)
    naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    naam_like = 'naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    naam_not = ['naam_not_example'] # List[str] | Exclude matches; text (optional)
    verwijderd_dp = True # bool | Indicatie of het object verwijderd is bij de bronhouder (optional)
    verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volume_m3 = 3.4 # float | Het volume (m3) aan afval wat de container kan bevatten (optional)
    volume_m3_gt = 3.4 # float | Greater than; number (optional)
    volume_m3_gte = 3.4 # float | Greater than or equal to; number (optional)
    volume_m3_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    volume_m3_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volume_m3_lt = 3.4 # float | Less than; number (optional)
    volume_m3_lte = 3.4 # float | Less than or equal to; number (optional)
    volume_m3_not = [3.4] # List[float] | Exclude matches; number (optional)
    wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop het object is gewijzigd (optional)
    wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_containertype_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, containertype_artikelcode=containertype_artikelcode, containertype_artikelcode_in=containertype_artikelcode_in, containertype_artikelcode_isempty=containertype_artikelcode_isempty, containertype_artikelcode_isnull=containertype_artikelcode_isnull, containertype_artikelcode_like=containertype_artikelcode_like, containertype_artikelcode_not=containertype_artikelcode_not, containertype_compressie_container_ind=containertype_compressie_container_ind, containertype_compressie_container_ind_isnull=containertype_compressie_container_ind_isnull, containertype_compressiefactor=containertype_compressiefactor, containertype_compressiefactor_in=containertype_compressiefactor_in, containertype_compressiefactor_isempty=containertype_compressiefactor_isempty, containertype_compressiefactor_isnull=containertype_compressiefactor_isnull, containertype_compressiefactor_like=containertype_compressiefactor_like, containertype_compressiefactor_not=containertype_compressiefactor_not, containertype_container_type=containertype_container_type, containertype_container_type_in=containertype_container_type_in, containertype_container_type_isempty=containertype_container_type_isempty, containertype_container_type_isnull=containertype_container_type_isnull, containertype_container_type_like=containertype_container_type_like, containertype_container_type_not=containertype_container_type_not, containertype_hijskraan_opmerking=containertype_hijskraan_opmerking, containertype_hijskraan_opmerking_in=containertype_hijskraan_opmerking_in, containertype_hijskraan_opmerking_isempty=containertype_hijskraan_opmerking_isempty, containertype_hijskraan_opmerking_isnull=containertype_hijskraan_opmerking_isnull, containertype_hijskraan_opmerking_like=containertype_hijskraan_opmerking_like, containertype_hijskraan_opmerking_not=containertype_hijskraan_opmerking_not, containertype_hijskraantype_naam=containertype_hijskraantype_naam, containertype_hijskraantype_naam_in=containertype_hijskraantype_naam_in, containertype_hijskraantype_naam_isempty=containertype_hijskraantype_naam_isempty, containertype_hijskraantype_naam_isnull=containertype_hijskraantype_naam_isnull, containertype_hijskraantype_naam_like=containertype_hijskraantype_naam_like, containertype_hijskraantype_naam_not=containertype_hijskraantype_naam_not, gewicht_kg=gewicht_kg, gewicht_kg_gt=gewicht_kg_gt, gewicht_kg_gte=gewicht_kg_gte, gewicht_kg_in=gewicht_kg_in, gewicht_kg_isnull=gewicht_kg_isnull, gewicht_kg_lt=gewicht_kg_lt, gewicht_kg_lte=gewicht_kg_lte, gewicht_kg_not=gewicht_kg_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, naam=naam, naam_in=naam_in, naam_isempty=naam_isempty, naam_isnull=naam_isnull, naam_like=naam_like, naam_not=naam_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volume_m3=volume_m3, volume_m3_gt=volume_m3_gt, volume_m3_gte=volume_m3_gte, volume_m3_in=volume_m3_in, volume_m3_isnull=volume_m3_isnull, volume_m3_lt=volume_m3_lt, volume_m3_lte=volume_m3_lte, volume_m3_not=volume_m3_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ContainertypeApi->huishoudelijkafval_containertype_retrieve_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ContainertypeApi->huishoudelijkafval_containertype_retrieve_slash: %s\n" % e)
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
 **containertype_artikelcode** | **str**| Artikelcodevan het het containertype. | [optional] 
 **containertype_artikelcode_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_artikelcode_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_artikelcode_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_artikelcode_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_artikelcode_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containertype_compressie_container_ind** | **bool**| Indicatie voor aanwezigheid van compressie instrument. | [optional] 
 **containertype_compressie_container_ind_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_compressiefactor** | **str**| De compressiefactor van compressie instrument | [optional] 
 **containertype_compressiefactor_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_compressiefactor_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_compressiefactor_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_compressiefactor_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_compressiefactor_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containertype_container_type** | **str**| Het type van de container type | [optional] 
 **containertype_container_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_container_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_container_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_container_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_container_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containertype_hijskraan_opmerking** | **str**| Opmerking over het hijskraantype | [optional] 
 **containertype_hijskraan_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_hijskraan_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_hijskraan_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_hijskraan_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_hijskraan_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containertype_hijskraantype_naam** | **str**| Naam van het type hijskraantype. | [optional] 
 **containertype_hijskraantype_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containertype_hijskraantype_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containertype_hijskraantype_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containertype_hijskraantype_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containertype_hijskraantype_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gewicht_kg** | **int**| Het volume (m3) aan afval wat de container kan bevatten | [optional] 
 **gewicht_kg_gt** | **int**| Greater than; number | [optional] 
 **gewicht_kg_gte** | **int**| Greater than or equal to; number | [optional] 
 **gewicht_kg_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gewicht_kg_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gewicht_kg_lt** | **int**| Less than; number | [optional] 
 **gewicht_kg_lte** | **int**| Less than or equal to; number | [optional] 
 **gewicht_kg_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **id2** | **str**| Unieke aanduiding objecttype | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **naam** | **str**| Naam van het containertype | [optional] 
 **naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **verwijderd_dp** | **bool**| Indicatie of het object verwijderd is bij de bronhouder | [optional] 
 **verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volume_m3** | **float**| Het volume (m3) aan afval wat de container kan bevatten | [optional] 
 **volume_m3_gt** | **float**| Greater than; number | [optional] 
 **volume_m3_gte** | **float**| Greater than or equal to; number | [optional] 
 **volume_m3_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **volume_m3_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volume_m3_lt** | **float**| Less than; number | [optional] 
 **volume_m3_lte** | **float**| Less than or equal to; number | [optional] 
 **volume_m3_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **wijzigingsdatum_dp** | **datetime**| Datum waarop het object is gewijzigd | [optional] 
 **wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**Huishoudelijkafvalcontainertype**](Huishoudelijkafvalcontainertype.md)

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

