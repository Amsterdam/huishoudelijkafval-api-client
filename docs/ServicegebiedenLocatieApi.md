# huishoudelijkafval_api_client.ServicegebiedenLocatieApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_servicegebieden_locatie_list_slash**](ServicegebiedenLocatieApi.md#huishoudelijkafval_servicegebieden_locatie_list_slash) | **GET** /servicegebieden_locatie | 
[**huishoudelijkafval_servicegebieden_locatie_retrieve_slash**](ServicegebiedenLocatieApi.md#huishoudelijkafval_servicegebieden_locatie_retrieve_slash) | **GET** /servicegebieden_locatie/{id} | 


# **huishoudelijkafval_servicegebieden_locatie_list_slash**
> PaginatedHuishoudelijkafvalservicegebiedenLocatieList huishoudelijkafval_servicegebieden_locatie_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aantal_woningen=aantal_woningen, aantal_woningen_gt=aantal_woningen_gt, aantal_woningen_gte=aantal_woningen_gte, aantal_woningen_in=aantal_woningen_in, aantal_woningen_isnull=aantal_woningen_isnull, aantal_woningen_lt=aantal_woningen_lt, aantal_woningen_lte=aantal_woningen_lte, aantal_woningen_not=aantal_woningen_not, cluster_fractie_aantal_containers=cluster_fractie_aantal_containers, cluster_fractie_aantal_containers_gt=cluster_fractie_aantal_containers_gt, cluster_fractie_aantal_containers_gte=cluster_fractie_aantal_containers_gte, cluster_fractie_aantal_containers_in=cluster_fractie_aantal_containers_in, cluster_fractie_aantal_containers_isnull=cluster_fractie_aantal_containers_isnull, cluster_fractie_aantal_containers_lt=cluster_fractie_aantal_containers_lt, cluster_fractie_aantal_containers_lte=cluster_fractie_aantal_containers_lte, cluster_fractie_aantal_containers_not=cluster_fractie_aantal_containers_not, cluster_fractie_code=cluster_fractie_code, cluster_fractie_code_in=cluster_fractie_code_in, cluster_fractie_code_isempty=cluster_fractie_code_isempty, cluster_fractie_code_isnull=cluster_fractie_code_isnull, cluster_fractie_code_like=cluster_fractie_code_like, cluster_fractie_code_not=cluster_fractie_code_not, cluster_fractie_omschrijving=cluster_fractie_omschrijving, cluster_fractie_omschrijving_in=cluster_fractie_omschrijving_in, cluster_fractie_omschrijving_isempty=cluster_fractie_omschrijving_isempty, cluster_fractie_omschrijving_isnull=cluster_fractie_omschrijving_isnull, cluster_fractie_omschrijving_like=cluster_fractie_omschrijving_like, cluster_fractie_omschrijving_not=cluster_fractie_omschrijving_not, cluster_fractie_volume_m3=cluster_fractie_volume_m3, cluster_fractie_volume_m3_gt=cluster_fractie_volume_m3_gt, cluster_fractie_volume_m3_gte=cluster_fractie_volume_m3_gte, cluster_fractie_volume_m3_in=cluster_fractie_volume_m3_in, cluster_fractie_volume_m3_isnull=cluster_fractie_volume_m3_isnull, cluster_fractie_volume_m3_lt=cluster_fractie_volume_m3_lt, cluster_fractie_volume_m3_lte=cluster_fractie_volume_m3_lte, cluster_fractie_volume_m3_not=cluster_fractie_volume_m3_not, gemiddelde_loopafstand=gemiddelde_loopafstand, gemiddelde_loopafstand_gt=gemiddelde_loopafstand_gt, gemiddelde_loopafstand_gte=gemiddelde_loopafstand_gte, gemiddelde_loopafstand_in=gemiddelde_loopafstand_in, gemiddelde_loopafstand_isnull=gemiddelde_loopafstand_isnull, gemiddelde_loopafstand_lt=gemiddelde_loopafstand_lt, gemiddelde_loopafstand_lte=gemiddelde_loopafstand_lte, gemiddelde_loopafstand_not=gemiddelde_loopafstand_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, page=page)

