# huishoudelijkafval_api_client.ClusterfractieApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_clusterfractie_list2**](ClusterfractieApi.md#huishoudelijkafval_clusterfractie_list2) | **GET** /clusterfractie | 
[**huishoudelijkafval_clusterfractie_retrieve2**](ClusterfractieApi.md#huishoudelijkafval_clusterfractie_retrieve2) | **GET** /clusterfractie/{id} | 


# **huishoudelijkafval_clusterfractie_list2**
> PaginatedHuishoudelijkafvalclusterfractieList huishoudelijkafval_clusterfractie_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aantal_containers=aantal_containers, aantal_containers_gt=aantal_containers_gt, aantal_containers_gte=aantal_containers_gte, aantal_containers_in=aantal_containers_in, aantal_containers_isnull=aantal_containers_isnull, aantal_containers_lt=aantal_containers_lt, aantal_containers_lte=aantal_containers_lte, aantal_containers_not=aantal_containers_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, code=code, code_in=code_in, code_isempty=code_isempty, code_isnull=code_isnull, code_like=code_like, code_not=code_not, datum_einde=datum_einde, datum_einde_gt=datum_einde_gt, datum_einde_gte=datum_einde_gte, datum_einde_in=datum_einde_in, datum_einde_isnull=datum_einde_isnull, datum_einde_lt=datum_einde_lt, datum_einde_lte=datum_einde_lte, datum_einde_not=datum_einde_not, datum_opvoer=datum_opvoer, datum_opvoer_gt=datum_opvoer_gt, datum_opvoer_gte=datum_opvoer_gte, datum_opvoer_in=datum_opvoer_in, datum_opvoer_isnull=datum_opvoer_isnull, datum_opvoer_lt=datum_opvoer_lt, datum_opvoer_lte=datum_opvoer_lte, datum_opvoer_not=datum_opvoer_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, omschrijving=omschrijving, omschrijving_in=omschrijving_in, omschrijving_isempty=omschrijving_isempty, omschrijving_isnull=omschrijving_isnull, omschrijving_like=omschrijving_like, omschrijving_not=omschrijving_not, page=page, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volume_m3=volume_m3, volume_m3_gt=volume_m3_gt, volume_m3_gte=volume_m3_gte, volume_m3_in=volume_m3_in, volume_m3_isnull=volume_m3_isnull, volume_m3_lt=volume_m3_lt, volume_m3_lte=volume_m3_lte, volume_m3_not=volume_m3_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalclusterfractie_list import PaginatedHuishoudelijkafvalclusterfractieList
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
    api_instance = huishoudelijkafval_api_client.ClusterfractieApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'expand_scope_example' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    aantal_containers = 56 # int | Aantal containers per clusterfractie (optional)
    aantal_containers_gt = 56 # int | Greater than; number (optional)
    aantal_containers_gte = 56 # int | Greater than or equal to; number (optional)
    aantal_containers_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_containers_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_containers_lt = 56 # int | Less than; number (optional)
    aantal_containers_lte = 56 # int | Less than or equal to; number (optional)
    aantal_containers_not = [56] # List[int] | Exclude matches; number (optional)
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
    code = 'code_example' # str | Code afvalfractie zoals door Welvaarts is aanleverd. 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 7 - Grof, 8 - PMD, 9 - Brood, -999 - Onbekend (optional)
    code_in = ['code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    code_isempty = True # bool | Whether the field is empty or not. (optional)
    code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    code_like = 'code_like_example' # str | Matches text using wildcards (? and *). (optional)
    code_not = ['code_not_example'] # List[str] | Exclude matches; text (optional)
    datum_einde = '2013-10-20' # date | De datum waarop de cluster in het systeem is eindigd. (optional)
    datum_einde_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_einde_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_einde_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_einde_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_einde_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_einde_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_einde_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_opvoer = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de cluster in het systeem is opgevoerd. (optional)
    datum_opvoer_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_opvoer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_opvoer_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    id = 'id_example' # str | Uniek identificerend kenmerk van clusterfractie (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    omschrijving = 'omschrijving_example' # str | Afvalfractie zoals door Welvaarts is aangeleverd (optional)
    omschrijving_in = ['omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    omschrijving_like = 'omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    omschrijving_not = ['omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    verwijderd_dp = True # bool | indicatie of het object verwijderd is bij de bronhouder (optional)
    verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volume_m3 = 3.4 # float | De som van het volume (m3) van containers per clusterfractie (optional)
    volume_m3_gt = 3.4 # float | Greater than; number (optional)
    volume_m3_gte = 3.4 # float | Greater than or equal to; number (optional)
    volume_m3_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    volume_m3_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volume_m3_lt = 3.4 # float | Less than; number (optional)
    volume_m3_lte = 3.4 # float | Less than or equal to; number (optional)
    volume_m3_not = [3.4] # List[float] | Exclude matches; number (optional)
    wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de cluster in het systeem is gewijzigd. (optional)
    wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_clusterfractie_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aantal_containers=aantal_containers, aantal_containers_gt=aantal_containers_gt, aantal_containers_gte=aantal_containers_gte, aantal_containers_in=aantal_containers_in, aantal_containers_isnull=aantal_containers_isnull, aantal_containers_lt=aantal_containers_lt, aantal_containers_lte=aantal_containers_lte, aantal_containers_not=aantal_containers_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, code=code, code_in=code_in, code_isempty=code_isempty, code_isnull=code_isnull, code_like=code_like, code_not=code_not, datum_einde=datum_einde, datum_einde_gt=datum_einde_gt, datum_einde_gte=datum_einde_gte, datum_einde_in=datum_einde_in, datum_einde_isnull=datum_einde_isnull, datum_einde_lt=datum_einde_lt, datum_einde_lte=datum_einde_lte, datum_einde_not=datum_einde_not, datum_opvoer=datum_opvoer, datum_opvoer_gt=datum_opvoer_gt, datum_opvoer_gte=datum_opvoer_gte, datum_opvoer_in=datum_opvoer_in, datum_opvoer_isnull=datum_opvoer_isnull, datum_opvoer_lt=datum_opvoer_lt, datum_opvoer_lte=datum_opvoer_lte, datum_opvoer_not=datum_opvoer_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, omschrijving=omschrijving, omschrijving_in=omschrijving_in, omschrijving_isempty=omschrijving_isempty, omschrijving_isnull=omschrijving_isnull, omschrijving_like=omschrijving_like, omschrijving_not=omschrijving_not, page=page, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volume_m3=volume_m3, volume_m3_gt=volume_m3_gt, volume_m3_gte=volume_m3_gte, volume_m3_in=volume_m3_in, volume_m3_isnull=volume_m3_isnull, volume_m3_lt=volume_m3_lt, volume_m3_lte=volume_m3_lte, volume_m3_not=volume_m3_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ClusterfractieApi->huishoudelijkafval_clusterfractie_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClusterfractieApi->huishoudelijkafval_clusterfractie_list2: %s\n" % e)
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
 **aantal_containers** | **int**| Aantal containers per clusterfractie | [optional] 
 **aantal_containers_gt** | **int**| Greater than; number | [optional] 
 **aantal_containers_gte** | **int**| Greater than or equal to; number | [optional] 
 **aantal_containers_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_containers_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_containers_lt** | **int**| Less than; number | [optional] 
 **aantal_containers_lte** | **int**| Less than or equal to; number | [optional] 
 **aantal_containers_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **code** | **str**| Code afvalfractie zoals door Welvaarts is aanleverd. 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 7 - Grof, 8 - PMD, 9 - Brood, -999 - Onbekend | [optional] 
 **code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_einde** | **date**| De datum waarop de cluster in het systeem is eindigd. | [optional] 
 **datum_einde_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_einde_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_einde_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_einde_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_einde_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_einde_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_einde_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_opvoer** | **datetime**| De datum waarop de cluster in het systeem is opgevoerd. | [optional] 
 **datum_opvoer_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_opvoer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_opvoer_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **id** | **str**| Uniek identificerend kenmerk van clusterfractie | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **omschrijving** | **str**| Afvalfractie zoals door Welvaarts is aangeleverd | [optional] 
 **omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **verwijderd_dp** | **bool**| indicatie of het object verwijderd is bij de bronhouder | [optional] 
 **verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volume_m3** | **float**| De som van het volume (m3) van containers per clusterfractie | [optional] 
 **volume_m3_gt** | **float**| Greater than; number | [optional] 
 **volume_m3_gte** | **float**| Greater than or equal to; number | [optional] 
 **volume_m3_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **volume_m3_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volume_m3_lt** | **float**| Less than; number | [optional] 
 **volume_m3_lte** | **float**| Less than or equal to; number | [optional] 
 **volume_m3_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **wijzigingsdatum_dp** | **datetime**| De datum waarop de cluster in het systeem is gewijzigd. | [optional] 
 **wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalclusterfractieList**](PaginatedHuishoudelijkafvalclusterfractieList.md)

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

# **huishoudelijkafval_clusterfractie_retrieve2**
> Huishoudelijkafvalclusterfractie huishoudelijkafval_clusterfractie_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aantal_containers=aantal_containers, aantal_containers_gt=aantal_containers_gt, aantal_containers_gte=aantal_containers_gte, aantal_containers_in=aantal_containers_in, aantal_containers_isnull=aantal_containers_isnull, aantal_containers_lt=aantal_containers_lt, aantal_containers_lte=aantal_containers_lte, aantal_containers_not=aantal_containers_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, code=code, code_in=code_in, code_isempty=code_isempty, code_isnull=code_isnull, code_like=code_like, code_not=code_not, datum_einde=datum_einde, datum_einde_gt=datum_einde_gt, datum_einde_gte=datum_einde_gte, datum_einde_in=datum_einde_in, datum_einde_isnull=datum_einde_isnull, datum_einde_lt=datum_einde_lt, datum_einde_lte=datum_einde_lte, datum_einde_not=datum_einde_not, datum_opvoer=datum_opvoer, datum_opvoer_gt=datum_opvoer_gt, datum_opvoer_gte=datum_opvoer_gte, datum_opvoer_in=datum_opvoer_in, datum_opvoer_isnull=datum_opvoer_isnull, datum_opvoer_lt=datum_opvoer_lt, datum_opvoer_lte=datum_opvoer_lte, datum_opvoer_not=datum_opvoer_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, omschrijving=omschrijving, omschrijving_in=omschrijving_in, omschrijving_isempty=omschrijving_isempty, omschrijving_isnull=omschrijving_isnull, omschrijving_like=omschrijving_like, omschrijving_not=omschrijving_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volume_m3=volume_m3, volume_m3_gt=volume_m3_gt, volume_m3_gte=volume_m3_gte, volume_m3_in=volume_m3_in, volume_m3_isnull=volume_m3_isnull, volume_m3_lt=volume_m3_lt, volume_m3_lte=volume_m3_lte, volume_m3_not=volume_m3_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalclusterfractie import Huishoudelijkafvalclusterfractie
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
    api_instance = huishoudelijkafval_api_client.ClusterfractieApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'expand_scope_example' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    aantal_containers = 56 # int | Aantal containers per clusterfractie (optional)
    aantal_containers_gt = 56 # int | Greater than; number (optional)
    aantal_containers_gte = 56 # int | Greater than or equal to; number (optional)
    aantal_containers_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_containers_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_containers_lt = 56 # int | Less than; number (optional)
    aantal_containers_lte = 56 # int | Less than or equal to; number (optional)
    aantal_containers_not = [56] # List[int] | Exclude matches; number (optional)
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
    code = 'code_example' # str | Code afvalfractie zoals door Welvaarts is aanleverd. 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 7 - Grof, 8 - PMD, 9 - Brood, -999 - Onbekend (optional)
    code_in = ['code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    code_isempty = True # bool | Whether the field is empty or not. (optional)
    code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    code_like = 'code_like_example' # str | Matches text using wildcards (? and *). (optional)
    code_not = ['code_not_example'] # List[str] | Exclude matches; text (optional)
    datum_einde = '2013-10-20' # date | De datum waarop de cluster in het systeem is eindigd. (optional)
    datum_einde_gt = '2013-10-20' # date | Greater than; use yyyy-mm-dd (optional)
    datum_einde_gte = '2013-10-20' # date | Greater than or equal to; use yyyy-mm-dd (optional)
    datum_einde_in = ['2013-10-20'] # List[date] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_einde_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_einde_lt = '2013-10-20' # date | Less than; use yyyy-mm-dd (optional)
    datum_einde_lte = '2013-10-20' # date | Less than or equal to; use yyyy-mm-dd (optional)
    datum_einde_not = ['2013-10-20'] # List[date] | Exclude matches; use yyyy-mm-dd (optional)
    datum_opvoer = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de cluster in het systeem is opgevoerd. (optional)
    datum_opvoer_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_opvoer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_opvoer_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_opvoer_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    id2 = 'id_example' # str | Uniek identificerend kenmerk van clusterfractie (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    omschrijving = 'omschrijving_example' # str | Afvalfractie zoals door Welvaarts is aangeleverd (optional)
    omschrijving_in = ['omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    omschrijving_like = 'omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    omschrijving_not = ['omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    verwijderd_dp = True # bool | indicatie of het object verwijderd is bij de bronhouder (optional)
    verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volume_m3 = 3.4 # float | De som van het volume (m3) van containers per clusterfractie (optional)
    volume_m3_gt = 3.4 # float | Greater than; number (optional)
    volume_m3_gte = 3.4 # float | Greater than or equal to; number (optional)
    volume_m3_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    volume_m3_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    volume_m3_lt = 3.4 # float | Less than; number (optional)
    volume_m3_lte = 3.4 # float | Less than or equal to; number (optional)
    volume_m3_not = [3.4] # List[float] | Exclude matches; number (optional)
    wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de cluster in het systeem is gewijzigd. (optional)
    wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_clusterfractie_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aantal_containers=aantal_containers, aantal_containers_gt=aantal_containers_gt, aantal_containers_gte=aantal_containers_gte, aantal_containers_in=aantal_containers_in, aantal_containers_isnull=aantal_containers_isnull, aantal_containers_lt=aantal_containers_lt, aantal_containers_lte=aantal_containers_lte, aantal_containers_not=aantal_containers_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, code=code, code_in=code_in, code_isempty=code_isempty, code_isnull=code_isnull, code_like=code_like, code_not=code_not, datum_einde=datum_einde, datum_einde_gt=datum_einde_gt, datum_einde_gte=datum_einde_gte, datum_einde_in=datum_einde_in, datum_einde_isnull=datum_einde_isnull, datum_einde_lt=datum_einde_lt, datum_einde_lte=datum_einde_lte, datum_einde_not=datum_einde_not, datum_opvoer=datum_opvoer, datum_opvoer_gt=datum_opvoer_gt, datum_opvoer_gte=datum_opvoer_gte, datum_opvoer_in=datum_opvoer_in, datum_opvoer_isnull=datum_opvoer_isnull, datum_opvoer_lt=datum_opvoer_lt, datum_opvoer_lte=datum_opvoer_lte, datum_opvoer_not=datum_opvoer_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, omschrijving=omschrijving, omschrijving_in=omschrijving_in, omschrijving_isempty=omschrijving_isempty, omschrijving_isnull=omschrijving_isnull, omschrijving_like=omschrijving_like, omschrijving_not=omschrijving_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, volume_m3=volume_m3, volume_m3_gt=volume_m3_gt, volume_m3_gte=volume_m3_gte, volume_m3_in=volume_m3_in, volume_m3_isnull=volume_m3_isnull, volume_m3_lt=volume_m3_lt, volume_m3_lte=volume_m3_lte, volume_m3_not=volume_m3_not, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of ClusterfractieApi->huishoudelijkafval_clusterfractie_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ClusterfractieApi->huishoudelijkafval_clusterfractie_retrieve2: %s\n" % e)
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
 **aantal_containers** | **int**| Aantal containers per clusterfractie | [optional] 
 **aantal_containers_gt** | **int**| Greater than; number | [optional] 
 **aantal_containers_gte** | **int**| Greater than or equal to; number | [optional] 
 **aantal_containers_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_containers_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_containers_lt** | **int**| Less than; number | [optional] 
 **aantal_containers_lte** | **int**| Less than or equal to; number | [optional] 
 **aantal_containers_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster waaraan de container is gerelateerd | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **code** | **str**| Code afvalfractie zoals door Welvaarts is aanleverd. 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 7 - Grof, 8 - PMD, 9 - Brood, -999 - Onbekend | [optional] 
 **code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_einde** | **date**| De datum waarop de cluster in het systeem is eindigd. | [optional] 
 **datum_einde_gt** | **date**| Greater than; use yyyy-mm-dd | [optional] 
 **datum_einde_gte** | **date**| Greater than or equal to; use yyyy-mm-dd | [optional] 
 **datum_einde_in** | [**List[date]**](date.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_einde_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_einde_lt** | **date**| Less than; use yyyy-mm-dd | [optional] 
 **datum_einde_lte** | **date**| Less than or equal to; use yyyy-mm-dd | [optional] 
 **datum_einde_not** | [**List[date]**](date.md)| Exclude matches; use yyyy-mm-dd | [optional] 
 **datum_opvoer** | **datetime**| De datum waarop de cluster in het systeem is opgevoerd. | [optional] 
 **datum_opvoer_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_opvoer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_opvoer_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_opvoer_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **id2** | **str**| Uniek identificerend kenmerk van clusterfractie | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **omschrijving** | **str**| Afvalfractie zoals door Welvaarts is aangeleverd | [optional] 
 **omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **verwijderd_dp** | **bool**| indicatie of het object verwijderd is bij de bronhouder | [optional] 
 **verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volume_m3** | **float**| De som van het volume (m3) van containers per clusterfractie | [optional] 
 **volume_m3_gt** | **float**| Greater than; number | [optional] 
 **volume_m3_gte** | **float**| Greater than or equal to; number | [optional] 
 **volume_m3_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **volume_m3_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **volume_m3_lt** | **float**| Less than; number | [optional] 
 **volume_m3_lte** | **float**| Less than or equal to; number | [optional] 
 **volume_m3_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **wijzigingsdatum_dp** | **datetime**| De datum waarop de cluster in het systeem is gewijzigd. | [optional] 
 **wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**Huishoudelijkafvalclusterfractie**](Huishoudelijkafvalclusterfractie.md)

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

