# huishoudelijkafval_api_client.LoopafstandCategorieV2Api

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_loopafstand_categorie_v2_list2**](LoopafstandCategorieV2Api.md#huishoudelijkafval_loopafstand_categorie_v2_list2) | **GET** /loopafstand_categorie_v2 | 
[**huishoudelijkafval_loopafstand_categorie_v2_retrieve2**](LoopafstandCategorieV2Api.md#huishoudelijkafval_loopafstand_categorie_v2_retrieve2) | **GET** /loopafstand_categorie_v2/{id} | 


# **huishoudelijkafval_loopafstand_categorie_v2_list2**
> PaginatedHuishoudelijkafvalloopafstandCategorieV2List huishoudelijkafval_loopafstand_categorie_v2_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, fractie=fractie, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, fractie_in=fractie_in, fractie_isempty=fractie_isempty, fractie_isnull=fractie_isnull, fractie_like=fractie_like, fractie_not=fractie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand_categorie_omschrijving=loopafstand_categorie_omschrijving, loopafstand_categorie_omschrijving_in=loopafstand_categorie_omschrijving_in, loopafstand_categorie_omschrijving_isempty=loopafstand_categorie_omschrijving_isempty, loopafstand_categorie_omschrijving_isnull=loopafstand_categorie_omschrijving_isnull, loopafstand_categorie_omschrijving_like=loopafstand_categorie_omschrijving_like, loopafstand_categorie_omschrijving_not=loopafstand_categorie_omschrijving_not, loopafstand_categorie_tot=loopafstand_categorie_tot, loopafstand_categorie_tot_gt=loopafstand_categorie_tot_gt, loopafstand_categorie_tot_gte=loopafstand_categorie_tot_gte, loopafstand_categorie_tot_in=loopafstand_categorie_tot_in, loopafstand_categorie_tot_isnull=loopafstand_categorie_tot_isnull, loopafstand_categorie_tot_lt=loopafstand_categorie_tot_lt, loopafstand_categorie_tot_lte=loopafstand_categorie_tot_lte, loopafstand_categorie_tot_not=loopafstand_categorie_tot_not, loopafstand_categorie_vanaf=loopafstand_categorie_vanaf, loopafstand_categorie_vanaf_gt=loopafstand_categorie_vanaf_gt, loopafstand_categorie_vanaf_gte=loopafstand_categorie_vanaf_gte, loopafstand_categorie_vanaf_in=loopafstand_categorie_vanaf_in, loopafstand_categorie_vanaf_isnull=loopafstand_categorie_vanaf_isnull, loopafstand_categorie_vanaf_lt=loopafstand_categorie_vanaf_lt, loopafstand_categorie_vanaf_lte=loopafstand_categorie_vanaf_lte, loopafstand_categorie_vanaf_not=loopafstand_categorie_vanaf_not, page=page, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalloopafstand_categorie_v2_list import PaginatedHuishoudelijkafvalloopafstandCategorieV2List
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
    api_instance = huishoudelijkafval_api_client.LoopafstandCategorieV2Api(api_client)
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
    fractie = 'fractie_example' # str | Code afvalfractie waarnaar de afstand is bepaald (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Omschrijving afvalfractie waarnaar de afstand is bepaald (optional)
    fractie_omschrijving_in = ['fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_omschrijving_like = 'fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_omschrijving_not = ['fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    fractie_in = ['fractie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_like = 'fractie_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_not = ['fractie_not_example'] # List[str] | Exclude matches; text (optional)
    id = 'id_example' # str | identificatie categorie loopafstand (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_omschrijving = 'loopafstand_categorie_omschrijving_example' # str | Omschrijving van de categorie waarin de berekende loopafstand valt (optional)
    loopafstand_categorie_omschrijving_in = ['loopafstand_categorie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    loopafstand_categorie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_omschrijving_like = 'loopafstand_categorie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    loopafstand_categorie_omschrijving_not = ['loopafstand_categorie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_tot = 56 # int | Bovengrens van de categorie waarin de berekende loopafstand valt (optional)
    loopafstand_categorie_tot_gt = 56 # int | Greater than; number (optional)
    loopafstand_categorie_tot_gte = 56 # int | Greater than or equal to; number (optional)
    loopafstand_categorie_tot_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_tot_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_tot_lt = 56 # int | Less than; number (optional)
    loopafstand_categorie_tot_lte = 56 # int | Less than or equal to; number (optional)
    loopafstand_categorie_tot_not = [56] # List[int] | Exclude matches; number (optional)
    loopafstand_categorie_vanaf = 56 # int | Ondergrens van de categorie waarin de berekende loopafstand valt (optional)
    loopafstand_categorie_vanaf_gt = 56 # int | Greater than; number (optional)
    loopafstand_categorie_vanaf_gte = 56 # int | Greater than or equal to; number (optional)
    loopafstand_categorie_vanaf_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_vanaf_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_vanaf_lt = 56 # int | Less than; number (optional)
    loopafstand_categorie_vanaf_lte = 56 # int | Less than or equal to; number (optional)
    loopafstand_categorie_vanaf_not = [56] # List[int] | Exclude matches; number (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    verwijderd_dp = True # bool | Indicatie of het object verwijderd is in de datapijplijn (optional)
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
        api_response = await api_instance.huishoudelijkafval_loopafstand_categorie_v2_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, fractie=fractie, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, fractie_in=fractie_in, fractie_isempty=fractie_isempty, fractie_isnull=fractie_isnull, fractie_like=fractie_like, fractie_not=fractie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand_categorie_omschrijving=loopafstand_categorie_omschrijving, loopafstand_categorie_omschrijving_in=loopafstand_categorie_omschrijving_in, loopafstand_categorie_omschrijving_isempty=loopafstand_categorie_omschrijving_isempty, loopafstand_categorie_omschrijving_isnull=loopafstand_categorie_omschrijving_isnull, loopafstand_categorie_omschrijving_like=loopafstand_categorie_omschrijving_like, loopafstand_categorie_omschrijving_not=loopafstand_categorie_omschrijving_not, loopafstand_categorie_tot=loopafstand_categorie_tot, loopafstand_categorie_tot_gt=loopafstand_categorie_tot_gt, loopafstand_categorie_tot_gte=loopafstand_categorie_tot_gte, loopafstand_categorie_tot_in=loopafstand_categorie_tot_in, loopafstand_categorie_tot_isnull=loopafstand_categorie_tot_isnull, loopafstand_categorie_tot_lt=loopafstand_categorie_tot_lt, loopafstand_categorie_tot_lte=loopafstand_categorie_tot_lte, loopafstand_categorie_tot_not=loopafstand_categorie_tot_not, loopafstand_categorie_vanaf=loopafstand_categorie_vanaf, loopafstand_categorie_vanaf_gt=loopafstand_categorie_vanaf_gt, loopafstand_categorie_vanaf_gte=loopafstand_categorie_vanaf_gte, loopafstand_categorie_vanaf_in=loopafstand_categorie_vanaf_in, loopafstand_categorie_vanaf_isnull=loopafstand_categorie_vanaf_isnull, loopafstand_categorie_vanaf_lt=loopafstand_categorie_vanaf_lt, loopafstand_categorie_vanaf_lte=loopafstand_categorie_vanaf_lte, loopafstand_categorie_vanaf_not=loopafstand_categorie_vanaf_not, page=page, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of LoopafstandCategorieV2Api->huishoudelijkafval_loopafstand_categorie_v2_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LoopafstandCategorieV2Api->huishoudelijkafval_loopafstand_categorie_v2_list2: %s\n" % e)
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
 **fractie** | **str**| Code afvalfractie waarnaar de afstand is bepaald | [optional] 
 **fractie_omschrijving** | **str**| Omschrijving afvalfractie waarnaar de afstand is bepaald | [optional] 
 **fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **fractie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id** | **str**| identificatie categorie loopafstand | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_omschrijving** | **str**| Omschrijving van de categorie waarin de berekende loopafstand valt | [optional] 
 **loopafstand_categorie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **loopafstand_categorie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **loopafstand_categorie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_tot** | **int**| Bovengrens van de categorie waarin de berekende loopafstand valt | [optional] 
 **loopafstand_categorie_tot_gt** | **int**| Greater than; number | [optional] 
 **loopafstand_categorie_tot_gte** | **int**| Greater than or equal to; number | [optional] 
 **loopafstand_categorie_tot_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_tot_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_tot_lt** | **int**| Less than; number | [optional] 
 **loopafstand_categorie_tot_lte** | **int**| Less than or equal to; number | [optional] 
 **loopafstand_categorie_tot_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **loopafstand_categorie_vanaf** | **int**| Ondergrens van de categorie waarin de berekende loopafstand valt | [optional] 
 **loopafstand_categorie_vanaf_gt** | **int**| Greater than; number | [optional] 
 **loopafstand_categorie_vanaf_gte** | **int**| Greater than or equal to; number | [optional] 
 **loopafstand_categorie_vanaf_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_vanaf_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_vanaf_lt** | **int**| Less than; number | [optional] 
 **loopafstand_categorie_vanaf_lte** | **int**| Less than or equal to; number | [optional] 
 **loopafstand_categorie_vanaf_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **verwijderd_dp** | **bool**| Indicatie of het object verwijderd is in de datapijplijn | [optional] 
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

[**PaginatedHuishoudelijkafvalloopafstandCategorieV2List**](PaginatedHuishoudelijkafvalloopafstandCategorieV2List.md)

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

# **huishoudelijkafval_loopafstand_categorie_v2_retrieve2**
> HuishoudelijkafvalloopafstandCategorieV2 huishoudelijkafval_loopafstand_categorie_v2_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, fractie=fractie, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, fractie_in=fractie_in, fractie_isempty=fractie_isempty, fractie_isnull=fractie_isnull, fractie_like=fractie_like, fractie_not=fractie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand_categorie_omschrijving=loopafstand_categorie_omschrijving, loopafstand_categorie_omschrijving_in=loopafstand_categorie_omschrijving_in, loopafstand_categorie_omschrijving_isempty=loopafstand_categorie_omschrijving_isempty, loopafstand_categorie_omschrijving_isnull=loopafstand_categorie_omschrijving_isnull, loopafstand_categorie_omschrijving_like=loopafstand_categorie_omschrijving_like, loopafstand_categorie_omschrijving_not=loopafstand_categorie_omschrijving_not, loopafstand_categorie_tot=loopafstand_categorie_tot, loopafstand_categorie_tot_gt=loopafstand_categorie_tot_gt, loopafstand_categorie_tot_gte=loopafstand_categorie_tot_gte, loopafstand_categorie_tot_in=loopafstand_categorie_tot_in, loopafstand_categorie_tot_isnull=loopafstand_categorie_tot_isnull, loopafstand_categorie_tot_lt=loopafstand_categorie_tot_lt, loopafstand_categorie_tot_lte=loopafstand_categorie_tot_lte, loopafstand_categorie_tot_not=loopafstand_categorie_tot_not, loopafstand_categorie_vanaf=loopafstand_categorie_vanaf, loopafstand_categorie_vanaf_gt=loopafstand_categorie_vanaf_gt, loopafstand_categorie_vanaf_gte=loopafstand_categorie_vanaf_gte, loopafstand_categorie_vanaf_in=loopafstand_categorie_vanaf_in, loopafstand_categorie_vanaf_isnull=loopafstand_categorie_vanaf_isnull, loopafstand_categorie_vanaf_lt=loopafstand_categorie_vanaf_lt, loopafstand_categorie_vanaf_lte=loopafstand_categorie_vanaf_lte, loopafstand_categorie_vanaf_not=loopafstand_categorie_vanaf_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalloopafstand_categorie_v2 import HuishoudelijkafvalloopafstandCategorieV2
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
    api_instance = huishoudelijkafval_api_client.LoopafstandCategorieV2Api(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'expand_scope_example' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    fractie = 'fractie_example' # str | Code afvalfractie waarnaar de afstand is bepaald (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Omschrijving afvalfractie waarnaar de afstand is bepaald (optional)
    fractie_omschrijving_in = ['fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_omschrijving_like = 'fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_omschrijving_not = ['fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    fractie_in = ['fractie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_like = 'fractie_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_not = ['fractie_not_example'] # List[str] | Exclude matches; text (optional)
    id2 = 'id_example' # str | identificatie categorie loopafstand (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_omschrijving = 'loopafstand_categorie_omschrijving_example' # str | Omschrijving van de categorie waarin de berekende loopafstand valt (optional)
    loopafstand_categorie_omschrijving_in = ['loopafstand_categorie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    loopafstand_categorie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_omschrijving_like = 'loopafstand_categorie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    loopafstand_categorie_omschrijving_not = ['loopafstand_categorie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_tot = 56 # int | Bovengrens van de categorie waarin de berekende loopafstand valt (optional)
    loopafstand_categorie_tot_gt = 56 # int | Greater than; number (optional)
    loopafstand_categorie_tot_gte = 56 # int | Greater than or equal to; number (optional)
    loopafstand_categorie_tot_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_tot_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_tot_lt = 56 # int | Less than; number (optional)
    loopafstand_categorie_tot_lte = 56 # int | Less than or equal to; number (optional)
    loopafstand_categorie_tot_not = [56] # List[int] | Exclude matches; number (optional)
    loopafstand_categorie_vanaf = 56 # int | Ondergrens van de categorie waarin de berekende loopafstand valt (optional)
    loopafstand_categorie_vanaf_gt = 56 # int | Greater than; number (optional)
    loopafstand_categorie_vanaf_gte = 56 # int | Greater than or equal to; number (optional)
    loopafstand_categorie_vanaf_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_vanaf_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_vanaf_lt = 56 # int | Less than; number (optional)
    loopafstand_categorie_vanaf_lte = 56 # int | Less than or equal to; number (optional)
    loopafstand_categorie_vanaf_not = [56] # List[int] | Exclude matches; number (optional)
    verwijderd_dp = True # bool | Indicatie of het object verwijderd is in de datapijplijn (optional)
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
        api_response = await api_instance.huishoudelijkafval_loopafstand_categorie_v2_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, fractie=fractie, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, fractie_in=fractie_in, fractie_isempty=fractie_isempty, fractie_isnull=fractie_isnull, fractie_like=fractie_like, fractie_not=fractie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand_categorie_omschrijving=loopafstand_categorie_omschrijving, loopafstand_categorie_omschrijving_in=loopafstand_categorie_omschrijving_in, loopafstand_categorie_omschrijving_isempty=loopafstand_categorie_omschrijving_isempty, loopafstand_categorie_omschrijving_isnull=loopafstand_categorie_omschrijving_isnull, loopafstand_categorie_omschrijving_like=loopafstand_categorie_omschrijving_like, loopafstand_categorie_omschrijving_not=loopafstand_categorie_omschrijving_not, loopafstand_categorie_tot=loopafstand_categorie_tot, loopafstand_categorie_tot_gt=loopafstand_categorie_tot_gt, loopafstand_categorie_tot_gte=loopafstand_categorie_tot_gte, loopafstand_categorie_tot_in=loopafstand_categorie_tot_in, loopafstand_categorie_tot_isnull=loopafstand_categorie_tot_isnull, loopafstand_categorie_tot_lt=loopafstand_categorie_tot_lt, loopafstand_categorie_tot_lte=loopafstand_categorie_tot_lte, loopafstand_categorie_tot_not=loopafstand_categorie_tot_not, loopafstand_categorie_vanaf=loopafstand_categorie_vanaf, loopafstand_categorie_vanaf_gt=loopafstand_categorie_vanaf_gt, loopafstand_categorie_vanaf_gte=loopafstand_categorie_vanaf_gte, loopafstand_categorie_vanaf_in=loopafstand_categorie_vanaf_in, loopafstand_categorie_vanaf_isnull=loopafstand_categorie_vanaf_isnull, loopafstand_categorie_vanaf_lt=loopafstand_categorie_vanaf_lt, loopafstand_categorie_vanaf_lte=loopafstand_categorie_vanaf_lte, loopafstand_categorie_vanaf_not=loopafstand_categorie_vanaf_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of LoopafstandCategorieV2Api->huishoudelijkafval_loopafstand_categorie_v2_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling LoopafstandCategorieV2Api->huishoudelijkafval_loopafstand_categorie_v2_retrieve2: %s\n" % e)
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
 **fractie** | **str**| Code afvalfractie waarnaar de afstand is bepaald | [optional] 
 **fractie_omschrijving** | **str**| Omschrijving afvalfractie waarnaar de afstand is bepaald | [optional] 
 **fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **fractie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id2** | **str**| identificatie categorie loopafstand | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_omschrijving** | **str**| Omschrijving van de categorie waarin de berekende loopafstand valt | [optional] 
 **loopafstand_categorie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **loopafstand_categorie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **loopafstand_categorie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_tot** | **int**| Bovengrens van de categorie waarin de berekende loopafstand valt | [optional] 
 **loopafstand_categorie_tot_gt** | **int**| Greater than; number | [optional] 
 **loopafstand_categorie_tot_gte** | **int**| Greater than or equal to; number | [optional] 
 **loopafstand_categorie_tot_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_tot_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_tot_lt** | **int**| Less than; number | [optional] 
 **loopafstand_categorie_tot_lte** | **int**| Less than or equal to; number | [optional] 
 **loopafstand_categorie_tot_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **loopafstand_categorie_vanaf** | **int**| Ondergrens van de categorie waarin de berekende loopafstand valt | [optional] 
 **loopafstand_categorie_vanaf_gt** | **int**| Greater than; number | [optional] 
 **loopafstand_categorie_vanaf_gte** | **int**| Greater than or equal to; number | [optional] 
 **loopafstand_categorie_vanaf_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_vanaf_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_vanaf_lt** | **int**| Less than; number | [optional] 
 **loopafstand_categorie_vanaf_lte** | **int**| Less than or equal to; number | [optional] 
 **loopafstand_categorie_vanaf_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **verwijderd_dp** | **bool**| Indicatie of het object verwijderd is in de datapijplijn | [optional] 
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

[**HuishoudelijkafvalloopafstandCategorieV2**](HuishoudelijkafvalloopafstandCategorieV2.md)

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