Afvalservicegebied-locatie voor ondergrondse- en bovengrondsecontainers vertegenwoordigt een ophaallocatie voor één type afvalfractie, met een gemiddelde loopafstand naar de nabijgelegen panden. Als er op een ophaallocatie meerdere containers voor dezelfde fractie zijn, worden deze als één enkele fractie beschouwd.

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalservicegebieden_locatie_list import PaginatedHuishoudelijkafvalservicegebiedenLocatieList
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
    api_instance = huishoudelijkafval_api_client.ServicegebiedenLocatieApi(api_client)
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
    aantal_woningen = 3.4 # float | Aantal woningen die gebruik maken van de servicegebiedlocatie (optional)
    aantal_woningen_gt = 3.4 # float | Greater than; number (optional)
    aantal_woningen_gte = 3.4 # float | Greater than or equal to; number (optional)
    aantal_woningen_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_woningen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_woningen_lt = 3.4 # float | Less than; number (optional)
    aantal_woningen_lte = 3.4 # float | Less than or equal to; number (optional)
    aantal_woningen_not = [3.4] # List[float] | Exclude matches; number (optional)
    cluster_fractie_aantal_containers = 3.4 # float | Aantal containers per clusterfractie (optional)
    cluster_fractie_aantal_containers_gt = 3.4 # float | Greater than; number (optional)
    cluster_fractie_aantal_containers_gte = 3.4 # float | Greater than or equal to; number (optional)
    cluster_fractie_aantal_containers_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_fractie_aantal_containers_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_fractie_aantal_containers_lt = 3.4 # float | Less than; number (optional)
    cluster_fractie_aantal_containers_lte = 3.4 # float | Less than or equal to; number (optional)
    cluster_fractie_aantal_containers_not = [3.4] # List[float] | Exclude matches; number (optional)
    cluster_fractie_code = 'cluster_fractie_code_example' # str | Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood (optional)
    cluster_fractie_code_in = ['cluster_fractie_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_fractie_code_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_fractie_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_fractie_code_like = 'cluster_fractie_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_fractie_code_not = ['cluster_fractie_code_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_fractie_omschrijving = 'cluster_fractie_omschrijving_example' # str | Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. (optional)
    cluster_fractie_omschrijving_in = ['cluster_fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_fractie_omschrijving_like = 'cluster_fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_fractie_omschrijving_not = ['cluster_fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_fractie_volume_m3 = 3.4 # float | De som van het volume (m3) van containers per clusterfractie (optional)
    cluster_fractie_volume_m3_gt = 3.4 # float | Greater than; number (optional)
    cluster_fractie_volume_m3_gte = 3.4 # float | Greater than or equal to; number (optional)
    cluster_fractie_volume_m3_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_fractie_volume_m3_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_fractie_volume_m3_lt = 3.4 # float | Less than; number (optional)
    cluster_fractie_volume_m3_lte = 3.4 # float | Less than or equal to; number (optional)
    cluster_fractie_volume_m3_not = [3.4] # List[float] | Exclude matches; number (optional)
    gemiddelde_loopafstand = 3.4 # float | De gemiddelde loopafstand van woningen naar een servicegebiedlocatie. (optional)
    gemiddelde_loopafstand_gt = 3.4 # float | Greater than; number (optional)
    gemiddelde_loopafstand_gte = 3.4 # float | Greater than or equal to; number (optional)
    gemiddelde_loopafstand_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gemiddelde_loopafstand_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gemiddelde_loopafstand_lt = 3.4 # float | Less than; number (optional)
    gemiddelde_loopafstand_lte = 3.4 # float | Less than or equal to; number (optional)
    gemiddelde_loopafstand_not = [3.4] # List[float] | Exclude matches; number (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POLYGON van de servicegebiedlocatie RD (epsg:28992) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id = 'id_example' # str | Unieke identificatie van een afval servicegebied locatie (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    page = 56 # int | A page number within the paginated result set. (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_servicegebieden_locatie_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aantal_woningen=aantal_woningen, aantal_woningen_gt=aantal_woningen_gt, aantal_woningen_gte=aantal_woningen_gte, aantal_woningen_in=aantal_woningen_in, aantal_woningen_isnull=aantal_woningen_isnull, aantal_woningen_lt=aantal_woningen_lt, aantal_woningen_lte=aantal_woningen_lte, aantal_woningen_not=aantal_woningen_not, cluster_fractie_aantal_containers=cluster_fractie_aantal_containers, cluster_fractie_aantal_containers_gt=cluster_fractie_aantal_containers_gt, cluster_fractie_aantal_containers_gte=cluster_fractie_aantal_containers_gte, cluster_fractie_aantal_containers_in=cluster_fractie_aantal_containers_in, cluster_fractie_aantal_containers_isnull=cluster_fractie_aantal_containers_isnull, cluster_fractie_aantal_containers_lt=cluster_fractie_aantal_containers_lt, cluster_fractie_aantal_containers_lte=cluster_fractie_aantal_containers_lte, cluster_fractie_aantal_containers_not=cluster_fractie_aantal_containers_not, cluster_fractie_code=cluster_fractie_code, cluster_fractie_code_in=cluster_fractie_code_in, cluster_fractie_code_isempty=cluster_fractie_code_isempty, cluster_fractie_code_isnull=cluster_fractie_code_isnull, cluster_fractie_code_like=cluster_fractie_code_like, cluster_fractie_code_not=cluster_fractie_code_not, cluster_fractie_omschrijving=cluster_fractie_omschrijving, cluster_fractie_omschrijving_in=cluster_fractie_omschrijving_in, cluster_fractie_omschrijving_isempty=cluster_fractie_omschrijving_isempty, cluster_fractie_omschrijving_isnull=cluster_fractie_omschrijving_isnull, cluster_fractie_omschrijving_like=cluster_fractie_omschrijving_like, cluster_fractie_omschrijving_not=cluster_fractie_omschrijving_not, cluster_fractie_volume_m3=cluster_fractie_volume_m3, cluster_fractie_volume_m3_gt=cluster_fractie_volume_m3_gt, cluster_fractie_volume_m3_gte=cluster_fractie_volume_m3_gte, cluster_fractie_volume_m3_in=cluster_fractie_volume_m3_in, cluster_fractie_volume_m3_isnull=cluster_fractie_volume_m3_isnull, cluster_fractie_volume_m3_lt=cluster_fractie_volume_m3_lt, cluster_fractie_volume_m3_lte=cluster_fractie_volume_m3_lte, cluster_fractie_volume_m3_not=cluster_fractie_volume_m3_not, gemiddelde_loopafstand=gemiddelde_loopafstand, gemiddelde_loopafstand_gt=gemiddelde_loopafstand_gt, gemiddelde_loopafstand_gte=gemiddelde_loopafstand_gte, gemiddelde_loopafstand_in=gemiddelde_loopafstand_in, gemiddelde_loopafstand_isnull=gemiddelde_loopafstand_isnull, gemiddelde_loopafstand_lt=gemiddelde_loopafstand_lt, gemiddelde_loopafstand_lte=gemiddelde_loopafstand_lte, gemiddelde_loopafstand_not=gemiddelde_loopafstand_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, page=page)
        print("The response of ServicegebiedenLocatieApi->huishoudelijkafval_servicegebieden_locatie_list_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicegebiedenLocatieApi->huishoudelijkafval_servicegebieden_locatie_list_slash: %s\n" % e)
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
 **aantal_woningen** | **float**| Aantal woningen die gebruik maken van de servicegebiedlocatie | [optional] 
 **aantal_woningen_gt** | **float**| Greater than; number | [optional] 
 **aantal_woningen_gte** | **float**| Greater than or equal to; number | [optional] 
 **aantal_woningen_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_woningen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_woningen_lt** | **float**| Less than; number | [optional] 
 **aantal_woningen_lte** | **float**| Less than or equal to; number | [optional] 
 **aantal_woningen_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **cluster_fractie_aantal_containers** | **float**| Aantal containers per clusterfractie | [optional] 
 **cluster_fractie_aantal_containers_gt** | **float**| Greater than; number | [optional] 
 **cluster_fractie_aantal_containers_gte** | **float**| Greater than or equal to; number | [optional] 
 **cluster_fractie_aantal_containers_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_fractie_aantal_containers_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_fractie_aantal_containers_lt** | **float**| Less than; number | [optional] 
 **cluster_fractie_aantal_containers_lte** | **float**| Less than or equal to; number | [optional] 
 **cluster_fractie_aantal_containers_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **cluster_fractie_code** | **str**| Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood | [optional] 
 **cluster_fractie_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_fractie_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_fractie_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_fractie_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_fractie_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_fractie_omschrijving** | **str**| Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. | [optional] 
 **cluster_fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_fractie_volume_m3** | **float**| De som van het volume (m3) van containers per clusterfractie | [optional] 
 **cluster_fractie_volume_m3_gt** | **float**| Greater than; number | [optional] 
 **cluster_fractie_volume_m3_gte** | **float**| Greater than or equal to; number | [optional] 
 **cluster_fractie_volume_m3_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_fractie_volume_m3_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_fractie_volume_m3_lt** | **float**| Less than; number | [optional] 
 **cluster_fractie_volume_m3_lte** | **float**| Less than or equal to; number | [optional] 
 **cluster_fractie_volume_m3_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **gemiddelde_loopafstand** | **float**| De gemiddelde loopafstand van woningen naar een servicegebiedlocatie. | [optional] 
 **gemiddelde_loopafstand_gt** | **float**| Greater than; number | [optional] 
 **gemiddelde_loopafstand_gte** | **float**| Greater than or equal to; number | [optional] 
 **gemiddelde_loopafstand_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gemiddelde_loopafstand_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gemiddelde_loopafstand_lt** | **float**| Less than; number | [optional] 
 **gemiddelde_loopafstand_lte** | **float**| Less than or equal to; number | [optional] 
 **gemiddelde_loopafstand_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **geometrie** | **str**| Geometrie van het type POLYGON van de servicegebiedlocatie RD (epsg:28992) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id** | **str**| Unieke identificatie van een afval servicegebied locatie | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalservicegebiedenLocatieList**](PaginatedHuishoudelijkafvalservicegebiedenLocatieList.md)

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

# **huishoudelijkafval_servicegebieden_locatie_retrieve_slash**
> HuishoudelijkafvalservicegebiedenLocatie huishoudelijkafval_servicegebieden_locatie_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aantal_woningen=aantal_woningen, aantal_woningen_gt=aantal_woningen_gt, aantal_woningen_gte=aantal_woningen_gte, aantal_woningen_in=aantal_woningen_in, aantal_woningen_isnull=aantal_woningen_isnull, aantal_woningen_lt=aantal_woningen_lt, aantal_woningen_lte=aantal_woningen_lte, aantal_woningen_not=aantal_woningen_not, cluster_fractie_aantal_containers=cluster_fractie_aantal_containers, cluster_fractie_aantal_containers_gt=cluster_fractie_aantal_containers_gt, cluster_fractie_aantal_containers_gte=cluster_fractie_aantal_containers_gte, cluster_fractie_aantal_containers_in=cluster_fractie_aantal_containers_in, cluster_fractie_aantal_containers_isnull=cluster_fractie_aantal_containers_isnull, cluster_fractie_aantal_containers_lt=cluster_fractie_aantal_containers_lt, cluster_fractie_aantal_containers_lte=cluster_fractie_aantal_containers_lte, cluster_fractie_aantal_containers_not=cluster_fractie_aantal_containers_not, cluster_fractie_code=cluster_fractie_code, cluster_fractie_code_in=cluster_fractie_code_in, cluster_fractie_code_isempty=cluster_fractie_code_isempty, cluster_fractie_code_isnull=cluster_fractie_code_isnull, cluster_fractie_code_like=cluster_fractie_code_like, cluster_fractie_code_not=cluster_fractie_code_not, cluster_fractie_omschrijving=cluster_fractie_omschrijving, cluster_fractie_omschrijving_in=cluster_fractie_omschrijving_in, cluster_fractie_omschrijving_isempty=cluster_fractie_omschrijving_isempty, cluster_fractie_omschrijving_isnull=cluster_fractie_omschrijving_isnull, cluster_fractie_omschrijving_like=cluster_fractie_omschrijving_like, cluster_fractie_omschrijving_not=cluster_fractie_omschrijving_not, cluster_fractie_volume_m3=cluster_fractie_volume_m3, cluster_fractie_volume_m3_gt=cluster_fractie_volume_m3_gt, cluster_fractie_volume_m3_gte=cluster_fractie_volume_m3_gte, cluster_fractie_volume_m3_in=cluster_fractie_volume_m3_in, cluster_fractie_volume_m3_isnull=cluster_fractie_volume_m3_isnull, cluster_fractie_volume_m3_lt=cluster_fractie_volume_m3_lt, cluster_fractie_volume_m3_lte=cluster_fractie_volume_m3_lte, cluster_fractie_volume_m3_not=cluster_fractie_volume_m3_not, gemiddelde_loopafstand=gemiddelde_loopafstand, gemiddelde_loopafstand_gt=gemiddelde_loopafstand_gt, gemiddelde_loopafstand_gte=gemiddelde_loopafstand_gte, gemiddelde_loopafstand_in=gemiddelde_loopafstand_in, gemiddelde_loopafstand_isnull=gemiddelde_loopafstand_isnull, gemiddelde_loopafstand_lt=gemiddelde_loopafstand_lt, gemiddelde_loopafstand_lte=gemiddelde_loopafstand_lte, gemiddelde_loopafstand_not=gemiddelde_loopafstand_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalservicegebieden_locatie import HuishoudelijkafvalservicegebiedenLocatie
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
    api_instance = huishoudelijkafval_api_client.ServicegebiedenLocatieApi(api_client)
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
    aantal_woningen = 3.4 # float | Aantal woningen die gebruik maken van de servicegebiedlocatie (optional)
    aantal_woningen_gt = 3.4 # float | Greater than; number (optional)
    aantal_woningen_gte = 3.4 # float | Greater than or equal to; number (optional)
    aantal_woningen_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_woningen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_woningen_lt = 3.4 # float | Less than; number (optional)
    aantal_woningen_lte = 3.4 # float | Less than or equal to; number (optional)
    aantal_woningen_not = [3.4] # List[float] | Exclude matches; number (optional)
    cluster_fractie_aantal_containers = 3.4 # float | Aantal containers per clusterfractie (optional)
    cluster_fractie_aantal_containers_gt = 3.4 # float | Greater than; number (optional)
    cluster_fractie_aantal_containers_gte = 3.4 # float | Greater than or equal to; number (optional)
    cluster_fractie_aantal_containers_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_fractie_aantal_containers_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_fractie_aantal_containers_lt = 3.4 # float | Less than; number (optional)
    cluster_fractie_aantal_containers_lte = 3.4 # float | Less than or equal to; number (optional)
    cluster_fractie_aantal_containers_not = [3.4] # List[float] | Exclude matches; number (optional)
    cluster_fractie_code = 'cluster_fractie_code_example' # str | Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood (optional)
    cluster_fractie_code_in = ['cluster_fractie_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_fractie_code_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_fractie_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_fractie_code_like = 'cluster_fractie_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_fractie_code_not = ['cluster_fractie_code_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_fractie_omschrijving = 'cluster_fractie_omschrijving_example' # str | Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. (optional)
    cluster_fractie_omschrijving_in = ['cluster_fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_fractie_omschrijving_like = 'cluster_fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_fractie_omschrijving_not = ['cluster_fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_fractie_volume_m3 = 3.4 # float | De som van het volume (m3) van containers per clusterfractie (optional)
    cluster_fractie_volume_m3_gt = 3.4 # float | Greater than; number (optional)
    cluster_fractie_volume_m3_gte = 3.4 # float | Greater than or equal to; number (optional)
    cluster_fractie_volume_m3_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_fractie_volume_m3_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_fractie_volume_m3_lt = 3.4 # float | Less than; number (optional)
    cluster_fractie_volume_m3_lte = 3.4 # float | Less than or equal to; number (optional)
    cluster_fractie_volume_m3_not = [3.4] # List[float] | Exclude matches; number (optional)
    gemiddelde_loopafstand = 3.4 # float | De gemiddelde loopafstand van woningen naar een servicegebiedlocatie. (optional)
    gemiddelde_loopafstand_gt = 3.4 # float | Greater than; number (optional)
    gemiddelde_loopafstand_gte = 3.4 # float | Greater than or equal to; number (optional)
    gemiddelde_loopafstand_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gemiddelde_loopafstand_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gemiddelde_loopafstand_lt = 3.4 # float | Less than; number (optional)
    gemiddelde_loopafstand_lte = 3.4 # float | Less than or equal to; number (optional)
    gemiddelde_loopafstand_not = [3.4] # List[float] | Exclude matches; number (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POLYGON van de servicegebiedlocatie RD (epsg:28992) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id2 = 'id_example' # str | Unieke identificatie van een afval servicegebied locatie (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_servicegebieden_locatie_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aantal_woningen=aantal_woningen, aantal_woningen_gt=aantal_woningen_gt, aantal_woningen_gte=aantal_woningen_gte, aantal_woningen_in=aantal_woningen_in, aantal_woningen_isnull=aantal_woningen_isnull, aantal_woningen_lt=aantal_woningen_lt, aantal_woningen_lte=aantal_woningen_lte, aantal_woningen_not=aantal_woningen_not, cluster_fractie_aantal_containers=cluster_fractie_aantal_containers, cluster_fractie_aantal_containers_gt=cluster_fractie_aantal_containers_gt, cluster_fractie_aantal_containers_gte=cluster_fractie_aantal_containers_gte, cluster_fractie_aantal_containers_in=cluster_fractie_aantal_containers_in, cluster_fractie_aantal_containers_isnull=cluster_fractie_aantal_containers_isnull, cluster_fractie_aantal_containers_lt=cluster_fractie_aantal_containers_lt, cluster_fractie_aantal_containers_lte=cluster_fractie_aantal_containers_lte, cluster_fractie_aantal_containers_not=cluster_fractie_aantal_containers_not, cluster_fractie_code=cluster_fractie_code, cluster_fractie_code_in=cluster_fractie_code_in, cluster_fractie_code_isempty=cluster_fractie_code_isempty, cluster_fractie_code_isnull=cluster_fractie_code_isnull, cluster_fractie_code_like=cluster_fractie_code_like, cluster_fractie_code_not=cluster_fractie_code_not, cluster_fractie_omschrijving=cluster_fractie_omschrijving, cluster_fractie_omschrijving_in=cluster_fractie_omschrijving_in, cluster_fractie_omschrijving_isempty=cluster_fractie_omschrijving_isempty, cluster_fractie_omschrijving_isnull=cluster_fractie_omschrijving_isnull, cluster_fractie_omschrijving_like=cluster_fractie_omschrijving_like, cluster_fractie_omschrijving_not=cluster_fractie_omschrijving_not, cluster_fractie_volume_m3=cluster_fractie_volume_m3, cluster_fractie_volume_m3_gt=cluster_fractie_volume_m3_gt, cluster_fractie_volume_m3_gte=cluster_fractie_volume_m3_gte, cluster_fractie_volume_m3_in=cluster_fractie_volume_m3_in, cluster_fractie_volume_m3_isnull=cluster_fractie_volume_m3_isnull, cluster_fractie_volume_m3_lt=cluster_fractie_volume_m3_lt, cluster_fractie_volume_m3_lte=cluster_fractie_volume_m3_lte, cluster_fractie_volume_m3_not=cluster_fractie_volume_m3_not, gemiddelde_loopafstand=gemiddelde_loopafstand, gemiddelde_loopafstand_gt=gemiddelde_loopafstand_gt, gemiddelde_loopafstand_gte=gemiddelde_loopafstand_gte, gemiddelde_loopafstand_in=gemiddelde_loopafstand_in, gemiddelde_loopafstand_isnull=gemiddelde_loopafstand_isnull, gemiddelde_loopafstand_lt=gemiddelde_loopafstand_lt, gemiddelde_loopafstand_lte=gemiddelde_loopafstand_lte, gemiddelde_loopafstand_not=gemiddelde_loopafstand_not, geometrie=geometrie, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not)
        print("The response of ServicegebiedenLocatieApi->huishoudelijkafval_servicegebieden_locatie_retrieve_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicegebiedenLocatieApi->huishoudelijkafval_servicegebieden_locatie_retrieve_slash: %s\n" % e)
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
 **aantal_woningen** | **float**| Aantal woningen die gebruik maken van de servicegebiedlocatie | [optional] 
 **aantal_woningen_gt** | **float**| Greater than; number | [optional] 
 **aantal_woningen_gte** | **float**| Greater than or equal to; number | [optional] 
 **aantal_woningen_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_woningen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_woningen_lt** | **float**| Less than; number | [optional] 
 **aantal_woningen_lte** | **float**| Less than or equal to; number | [optional] 
 **aantal_woningen_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **cluster_fractie_aantal_containers** | **float**| Aantal containers per clusterfractie | [optional] 
 **cluster_fractie_aantal_containers_gt** | **float**| Greater than; number | [optional] 
 **cluster_fractie_aantal_containers_gte** | **float**| Greater than or equal to; number | [optional] 
 **cluster_fractie_aantal_containers_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_fractie_aantal_containers_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_fractie_aantal_containers_lt** | **float**| Less than; number | [optional] 
 **cluster_fractie_aantal_containers_lte** | **float**| Less than or equal to; number | [optional] 
 **cluster_fractie_aantal_containers_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **cluster_fractie_code** | **str**| Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood | [optional] 
 **cluster_fractie_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_fractie_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_fractie_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_fractie_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_fractie_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_fractie_omschrijving** | **str**| Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. | [optional] 
 **cluster_fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_fractie_volume_m3** | **float**| De som van het volume (m3) van containers per clusterfractie | [optional] 
 **cluster_fractie_volume_m3_gt** | **float**| Greater than; number | [optional] 
 **cluster_fractie_volume_m3_gte** | **float**| Greater than or equal to; number | [optional] 
 **cluster_fractie_volume_m3_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_fractie_volume_m3_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_fractie_volume_m3_lt** | **float**| Less than; number | [optional] 
 **cluster_fractie_volume_m3_lte** | **float**| Less than or equal to; number | [optional] 
 **cluster_fractie_volume_m3_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **gemiddelde_loopafstand** | **float**| De gemiddelde loopafstand van woningen naar een servicegebiedlocatie. | [optional] 
 **gemiddelde_loopafstand_gt** | **float**| Greater than; number | [optional] 
 **gemiddelde_loopafstand_gte** | **float**| Greater than or equal to; number | [optional] 
 **gemiddelde_loopafstand_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gemiddelde_loopafstand_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gemiddelde_loopafstand_lt** | **float**| Less than; number | [optional] 
 **gemiddelde_loopafstand_lte** | **float**| Less than or equal to; number | [optional] 
 **gemiddelde_loopafstand_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **geometrie** | **str**| Geometrie van het type POLYGON van de servicegebiedlocatie RD (epsg:28992) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id2** | **str**| Unieke identificatie van een afval servicegebied locatie | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 

### Return type

[**HuishoudelijkafvalservicegebiedenLocatie**](HuishoudelijkafvalservicegebiedenLocatie.md)

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

