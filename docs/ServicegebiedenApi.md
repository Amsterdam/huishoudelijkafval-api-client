# huishoudelijkafval_api_client.ServicegebiedenApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_servicegebieden_list_slash**](ServicegebiedenApi.md#huishoudelijkafval_servicegebieden_list_slash) | **GET** /servicegebieden | 
[**huishoudelijkafval_servicegebieden_retrieve_slash**](ServicegebiedenApi.md#huishoudelijkafval_servicegebieden_retrieve_slash) | **GET** /servicegebieden/{id} | 


# **huishoudelijkafval_servicegebieden_list_slash**
> PaginatedHuishoudelijkafvalservicegebiedenList huishoudelijkafval_servicegebieden_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_object_id=bag_object_id, bag_object_id_in=bag_object_id_in, bag_object_id_isempty=bag_object_id_isempty, bag_object_id_isnull=bag_object_id_isnull, bag_object_id_like=bag_object_id_like, bag_object_id_not=bag_object_id_not, bag_object_type=bag_object_type, bag_object_type_in=bag_object_type_in, bag_object_type_isempty=bag_object_type_isempty, bag_object_type_isnull=bag_object_type_isnull, bag_object_type_like=bag_object_type_like, bag_object_type_not=bag_object_type_not, categorie_verwijderd_dp=categorie_verwijderd_dp, categorie_verwijderd_dp_isnull=categorie_verwijderd_dp_isnull, categorie_wijzigingsdatum_dp=categorie_wijzigingsdatum_dp, categorie_wijzigingsdatum_dp_gt=categorie_wijzigingsdatum_dp_gt, categorie_wijzigingsdatum_dp_gte=categorie_wijzigingsdatum_dp_gte, categorie_wijzigingsdatum_dp_in=categorie_wijzigingsdatum_dp_in, categorie_wijzigingsdatum_dp_isnull=categorie_wijzigingsdatum_dp_isnull, categorie_wijzigingsdatum_dp_lt=categorie_wijzigingsdatum_dp_lt, categorie_wijzigingsdatum_dp_lte=categorie_wijzigingsdatum_dp_lte, categorie_wijzigingsdatum_dp_not=categorie_wijzigingsdatum_dp_not, fractie_code=fractie_code, fractie_code_in=fractie_code_in, fractie_code_isempty=fractie_code_isempty, fractie_code_isnull=fractie_code_isnull, fractie_code_like=fractie_code_like, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, geometrie=geometrie, geometrie_contains=geometrie_contains, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand_categorie_id=loopafstand_categorie_id, loopafstand_categorie_id_in=loopafstand_categorie_id_in, loopafstand_categorie_id_isempty=loopafstand_categorie_id_isempty, loopafstand_categorie_id_isnull=loopafstand_categorie_id_isnull, loopafstand_categorie_id_like=loopafstand_categorie_id_like, loopafstand_categorie_id_not=loopafstand_categorie_id_not, loopafstand_categorie_omschrijving=loopafstand_categorie_omschrijving, loopafstand_categorie_omschrijving_in=loopafstand_categorie_omschrijving_in, loopafstand_categorie_omschrijving_isempty=loopafstand_categorie_omschrijving_isempty, loopafstand_categorie_omschrijving_isnull=loopafstand_categorie_omschrijving_isnull, loopafstand_categorie_omschrijving_like=loopafstand_categorie_omschrijving_like, loopafstand_categorie_omschrijving_not=loopafstand_categorie_omschrijving_not, loopafstand_categorie_tot=loopafstand_categorie_tot, loopafstand_categorie_tot_gt=loopafstand_categorie_tot_gt, loopafstand_categorie_tot_gte=loopafstand_categorie_tot_gte, loopafstand_categorie_tot_in=loopafstand_categorie_tot_in, loopafstand_categorie_tot_isnull=loopafstand_categorie_tot_isnull, loopafstand_categorie_tot_lt=loopafstand_categorie_tot_lt, loopafstand_categorie_tot_lte=loopafstand_categorie_tot_lte, loopafstand_categorie_tot_not=loopafstand_categorie_tot_not, loopafstand_categorie_vanaf=loopafstand_categorie_vanaf, loopafstand_categorie_vanaf_gt=loopafstand_categorie_vanaf_gt, loopafstand_categorie_vanaf_gte=loopafstand_categorie_vanaf_gte, loopafstand_categorie_vanaf_in=loopafstand_categorie_vanaf_in, loopafstand_categorie_vanaf_isnull=loopafstand_categorie_vanaf_isnull, loopafstand_categorie_vanaf_lt=loopafstand_categorie_vanaf_lt, loopafstand_categorie_vanaf_lte=loopafstand_categorie_vanaf_lte, loopafstand_categorie_vanaf_not=loopafstand_categorie_vanaf_not, page=page, servicegebieden_locatie_id=servicegebieden_locatie_id, servicegebieden_locatie_id_in=servicegebieden_locatie_id_in, servicegebieden_locatie_id_isempty=servicegebieden_locatie_id_isempty, servicegebieden_locatie_id_isnull=servicegebieden_locatie_id_isnull, servicegebieden_locatie_id_like=servicegebieden_locatie_id_like, servicegebieden_locatie_id_not=servicegebieden_locatie_id_not)

