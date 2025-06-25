# huishoudelijkafval_api_client.BagObjectLoopafstandV2Api

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_bag_object_loopafstand_v2_list2**](BagObjectLoopafstandV2Api.md#huishoudelijkafval_bag_object_loopafstand_v2_list2) | **GET** /bag_object_loopafstand_v2 | 
[**huishoudelijkafval_bag_object_loopafstand_v2_retrieve2**](BagObjectLoopafstandV2Api.md#huishoudelijkafval_bag_object_loopafstand_v2_retrieve2) | **GET** /bag_object_loopafstand_v2/{id} | 


# **huishoudelijkafval_bag_object_loopafstand_v2_list2**
> PaginatedHuishoudelijkafvalbagObjectLoopafstandV2List huishoudelijkafval_bag_object_loopafstand_v2_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_object_id=bag_object_id, bag_object_id_in=bag_object_id_in, bag_object_id_isempty=bag_object_id_isempty, bag_object_id_isnull=bag_object_id_isnull, bag_object_id_like=bag_object_id_like, bag_object_id_not=bag_object_id_not, bag_object_type=bag_object_type, bag_object_type_in=bag_object_type_in, bag_object_type_isempty=bag_object_type_isempty, bag_object_type_isnull=bag_object_type_isnull, bag_object_type_like=bag_object_type_like, bag_object_type_not=bag_object_type_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, fractie=fractie, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, fractie_in=fractie_in, fractie_isempty=fractie_isempty, fractie_isnull=fractie_isnull, fractie_like=fractie_like, fractie_not=fractie_not, geometrie=geometrie, geometrie_contains=geometrie_contains, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand=loopafstand, loopafstand_categorie_id=loopafstand_categorie_id, loopafstand_categorie_id_in=loopafstand_categorie_id_in, loopafstand_categorie_id_isempty=loopafstand_categorie_id_isempty, loopafstand_categorie_id_isnull=loopafstand_categorie_id_isnull, loopafstand_categorie_id_like=loopafstand_categorie_id_like, loopafstand_categorie_id_not=loopafstand_categorie_id_not, loopafstand_gt=loopafstand_gt, loopafstand_gte=loopafstand_gte, loopafstand_in=loopafstand_in, loopafstand_isnull=loopafstand_isnull, loopafstand_lt=loopafstand_lt, loopafstand_lte=loopafstand_lte, loopafstand_not=loopafstand_not, page=page, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalbag_object_loopafstand_v2_list import PaginatedHuishoudelijkafvalbagObjectLoopafstandV2List
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
    api_instance = huishoudelijkafval_api_client.BagObjectLoopafstandV2Api(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'cluster' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    bag_object_id = 'bag_object_id_example' # str | Uniek identificerend kenmerk van bagobject (optional)
    bag_object_id_in = ['bag_object_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_object_id_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_object_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_object_id_like = 'bag_object_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_object_id_not = ['bag_object_id_not_example'] # List[str] | Exclude matches; text (optional)
    bag_object_type = 'bag_object_type_example' # str | Typering adresseerbaar object conform BAG: verblijfsobject, ligplaats , standplaats (optional)
    bag_object_type_in = ['bag_object_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_object_type_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_object_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_object_type_like = 'bag_object_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_object_type_not = ['bag_object_type_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
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
    geometrie = 'geometrie_example' # str | Geometrie van het type MULTIPOLYGON in RD (epsg:28992)) (optional)
    geometrie_contains = 'geometrie_contains_example' # str | Use x,y or POINT(x y) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id = 'id_example' # str | Uniek identificerend kenmerk van het record (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand = 3.4 # float | Berekende afstand over de weg in meter  van woning tot cluster van containers van de betreffende afvalfractie (optional)
    loopafstand_categorie_id = 'loopafstand_categorie_id_example' # str | identificatie categorie loopafstand (optional)
    loopafstand_categorie_id_in = ['loopafstand_categorie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    loopafstand_categorie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_id_like = 'loopafstand_categorie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    loopafstand_categorie_id_not = ['loopafstand_categorie_id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_gt = 3.4 # float | Greater than; number (optional)
    loopafstand_gte = 3.4 # float | Greater than or equal to; number (optional)
    loopafstand_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_lt = 3.4 # float | Less than; number (optional)
    loopafstand_lte = 3.4 # float | Less than or equal to; number (optional)
    loopafstand_not = [3.4] # List[float] | Exclude matches; number (optional)
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
        api_response = await api_instance.huishoudelijkafval_bag_object_loopafstand_v2_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_object_id=bag_object_id, bag_object_id_in=bag_object_id_in, bag_object_id_isempty=bag_object_id_isempty, bag_object_id_isnull=bag_object_id_isnull, bag_object_id_like=bag_object_id_like, bag_object_id_not=bag_object_id_not, bag_object_type=bag_object_type, bag_object_type_in=bag_object_type_in, bag_object_type_isempty=bag_object_type_isempty, bag_object_type_isnull=bag_object_type_isnull, bag_object_type_like=bag_object_type_like, bag_object_type_not=bag_object_type_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, fractie=fractie, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, fractie_in=fractie_in, fractie_isempty=fractie_isempty, fractie_isnull=fractie_isnull, fractie_like=fractie_like, fractie_not=fractie_not, geometrie=geometrie, geometrie_contains=geometrie_contains, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand=loopafstand, loopafstand_categorie_id=loopafstand_categorie_id, loopafstand_categorie_id_in=loopafstand_categorie_id_in, loopafstand_categorie_id_isempty=loopafstand_categorie_id_isempty, loopafstand_categorie_id_isnull=loopafstand_categorie_id_isnull, loopafstand_categorie_id_like=loopafstand_categorie_id_like, loopafstand_categorie_id_not=loopafstand_categorie_id_not, loopafstand_gt=loopafstand_gt, loopafstand_gte=loopafstand_gte, loopafstand_in=loopafstand_in, loopafstand_isnull=loopafstand_isnull, loopafstand_lt=loopafstand_lt, loopafstand_lte=loopafstand_lte, loopafstand_not=loopafstand_not, page=page, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of BagObjectLoopafstandV2Api->huishoudelijkafval_bag_object_loopafstand_v2_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BagObjectLoopafstandV2Api->huishoudelijkafval_bag_object_loopafstand_v2_list2: %s\n" % e)
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
 **bag_object_id** | **str**| Uniek identificerend kenmerk van bagobject | [optional] 
 **bag_object_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_object_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_object_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_object_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_object_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_object_type** | **str**| Typering adresseerbaar object conform BAG: verblijfsobject, ligplaats , standplaats | [optional] 
 **bag_object_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_object_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_object_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_object_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_object_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
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
 **geometrie** | **str**| Geometrie van het type MULTIPOLYGON in RD (epsg:28992)) | [optional] 
 **geometrie_contains** | **str**| Use x,y or POINT(x y) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id** | **str**| Uniek identificerend kenmerk van het record | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand** | **float**| Berekende afstand over de weg in meter  van woning tot cluster van containers van de betreffende afvalfractie | [optional] 
 **loopafstand_categorie_id** | **str**| identificatie categorie loopafstand | [optional] 
 **loopafstand_categorie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **loopafstand_categorie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **loopafstand_categorie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_gt** | **float**| Greater than; number | [optional] 
 **loopafstand_gte** | **float**| Greater than or equal to; number | [optional] 
 **loopafstand_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_lt** | **float**| Less than; number | [optional] 
 **loopafstand_lte** | **float**| Less than or equal to; number | [optional] 
 **loopafstand_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
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

[**PaginatedHuishoudelijkafvalbagObjectLoopafstandV2List**](PaginatedHuishoudelijkafvalbagObjectLoopafstandV2List.md)

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

# **huishoudelijkafval_bag_object_loopafstand_v2_retrieve2**
> HuishoudelijkafvalbagObjectLoopafstandV2 huishoudelijkafval_bag_object_loopafstand_v2_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_object_id=bag_object_id, bag_object_id_in=bag_object_id_in, bag_object_id_isempty=bag_object_id_isempty, bag_object_id_isnull=bag_object_id_isnull, bag_object_id_like=bag_object_id_like, bag_object_id_not=bag_object_id_not, bag_object_type=bag_object_type, bag_object_type_in=bag_object_type_in, bag_object_type_isempty=bag_object_type_isempty, bag_object_type_isnull=bag_object_type_isnull, bag_object_type_like=bag_object_type_like, bag_object_type_not=bag_object_type_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, fractie=fractie, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, fractie_in=fractie_in, fractie_isempty=fractie_isempty, fractie_isnull=fractie_isnull, fractie_like=fractie_like, fractie_not=fractie_not, geometrie=geometrie, geometrie_contains=geometrie_contains, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand=loopafstand, loopafstand_categorie_id=loopafstand_categorie_id, loopafstand_categorie_id_in=loopafstand_categorie_id_in, loopafstand_categorie_id_isempty=loopafstand_categorie_id_isempty, loopafstand_categorie_id_isnull=loopafstand_categorie_id_isnull, loopafstand_categorie_id_like=loopafstand_categorie_id_like, loopafstand_categorie_id_not=loopafstand_categorie_id_not, loopafstand_gt=loopafstand_gt, loopafstand_gte=loopafstand_gte, loopafstand_in=loopafstand_in, loopafstand_isnull=loopafstand_isnull, loopafstand_lt=loopafstand_lt, loopafstand_lte=loopafstand_lte, loopafstand_not=loopafstand_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalbag_object_loopafstand_v2 import HuishoudelijkafvalbagObjectLoopafstandV2
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
    api_instance = huishoudelijkafval_api_client.BagObjectLoopafstandV2Api(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'cluster' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    bag_object_id = 'bag_object_id_example' # str | Uniek identificerend kenmerk van bagobject (optional)
    bag_object_id_in = ['bag_object_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_object_id_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_object_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_object_id_like = 'bag_object_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_object_id_not = ['bag_object_id_not_example'] # List[str] | Exclude matches; text (optional)
    bag_object_type = 'bag_object_type_example' # str | Typering adresseerbaar object conform BAG: verblijfsobject, ligplaats , standplaats (optional)
    bag_object_type_in = ['bag_object_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_object_type_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_object_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_object_type_like = 'bag_object_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_object_type_not = ['bag_object_type_not_example'] # List[str] | Exclude matches; text (optional)
    cluster_id = 'cluster_id_example' # str | Uniek identificerend kenmerk van cluster (optional)
    cluster_id_in = ['cluster_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    cluster_id_isempty = True # bool | Whether the field is empty or not. (optional)
    cluster_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    cluster_id_like = 'cluster_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    cluster_id_not = ['cluster_id_not_example'] # List[str] | Exclude matches; text (optional)
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
    geometrie = 'geometrie_example' # str | Geometrie van het type MULTIPOLYGON in RD (epsg:28992)) (optional)
    geometrie_contains = 'geometrie_contains_example' # str | Use x,y or POINT(x y) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id2 = 'id_example' # str | Uniek identificerend kenmerk van het record (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand = 3.4 # float | Berekende afstand over de weg in meter  van woning tot cluster van containers van de betreffende afvalfractie (optional)
    loopafstand_categorie_id = 'loopafstand_categorie_id_example' # str | identificatie categorie loopafstand (optional)
    loopafstand_categorie_id_in = ['loopafstand_categorie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    loopafstand_categorie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_id_like = 'loopafstand_categorie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    loopafstand_categorie_id_not = ['loopafstand_categorie_id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_gt = 3.4 # float | Greater than; number (optional)
    loopafstand_gte = 3.4 # float | Greater than or equal to; number (optional)
    loopafstand_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_lt = 3.4 # float | Less than; number (optional)
    loopafstand_lte = 3.4 # float | Less than or equal to; number (optional)
    loopafstand_not = [3.4] # List[float] | Exclude matches; number (optional)
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
        api_response = await api_instance.huishoudelijkafval_bag_object_loopafstand_v2_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_object_id=bag_object_id, bag_object_id_in=bag_object_id_in, bag_object_id_isempty=bag_object_id_isempty, bag_object_id_isnull=bag_object_id_isnull, bag_object_id_like=bag_object_id_like, bag_object_id_not=bag_object_id_not, bag_object_type=bag_object_type, bag_object_type_in=bag_object_type_in, bag_object_type_isempty=bag_object_type_isempty, bag_object_type_isnull=bag_object_type_isnull, bag_object_type_like=bag_object_type_like, bag_object_type_not=bag_object_type_not, cluster_id=cluster_id, cluster_id_in=cluster_id_in, cluster_id_isempty=cluster_id_isempty, cluster_id_isnull=cluster_id_isnull, cluster_id_like=cluster_id_like, cluster_id_not=cluster_id_not, fractie=fractie, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, fractie_in=fractie_in, fractie_isempty=fractie_isempty, fractie_isnull=fractie_isnull, fractie_like=fractie_like, fractie_not=fractie_not, geometrie=geometrie, geometrie_contains=geometrie_contains, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand=loopafstand, loopafstand_categorie_id=loopafstand_categorie_id, loopafstand_categorie_id_in=loopafstand_categorie_id_in, loopafstand_categorie_id_isempty=loopafstand_categorie_id_isempty, loopafstand_categorie_id_isnull=loopafstand_categorie_id_isnull, loopafstand_categorie_id_like=loopafstand_categorie_id_like, loopafstand_categorie_id_not=loopafstand_categorie_id_not, loopafstand_gt=loopafstand_gt, loopafstand_gte=loopafstand_gte, loopafstand_in=loopafstand_in, loopafstand_isnull=loopafstand_isnull, loopafstand_lt=loopafstand_lt, loopafstand_lte=loopafstand_lte, loopafstand_not=loopafstand_not, verwijderd_dp=verwijderd_dp, verwijderd_dp_isnull=verwijderd_dp_isnull, wijzigingsdatum_dp=wijzigingsdatum_dp, wijzigingsdatum_dp_gt=wijzigingsdatum_dp_gt, wijzigingsdatum_dp_gte=wijzigingsdatum_dp_gte, wijzigingsdatum_dp_in=wijzigingsdatum_dp_in, wijzigingsdatum_dp_isnull=wijzigingsdatum_dp_isnull, wijzigingsdatum_dp_lt=wijzigingsdatum_dp_lt, wijzigingsdatum_dp_lte=wijzigingsdatum_dp_lte, wijzigingsdatum_dp_not=wijzigingsdatum_dp_not)
        print("The response of BagObjectLoopafstandV2Api->huishoudelijkafval_bag_object_loopafstand_v2_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BagObjectLoopafstandV2Api->huishoudelijkafval_bag_object_loopafstand_v2_retrieve2: %s\n" % e)
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
 **bag_object_id** | **str**| Uniek identificerend kenmerk van bagobject | [optional] 
 **bag_object_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_object_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_object_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_object_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_object_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_object_type** | **str**| Typering adresseerbaar object conform BAG: verblijfsobject, ligplaats , standplaats | [optional] 
 **bag_object_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_object_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_object_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_object_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_object_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **cluster_id** | **str**| Uniek identificerend kenmerk van cluster | [optional] 
 **cluster_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **cluster_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **cluster_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **cluster_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **cluster_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
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
 **geometrie** | **str**| Geometrie van het type MULTIPOLYGON in RD (epsg:28992)) | [optional] 
 **geometrie_contains** | **str**| Use x,y or POINT(x y) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id2** | **str**| Uniek identificerend kenmerk van het record | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand** | **float**| Berekende afstand over de weg in meter  van woning tot cluster van containers van de betreffende afvalfractie | [optional] 
 **loopafstand_categorie_id** | **str**| identificatie categorie loopafstand | [optional] 
 **loopafstand_categorie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **loopafstand_categorie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **loopafstand_categorie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_gt** | **float**| Greater than; number | [optional] 
 **loopafstand_gte** | **float**| Greater than or equal to; number | [optional] 
 **loopafstand_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_lt** | **float**| Less than; number | [optional] 
 **loopafstand_lte** | **float**| Less than or equal to; number | [optional] 
 **loopafstand_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
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

[**HuishoudelijkafvalbagObjectLoopafstandV2**](HuishoudelijkafvalbagObjectLoopafstandV2.md)

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