Een afvalservicegebied is een verzameling van panden die dicht bij elkaar liggen op basis van hun loopafstand tot een afvalophaal locatie. De bewoners van deze panden maken gebruik van het dichtstbijzijnde afvalservicepunt.

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalservicegebieden_list import PaginatedHuishoudelijkafvalservicegebiedenList
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
    api_instance = huishoudelijkafval_api_client.ServicegebiedenApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'servicegebiedenLocatie' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    bag_object_id = 'bag_object_id_example' # str | Unieke BAG object (pand, ligplaats en standplaats) identificatie (optional)
    bag_object_id_in = ['bag_object_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_object_id_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_object_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_object_id_like = 'bag_object_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_object_id_not = ['bag_object_id_not_example'] # List[str] | Exclude matches; text (optional)
    bag_object_type = 'bag_object_type_example' # str | Type BAG object (pand, ligplaats en standplaats) (optional)
    bag_object_type_in = ['bag_object_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_object_type_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_object_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_object_type_like = 'bag_object_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_object_type_not = ['bag_object_type_not_example'] # List[str] | Exclude matches; text (optional)
    categorie_verwijderd_dp = True # bool | De datum waarop de loopafstandcategorie in de datapijplijn is verwijderd. (optional)
    categorie_verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    categorie_wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de loopafstandcategorie in de datapijplijn is gewijzigd (optional)
    categorie_wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    categorie_wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    categorie_wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    categorie_wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    categorie_wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    categorie_wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    categorie_wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    fractie_code = 'fractie_code_example' # str | Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood (optional)
    fractie_code_in = ['fractie_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_code_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_code_like = 'fractie_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_code_not = ['fractie_code_not_example'] # List[str] | Exclude matches; text (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. (optional)
    fractie_omschrijving_in = ['fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_omschrijving_like = 'fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_omschrijving_not = ['fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de container RD (epsg:28992) (optional)
    geometrie_contains = 'geometrie_contains_example' # str | Use x,y or POINT(x y) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id = 'id_example' # str | Unieke identificatie van een afval servicegebied (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_id = 'loopafstand_categorie_id_example' # str | Unieke identificatie van loopafstanden categoriën (optional)
    loopafstand_categorie_id_in = ['loopafstand_categorie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    loopafstand_categorie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_id_like = 'loopafstand_categorie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    loopafstand_categorie_id_not = ['loopafstand_categorie_id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_omschrijving = 'loopafstand_categorie_omschrijving_example' # str | De loopafstanden zijn volgens een vastgestelde indelijng gecategoriseerd. Bijvoorbeeld: 30 - 90 meter (optional)
    loopafstand_categorie_omschrijving_in = ['loopafstand_categorie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    loopafstand_categorie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_omschrijving_like = 'loopafstand_categorie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    loopafstand_categorie_omschrijving_not = ['loopafstand_categorie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_tot = 3.4 # float | De loopafstand tot een bepaalde meter volgens de loopafstandcategorisatie. (optional)
    loopafstand_categorie_tot_gt = 3.4 # float | Greater than; number (optional)
    loopafstand_categorie_tot_gte = 3.4 # float | Greater than or equal to; number (optional)
    loopafstand_categorie_tot_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_tot_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_tot_lt = 3.4 # float | Less than; number (optional)
    loopafstand_categorie_tot_lte = 3.4 # float | Less than or equal to; number (optional)
    loopafstand_categorie_tot_not = [3.4] # List[float] | Exclude matches; number (optional)
    loopafstand_categorie_vanaf = 3.4 # float | De loopafstand vanaf een bepaalde meter. Volgens de loopafstand categorisatie. (optional)
    loopafstand_categorie_vanaf_gt = 3.4 # float | Greater than; number (optional)
    loopafstand_categorie_vanaf_gte = 3.4 # float | Greater than or equal to; number (optional)
    loopafstand_categorie_vanaf_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_vanaf_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_vanaf_lt = 3.4 # float | Less than; number (optional)
    loopafstand_categorie_vanaf_lte = 3.4 # float | Less than or equal to; number (optional)
    loopafstand_categorie_vanaf_not = [3.4] # List[float] | Exclude matches; number (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    servicegebieden_locatie_id = 'servicegebieden_locatie_id_example' # str | Unieke identificatie van een afval servicegebied locatie (optional)
    servicegebieden_locatie_id_in = ['servicegebieden_locatie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    servicegebieden_locatie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    servicegebieden_locatie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    servicegebieden_locatie_id_like = 'servicegebieden_locatie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    servicegebieden_locatie_id_not = ['servicegebieden_locatie_id_not_example'] # List[str] | Exclude matches; text (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_servicegebieden_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, bag_object_id=bag_object_id, bag_object_id_in=bag_object_id_in, bag_object_id_isempty=bag_object_id_isempty, bag_object_id_isnull=bag_object_id_isnull, bag_object_id_like=bag_object_id_like, bag_object_id_not=bag_object_id_not, bag_object_type=bag_object_type, bag_object_type_in=bag_object_type_in, bag_object_type_isempty=bag_object_type_isempty, bag_object_type_isnull=bag_object_type_isnull, bag_object_type_like=bag_object_type_like, bag_object_type_not=bag_object_type_not, categorie_verwijderd_dp=categorie_verwijderd_dp, categorie_verwijderd_dp_isnull=categorie_verwijderd_dp_isnull, categorie_wijzigingsdatum_dp=categorie_wijzigingsdatum_dp, categorie_wijzigingsdatum_dp_gt=categorie_wijzigingsdatum_dp_gt, categorie_wijzigingsdatum_dp_gte=categorie_wijzigingsdatum_dp_gte, categorie_wijzigingsdatum_dp_in=categorie_wijzigingsdatum_dp_in, categorie_wijzigingsdatum_dp_isnull=categorie_wijzigingsdatum_dp_isnull, categorie_wijzigingsdatum_dp_lt=categorie_wijzigingsdatum_dp_lt, categorie_wijzigingsdatum_dp_lte=categorie_wijzigingsdatum_dp_lte, categorie_wijzigingsdatum_dp_not=categorie_wijzigingsdatum_dp_not, fractie_code=fractie_code, fractie_code_in=fractie_code_in, fractie_code_isempty=fractie_code_isempty, fractie_code_isnull=fractie_code_isnull, fractie_code_like=fractie_code_like, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, geometrie=geometrie, geometrie_contains=geometrie_contains, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id=id, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand_categorie_id=loopafstand_categorie_id, loopafstand_categorie_id_in=loopafstand_categorie_id_in, loopafstand_categorie_id_isempty=loopafstand_categorie_id_isempty, loopafstand_categorie_id_isnull=loopafstand_categorie_id_isnull, loopafstand_categorie_id_like=loopafstand_categorie_id_like, loopafstand_categorie_id_not=loopafstand_categorie_id_not, loopafstand_categorie_omschrijving=loopafstand_categorie_omschrijving, loopafstand_categorie_omschrijving_in=loopafstand_categorie_omschrijving_in, loopafstand_categorie_omschrijving_isempty=loopafstand_categorie_omschrijving_isempty, loopafstand_categorie_omschrijving_isnull=loopafstand_categorie_omschrijving_isnull, loopafstand_categorie_omschrijving_like=loopafstand_categorie_omschrijving_like, loopafstand_categorie_omschrijving_not=loopafstand_categorie_omschrijving_not, loopafstand_categorie_tot=loopafstand_categorie_tot, loopafstand_categorie_tot_gt=loopafstand_categorie_tot_gt, loopafstand_categorie_tot_gte=loopafstand_categorie_tot_gte, loopafstand_categorie_tot_in=loopafstand_categorie_tot_in, loopafstand_categorie_tot_isnull=loopafstand_categorie_tot_isnull, loopafstand_categorie_tot_lt=loopafstand_categorie_tot_lt, loopafstand_categorie_tot_lte=loopafstand_categorie_tot_lte, loopafstand_categorie_tot_not=loopafstand_categorie_tot_not, loopafstand_categorie_vanaf=loopafstand_categorie_vanaf, loopafstand_categorie_vanaf_gt=loopafstand_categorie_vanaf_gt, loopafstand_categorie_vanaf_gte=loopafstand_categorie_vanaf_gte, loopafstand_categorie_vanaf_in=loopafstand_categorie_vanaf_in, loopafstand_categorie_vanaf_isnull=loopafstand_categorie_vanaf_isnull, loopafstand_categorie_vanaf_lt=loopafstand_categorie_vanaf_lt, loopafstand_categorie_vanaf_lte=loopafstand_categorie_vanaf_lte, loopafstand_categorie_vanaf_not=loopafstand_categorie_vanaf_not, page=page, servicegebieden_locatie_id=servicegebieden_locatie_id, servicegebieden_locatie_id_in=servicegebieden_locatie_id_in, servicegebieden_locatie_id_isempty=servicegebieden_locatie_id_isempty, servicegebieden_locatie_id_isnull=servicegebieden_locatie_id_isnull, servicegebieden_locatie_id_like=servicegebieden_locatie_id_like, servicegebieden_locatie_id_not=servicegebieden_locatie_id_not)
        print("The response of ServicegebiedenApi->huishoudelijkafval_servicegebieden_list_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicegebiedenApi->huishoudelijkafval_servicegebieden_list_slash: %s\n" % e)
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
 **bag_object_id** | **str**| Unieke BAG object (pand, ligplaats en standplaats) identificatie | [optional] 
 **bag_object_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_object_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_object_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_object_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_object_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_object_type** | **str**| Type BAG object (pand, ligplaats en standplaats) | [optional] 
 **bag_object_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_object_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_object_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_object_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_object_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **categorie_verwijderd_dp** | **bool**| De datum waarop de loopafstandcategorie in de datapijplijn is verwijderd. | [optional] 
 **categorie_verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **categorie_wijzigingsdatum_dp** | **datetime**| De datum waarop de loopafstandcategorie in de datapijplijn is gewijzigd | [optional] 
 **categorie_wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **categorie_wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **categorie_wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **categorie_wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **categorie_wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **categorie_wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **categorie_wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **fractie_code** | **str**| Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood | [optional] 
 **fractie_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **fractie_omschrijving** | **str**| Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. | [optional] 
 **fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de container RD (epsg:28992) | [optional] 
 **geometrie_contains** | **str**| Use x,y or POINT(x y) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id** | **str**| Unieke identificatie van een afval servicegebied | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_id** | **str**| Unieke identificatie van loopafstanden categoriën | [optional] 
 **loopafstand_categorie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **loopafstand_categorie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **loopafstand_categorie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_omschrijving** | **str**| De loopafstanden zijn volgens een vastgestelde indelijng gecategoriseerd. Bijvoorbeeld: 30 - 90 meter | [optional] 
 **loopafstand_categorie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **loopafstand_categorie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **loopafstand_categorie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_tot** | **float**| De loopafstand tot een bepaalde meter volgens de loopafstandcategorisatie. | [optional] 
 **loopafstand_categorie_tot_gt** | **float**| Greater than; number | [optional] 
 **loopafstand_categorie_tot_gte** | **float**| Greater than or equal to; number | [optional] 
 **loopafstand_categorie_tot_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_tot_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_tot_lt** | **float**| Less than; number | [optional] 
 **loopafstand_categorie_tot_lte** | **float**| Less than or equal to; number | [optional] 
 **loopafstand_categorie_tot_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **loopafstand_categorie_vanaf** | **float**| De loopafstand vanaf een bepaalde meter. Volgens de loopafstand categorisatie. | [optional] 
 **loopafstand_categorie_vanaf_gt** | **float**| Greater than; number | [optional] 
 **loopafstand_categorie_vanaf_gte** | **float**| Greater than or equal to; number | [optional] 
 **loopafstand_categorie_vanaf_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_vanaf_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_vanaf_lt** | **float**| Less than; number | [optional] 
 **loopafstand_categorie_vanaf_lte** | **float**| Less than or equal to; number | [optional] 
 **loopafstand_categorie_vanaf_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **servicegebieden_locatie_id** | **str**| Unieke identificatie van een afval servicegebied locatie | [optional] 
 **servicegebieden_locatie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **servicegebieden_locatie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **servicegebieden_locatie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **servicegebieden_locatie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **servicegebieden_locatie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalservicegebiedenList**](PaginatedHuishoudelijkafvalservicegebiedenList.md)

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

# **huishoudelijkafval_servicegebieden_retrieve_slash**
> Huishoudelijkafvalservicegebieden huishoudelijkafval_servicegebieden_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_object_id=bag_object_id, bag_object_id_in=bag_object_id_in, bag_object_id_isempty=bag_object_id_isempty, bag_object_id_isnull=bag_object_id_isnull, bag_object_id_like=bag_object_id_like, bag_object_id_not=bag_object_id_not, bag_object_type=bag_object_type, bag_object_type_in=bag_object_type_in, bag_object_type_isempty=bag_object_type_isempty, bag_object_type_isnull=bag_object_type_isnull, bag_object_type_like=bag_object_type_like, bag_object_type_not=bag_object_type_not, categorie_verwijderd_dp=categorie_verwijderd_dp, categorie_verwijderd_dp_isnull=categorie_verwijderd_dp_isnull, categorie_wijzigingsdatum_dp=categorie_wijzigingsdatum_dp, categorie_wijzigingsdatum_dp_gt=categorie_wijzigingsdatum_dp_gt, categorie_wijzigingsdatum_dp_gte=categorie_wijzigingsdatum_dp_gte, categorie_wijzigingsdatum_dp_in=categorie_wijzigingsdatum_dp_in, categorie_wijzigingsdatum_dp_isnull=categorie_wijzigingsdatum_dp_isnull, categorie_wijzigingsdatum_dp_lt=categorie_wijzigingsdatum_dp_lt, categorie_wijzigingsdatum_dp_lte=categorie_wijzigingsdatum_dp_lte, categorie_wijzigingsdatum_dp_not=categorie_wijzigingsdatum_dp_not, fractie_code=fractie_code, fractie_code_in=fractie_code_in, fractie_code_isempty=fractie_code_isempty, fractie_code_isnull=fractie_code_isnull, fractie_code_like=fractie_code_like, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, geometrie=geometrie, geometrie_contains=geometrie_contains, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand_categorie_id=loopafstand_categorie_id, loopafstand_categorie_id_in=loopafstand_categorie_id_in, loopafstand_categorie_id_isempty=loopafstand_categorie_id_isempty, loopafstand_categorie_id_isnull=loopafstand_categorie_id_isnull, loopafstand_categorie_id_like=loopafstand_categorie_id_like, loopafstand_categorie_id_not=loopafstand_categorie_id_not, loopafstand_categorie_omschrijving=loopafstand_categorie_omschrijving, loopafstand_categorie_omschrijving_in=loopafstand_categorie_omschrijving_in, loopafstand_categorie_omschrijving_isempty=loopafstand_categorie_omschrijving_isempty, loopafstand_categorie_omschrijving_isnull=loopafstand_categorie_omschrijving_isnull, loopafstand_categorie_omschrijving_like=loopafstand_categorie_omschrijving_like, loopafstand_categorie_omschrijving_not=loopafstand_categorie_omschrijving_not, loopafstand_categorie_tot=loopafstand_categorie_tot, loopafstand_categorie_tot_gt=loopafstand_categorie_tot_gt, loopafstand_categorie_tot_gte=loopafstand_categorie_tot_gte, loopafstand_categorie_tot_in=loopafstand_categorie_tot_in, loopafstand_categorie_tot_isnull=loopafstand_categorie_tot_isnull, loopafstand_categorie_tot_lt=loopafstand_categorie_tot_lt, loopafstand_categorie_tot_lte=loopafstand_categorie_tot_lte, loopafstand_categorie_tot_not=loopafstand_categorie_tot_not, loopafstand_categorie_vanaf=loopafstand_categorie_vanaf, loopafstand_categorie_vanaf_gt=loopafstand_categorie_vanaf_gt, loopafstand_categorie_vanaf_gte=loopafstand_categorie_vanaf_gte, loopafstand_categorie_vanaf_in=loopafstand_categorie_vanaf_in, loopafstand_categorie_vanaf_isnull=loopafstand_categorie_vanaf_isnull, loopafstand_categorie_vanaf_lt=loopafstand_categorie_vanaf_lt, loopafstand_categorie_vanaf_lte=loopafstand_categorie_vanaf_lte, loopafstand_categorie_vanaf_not=loopafstand_categorie_vanaf_not, servicegebieden_locatie_id=servicegebieden_locatie_id, servicegebieden_locatie_id_in=servicegebieden_locatie_id_in, servicegebieden_locatie_id_isempty=servicegebieden_locatie_id_isempty, servicegebieden_locatie_id_isnull=servicegebieden_locatie_id_isnull, servicegebieden_locatie_id_like=servicegebieden_locatie_id_like, servicegebieden_locatie_id_not=servicegebieden_locatie_id_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalservicegebieden import Huishoudelijkafvalservicegebieden
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
    api_instance = huishoudelijkafval_api_client.ServicegebiedenApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'servicegebiedenLocatie' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    bag_object_id = 'bag_object_id_example' # str | Unieke BAG object (pand, ligplaats en standplaats) identificatie (optional)
    bag_object_id_in = ['bag_object_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_object_id_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_object_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_object_id_like = 'bag_object_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_object_id_not = ['bag_object_id_not_example'] # List[str] | Exclude matches; text (optional)
    bag_object_type = 'bag_object_type_example' # str | Type BAG object (pand, ligplaats en standplaats) (optional)
    bag_object_type_in = ['bag_object_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_object_type_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_object_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_object_type_like = 'bag_object_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_object_type_not = ['bag_object_type_not_example'] # List[str] | Exclude matches; text (optional)
    categorie_verwijderd_dp = True # bool | De datum waarop de loopafstandcategorie in de datapijplijn is verwijderd. (optional)
    categorie_verwijderd_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    categorie_wijzigingsdatum_dp = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de loopafstandcategorie in de datapijplijn is gewijzigd (optional)
    categorie_wijzigingsdatum_dp_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    categorie_wijzigingsdatum_dp_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    categorie_wijzigingsdatum_dp_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    categorie_wijzigingsdatum_dp_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    categorie_wijzigingsdatum_dp_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    categorie_wijzigingsdatum_dp_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    categorie_wijzigingsdatum_dp_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    fractie_code = 'fractie_code_example' # str | Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood (optional)
    fractie_code_in = ['fractie_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_code_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_code_like = 'fractie_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_code_not = ['fractie_code_not_example'] # List[str] | Exclude matches; text (optional)
    fractie_omschrijving = 'fractie_omschrijving_example' # str | Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. (optional)
    fractie_omschrijving_in = ['fractie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fractie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    fractie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fractie_omschrijving_like = 'fractie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    fractie_omschrijving_not = ['fractie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    geometrie = 'geometrie_example' # str | Geometrie van het type POINT van de container RD (epsg:28992) (optional)
    geometrie_contains = 'geometrie_contains_example' # str | Use x,y or POINT(x y) (optional)
    geometrie_intersects = 'geometrie_intersects_example' # str | Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON (optional)
    geometrie_isnull = 'geometrie_isnull_example' # str | Whether the field has a NULL value or not. (optional)
    geometrie_not = 'geometrie_not_example' # str | GeoJSON | GEOMETRY(...) (optional)
    id2 = 'id_example' # str | Unieke identificatie van een afval servicegebied (optional)
    id_in = ['id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isempty = True # bool | Whether the field is empty or not. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_like = 'id_like_example' # str | Matches text using wildcards (? and *). (optional)
    id_not = ['id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_id = 'loopafstand_categorie_id_example' # str | Unieke identificatie van loopafstanden categoriën (optional)
    loopafstand_categorie_id_in = ['loopafstand_categorie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    loopafstand_categorie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_id_like = 'loopafstand_categorie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    loopafstand_categorie_id_not = ['loopafstand_categorie_id_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_omschrijving = 'loopafstand_categorie_omschrijving_example' # str | De loopafstanden zijn volgens een vastgestelde indelijng gecategoriseerd. Bijvoorbeeld: 30 - 90 meter (optional)
    loopafstand_categorie_omschrijving_in = ['loopafstand_categorie_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    loopafstand_categorie_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_omschrijving_like = 'loopafstand_categorie_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    loopafstand_categorie_omschrijving_not = ['loopafstand_categorie_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    loopafstand_categorie_tot = 3.4 # float | De loopafstand tot een bepaalde meter volgens de loopafstandcategorisatie. (optional)
    loopafstand_categorie_tot_gt = 3.4 # float | Greater than; number (optional)
    loopafstand_categorie_tot_gte = 3.4 # float | Greater than or equal to; number (optional)
    loopafstand_categorie_tot_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_tot_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_tot_lt = 3.4 # float | Less than; number (optional)
    loopafstand_categorie_tot_lte = 3.4 # float | Less than or equal to; number (optional)
    loopafstand_categorie_tot_not = [3.4] # List[float] | Exclude matches; number (optional)
    loopafstand_categorie_vanaf = 3.4 # float | De loopafstand vanaf een bepaalde meter. Volgens de loopafstand categorisatie. (optional)
    loopafstand_categorie_vanaf_gt = 3.4 # float | Greater than; number (optional)
    loopafstand_categorie_vanaf_gte = 3.4 # float | Greater than or equal to; number (optional)
    loopafstand_categorie_vanaf_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    loopafstand_categorie_vanaf_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    loopafstand_categorie_vanaf_lt = 3.4 # float | Less than; number (optional)
    loopafstand_categorie_vanaf_lte = 3.4 # float | Less than or equal to; number (optional)
    loopafstand_categorie_vanaf_not = [3.4] # List[float] | Exclude matches; number (optional)
    servicegebieden_locatie_id = 'servicegebieden_locatie_id_example' # str | Unieke identificatie van een afval servicegebied locatie (optional)
    servicegebieden_locatie_id_in = ['servicegebieden_locatie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    servicegebieden_locatie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    servicegebieden_locatie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    servicegebieden_locatie_id_like = 'servicegebieden_locatie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    servicegebieden_locatie_id_not = ['servicegebieden_locatie_id_not_example'] # List[str] | Exclude matches; text (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_servicegebieden_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, bag_object_id=bag_object_id, bag_object_id_in=bag_object_id_in, bag_object_id_isempty=bag_object_id_isempty, bag_object_id_isnull=bag_object_id_isnull, bag_object_id_like=bag_object_id_like, bag_object_id_not=bag_object_id_not, bag_object_type=bag_object_type, bag_object_type_in=bag_object_type_in, bag_object_type_isempty=bag_object_type_isempty, bag_object_type_isnull=bag_object_type_isnull, bag_object_type_like=bag_object_type_like, bag_object_type_not=bag_object_type_not, categorie_verwijderd_dp=categorie_verwijderd_dp, categorie_verwijderd_dp_isnull=categorie_verwijderd_dp_isnull, categorie_wijzigingsdatum_dp=categorie_wijzigingsdatum_dp, categorie_wijzigingsdatum_dp_gt=categorie_wijzigingsdatum_dp_gt, categorie_wijzigingsdatum_dp_gte=categorie_wijzigingsdatum_dp_gte, categorie_wijzigingsdatum_dp_in=categorie_wijzigingsdatum_dp_in, categorie_wijzigingsdatum_dp_isnull=categorie_wijzigingsdatum_dp_isnull, categorie_wijzigingsdatum_dp_lt=categorie_wijzigingsdatum_dp_lt, categorie_wijzigingsdatum_dp_lte=categorie_wijzigingsdatum_dp_lte, categorie_wijzigingsdatum_dp_not=categorie_wijzigingsdatum_dp_not, fractie_code=fractie_code, fractie_code_in=fractie_code_in, fractie_code_isempty=fractie_code_isempty, fractie_code_isnull=fractie_code_isnull, fractie_code_like=fractie_code_like, fractie_code_not=fractie_code_not, fractie_omschrijving=fractie_omschrijving, fractie_omschrijving_in=fractie_omschrijving_in, fractie_omschrijving_isempty=fractie_omschrijving_isempty, fractie_omschrijving_isnull=fractie_omschrijving_isnull, fractie_omschrijving_like=fractie_omschrijving_like, fractie_omschrijving_not=fractie_omschrijving_not, geometrie=geometrie, geometrie_contains=geometrie_contains, geometrie_intersects=geometrie_intersects, geometrie_isnull=geometrie_isnull, geometrie_not=geometrie_not, id2=id2, id_in=id_in, id_isempty=id_isempty, id_isnull=id_isnull, id_like=id_like, id_not=id_not, loopafstand_categorie_id=loopafstand_categorie_id, loopafstand_categorie_id_in=loopafstand_categorie_id_in, loopafstand_categorie_id_isempty=loopafstand_categorie_id_isempty, loopafstand_categorie_id_isnull=loopafstand_categorie_id_isnull, loopafstand_categorie_id_like=loopafstand_categorie_id_like, loopafstand_categorie_id_not=loopafstand_categorie_id_not, loopafstand_categorie_omschrijving=loopafstand_categorie_omschrijving, loopafstand_categorie_omschrijving_in=loopafstand_categorie_omschrijving_in, loopafstand_categorie_omschrijving_isempty=loopafstand_categorie_omschrijving_isempty, loopafstand_categorie_omschrijving_isnull=loopafstand_categorie_omschrijving_isnull, loopafstand_categorie_omschrijving_like=loopafstand_categorie_omschrijving_like, loopafstand_categorie_omschrijving_not=loopafstand_categorie_omschrijving_not, loopafstand_categorie_tot=loopafstand_categorie_tot, loopafstand_categorie_tot_gt=loopafstand_categorie_tot_gt, loopafstand_categorie_tot_gte=loopafstand_categorie_tot_gte, loopafstand_categorie_tot_in=loopafstand_categorie_tot_in, loopafstand_categorie_tot_isnull=loopafstand_categorie_tot_isnull, loopafstand_categorie_tot_lt=loopafstand_categorie_tot_lt, loopafstand_categorie_tot_lte=loopafstand_categorie_tot_lte, loopafstand_categorie_tot_not=loopafstand_categorie_tot_not, loopafstand_categorie_vanaf=loopafstand_categorie_vanaf, loopafstand_categorie_vanaf_gt=loopafstand_categorie_vanaf_gt, loopafstand_categorie_vanaf_gte=loopafstand_categorie_vanaf_gte, loopafstand_categorie_vanaf_in=loopafstand_categorie_vanaf_in, loopafstand_categorie_vanaf_isnull=loopafstand_categorie_vanaf_isnull, loopafstand_categorie_vanaf_lt=loopafstand_categorie_vanaf_lt, loopafstand_categorie_vanaf_lte=loopafstand_categorie_vanaf_lte, loopafstand_categorie_vanaf_not=loopafstand_categorie_vanaf_not, servicegebieden_locatie_id=servicegebieden_locatie_id, servicegebieden_locatie_id_in=servicegebieden_locatie_id_in, servicegebieden_locatie_id_isempty=servicegebieden_locatie_id_isempty, servicegebieden_locatie_id_isnull=servicegebieden_locatie_id_isnull, servicegebieden_locatie_id_like=servicegebieden_locatie_id_like, servicegebieden_locatie_id_not=servicegebieden_locatie_id_not)
        print("The response of ServicegebiedenApi->huishoudelijkafval_servicegebieden_retrieve_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ServicegebiedenApi->huishoudelijkafval_servicegebieden_retrieve_slash: %s\n" % e)
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
 **bag_object_id** | **str**| Unieke BAG object (pand, ligplaats en standplaats) identificatie | [optional] 
 **bag_object_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_object_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_object_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_object_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_object_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_object_type** | **str**| Type BAG object (pand, ligplaats en standplaats) | [optional] 
 **bag_object_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_object_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_object_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_object_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_object_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **categorie_verwijderd_dp** | **bool**| De datum waarop de loopafstandcategorie in de datapijplijn is verwijderd. | [optional] 
 **categorie_verwijderd_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **categorie_wijzigingsdatum_dp** | **datetime**| De datum waarop de loopafstandcategorie in de datapijplijn is gewijzigd | [optional] 
 **categorie_wijzigingsdatum_dp_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **categorie_wijzigingsdatum_dp_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **categorie_wijzigingsdatum_dp_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **categorie_wijzigingsdatum_dp_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **categorie_wijzigingsdatum_dp_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **categorie_wijzigingsdatum_dp_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **categorie_wijzigingsdatum_dp_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **fractie_code** | **str**| Type afvalfractie code waarvoor de container is bedoeld: 1 - Rest, 2 - Glas, 3 - Papier, 4 - Plastic, 5 - Textiel, 6 - GFT, 9 - Brood | [optional] 
 **fractie_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **fractie_omschrijving** | **str**| Afvalcontainer fractieomschrijving zoals door leverancier is geleverd. | [optional] 
 **fractie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fractie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fractie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fractie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fractie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **geometrie** | **str**| Geometrie van het type POINT van de container RD (epsg:28992) | [optional] 
 **geometrie_contains** | **str**| Use x,y or POINT(x y) | [optional] 
 **geometrie_intersects** | **str**| Use WKT (POLYGON((x1 y1, x2 y2, ...))) or GeoJSON | [optional] 
 **geometrie_isnull** | **str**| Whether the field has a NULL value or not. | [optional] 
 **geometrie_not** | **str**| GeoJSON | GEOMETRY(...) | [optional] 
 **id2** | **str**| Unieke identificatie van een afval servicegebied | [optional] 
 **id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_id** | **str**| Unieke identificatie van loopafstanden categoriën | [optional] 
 **loopafstand_categorie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **loopafstand_categorie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **loopafstand_categorie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_omschrijving** | **str**| De loopafstanden zijn volgens een vastgestelde indelijng gecategoriseerd. Bijvoorbeeld: 30 - 90 meter | [optional] 
 **loopafstand_categorie_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **loopafstand_categorie_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **loopafstand_categorie_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **loopafstand_categorie_tot** | **float**| De loopafstand tot een bepaalde meter volgens de loopafstandcategorisatie. | [optional] 
 **loopafstand_categorie_tot_gt** | **float**| Greater than; number | [optional] 
 **loopafstand_categorie_tot_gte** | **float**| Greater than or equal to; number | [optional] 
 **loopafstand_categorie_tot_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_tot_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_tot_lt** | **float**| Less than; number | [optional] 
 **loopafstand_categorie_tot_lte** | **float**| Less than or equal to; number | [optional] 
 **loopafstand_categorie_tot_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **loopafstand_categorie_vanaf** | **float**| De loopafstand vanaf een bepaalde meter. Volgens de loopafstand categorisatie. | [optional] 
 **loopafstand_categorie_vanaf_gt** | **float**| Greater than; number | [optional] 
 **loopafstand_categorie_vanaf_gte** | **float**| Greater than or equal to; number | [optional] 
 **loopafstand_categorie_vanaf_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **loopafstand_categorie_vanaf_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **loopafstand_categorie_vanaf_lt** | **float**| Less than; number | [optional] 
 **loopafstand_categorie_vanaf_lte** | **float**| Less than or equal to; number | [optional] 
 **loopafstand_categorie_vanaf_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **servicegebieden_locatie_id** | **str**| Unieke identificatie van een afval servicegebied locatie | [optional] 
 **servicegebieden_locatie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **servicegebieden_locatie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **servicegebieden_locatie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **servicegebieden_locatie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **servicegebieden_locatie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 

### Return type

[**Huishoudelijkafvalservicegebieden**](Huishoudelijkafvalservicegebieden.md)

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

