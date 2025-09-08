# huishoudelijkafval_api_client.RolcontainerMeldingApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_rolcontainer_melding_list_slash**](RolcontainerMeldingApi.md#huishoudelijkafval_rolcontainer_melding_list_slash) | **GET** /rolcontainer_melding | 
[**huishoudelijkafval_rolcontainer_melding_retrieve_slash**](RolcontainerMeldingApi.md#huishoudelijkafval_rolcontainer_melding_retrieve_slash) | **GET** /rolcontainer_melding/{id} | 


# **huishoudelijkafval_rolcontainer_melding_list_slash**
> PaginatedHuishoudelijkafvalrolcontainerMeldingList huishoudelijkafval_rolcontainer_melding_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, afkomst_verzoek=afkomst_verzoek, afkomst_verzoek_in=afkomst_verzoek_in, afkomst_verzoek_isempty=afkomst_verzoek_isempty, afkomst_verzoek_isnull=afkomst_verzoek_isnull, afkomst_verzoek_like=afkomst_verzoek_like, afkomst_verzoek_not=afkomst_verzoek_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, melding_type=melding_type, melding_type_in=melding_type_in, melding_type_isempty=melding_type_isempty, melding_type_isnull=melding_type_isnull, melding_type_like=melding_type_like, melding_type_not=melding_type_not, page=page, rolcontainer_id=rolcontainer_id, rolcontainer_id_gt=rolcontainer_id_gt, rolcontainer_id_gte=rolcontainer_id_gte, rolcontainer_id_in=rolcontainer_id_in, rolcontainer_id_isnull=rolcontainer_id_isnull, rolcontainer_id_lt=rolcontainer_id_lt, rolcontainer_id_lte=rolcontainer_id_lte, rolcontainer_id_not=rolcontainer_id_not, soort_verzoek=soort_verzoek, soort_verzoek_in=soort_verzoek_in, soort_verzoek_isempty=soort_verzoek_isempty, soort_verzoek_isnull=soort_verzoek_isnull, soort_verzoek_like=soort_verzoek_like, soort_verzoek_not=soort_verzoek_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not)

Deze tabel bevat informatie over de meldingen die door de bewoners zijn gedaan. De meldingen gaan over een of meer containers.

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalrolcontainer_melding_list import PaginatedHuishoudelijkafvalrolcontainerMeldingList
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
    api_instance = huishoudelijkafval_api_client.RolcontainerMeldingApi(api_client)
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
    aanmaakdatum = '2013-10-20T19:20:30+01:00' # datetime | De datum en tijd waarop de registratie van de melding in het systeem is vastgelegd (optional)
    aanmaakdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aanmaakdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aanmaakdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    afkomst_verzoek = 'afkomst_verzoek_example' # str | Dit attribuut geeft aan of de melding intern of extern is gedaan. (optional)
    afkomst_verzoek_in = ['afkomst_verzoek_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    afkomst_verzoek_isempty = True # bool | Whether the field is empty or not. (optional)
    afkomst_verzoek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    afkomst_verzoek_like = 'afkomst_verzoek_like_example' # str | Matches text using wildcards (? and *). (optional)
    afkomst_verzoek_not = ['afkomst_verzoek_not_example'] # List[str] | Exclude matches; text (optional)
    bag_nummeraanduiding_identificatie = 'bag_nummeraanduiding_identificatie_example' # str | De unieke aanduiding van een nummeraanduiding (optional)
    bag_nummeraanduiding_identificatie_in = ['bag_nummeraanduiding_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_nummeraanduiding_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_nummeraanduiding_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_nummeraanduiding_identificatie_like = 'bag_nummeraanduiding_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_nummeraanduiding_identificatie_not = ['bag_nummeraanduiding_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_verblijfsobject_identificatie = 'bag_verblijfsobject_identificatie_example' # str | De unieke aanduiding van een verblijfsobject (optional)
    bag_verblijfsobject_identificatie_in = ['bag_verblijfsobject_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_verblijfsobject_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_verblijfsobject_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_verblijfsobject_identificatie_like = 'bag_verblijfsobject_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_verblijfsobject_identificatie_not = ['bag_verblijfsobject_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    id = 56 # int | Unieke aanduiding van een melding (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    melding_type = 'melding_type_example' # str | Het type van een melding. Bijvoorbeeld: Algemene informatie (optional)
    melding_type_in = ['melding_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    melding_type_isempty = True # bool | Whether the field is empty or not. (optional)
    melding_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    melding_type_like = 'melding_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    melding_type_not = ['melding_type_not_example'] # List[str] | Exclude matches; text (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    rolcontainer_id = 56 # int | Unieke aanduiding van een rolcontainer (optional)
    rolcontainer_id_gt = 56 # int | Greater than; number (optional)
    rolcontainer_id_gte = 56 # int | Greater than or equal to; number (optional)
    rolcontainer_id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    rolcontainer_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    rolcontainer_id_lt = 56 # int | Less than; number (optional)
    rolcontainer_id_lte = 56 # int | Less than or equal to; number (optional)
    rolcontainer_id_not = [56] # List[int] | Exclude matches; number (optional)
    soort_verzoek = 'soort_verzoek_example' # str | Dit attribuut geeft aan welk communicatiemiddel is gebruikt om de melding te registreren. (optional)
    soort_verzoek_in = ['soort_verzoek_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_verzoek_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_verzoek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_verzoek_like = 'soort_verzoek_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_verzoek_not = ['soort_verzoek_not_example'] # List[str] | Exclude matches; text (optional)
    wijzigingsdatum = '2013-10-20T19:20:30+01:00' # datetime | De datum en tijd waarop de registratie van de melding voor het laatst in het systeem is aangepast (optional)
    wijzigingsdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_rolcontainer_melding_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, afkomst_verzoek=afkomst_verzoek, afkomst_verzoek_in=afkomst_verzoek_in, afkomst_verzoek_isempty=afkomst_verzoek_isempty, afkomst_verzoek_isnull=afkomst_verzoek_isnull, afkomst_verzoek_like=afkomst_verzoek_like, afkomst_verzoek_not=afkomst_verzoek_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, melding_type=melding_type, melding_type_in=melding_type_in, melding_type_isempty=melding_type_isempty, melding_type_isnull=melding_type_isnull, melding_type_like=melding_type_like, melding_type_not=melding_type_not, page=page, rolcontainer_id=rolcontainer_id, rolcontainer_id_gt=rolcontainer_id_gt, rolcontainer_id_gte=rolcontainer_id_gte, rolcontainer_id_in=rolcontainer_id_in, rolcontainer_id_isnull=rolcontainer_id_isnull, rolcontainer_id_lt=rolcontainer_id_lt, rolcontainer_id_lte=rolcontainer_id_lte, rolcontainer_id_not=rolcontainer_id_not, soort_verzoek=soort_verzoek, soort_verzoek_in=soort_verzoek_in, soort_verzoek_isempty=soort_verzoek_isempty, soort_verzoek_isnull=soort_verzoek_isnull, soort_verzoek_like=soort_verzoek_like, soort_verzoek_not=soort_verzoek_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not)
        print("The response of RolcontainerMeldingApi->huishoudelijkafval_rolcontainer_melding_list_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolcontainerMeldingApi->huishoudelijkafval_rolcontainer_melding_list_slash: %s\n" % e)
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
 **aanmaakdatum** | **datetime**| De datum en tijd waarop de registratie van de melding in het systeem is vastgelegd | [optional] 
 **aanmaakdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aanmaakdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aanmaakdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **afkomst_verzoek** | **str**| Dit attribuut geeft aan of de melding intern of extern is gedaan. | [optional] 
 **afkomst_verzoek_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **afkomst_verzoek_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **afkomst_verzoek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **afkomst_verzoek_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **afkomst_verzoek_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_nummeraanduiding_identificatie** | **str**| De unieke aanduiding van een nummeraanduiding | [optional] 
 **bag_nummeraanduiding_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_nummeraanduiding_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_nummeraanduiding_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_nummeraanduiding_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_nummeraanduiding_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_verblijfsobject_identificatie** | **str**| De unieke aanduiding van een verblijfsobject | [optional] 
 **bag_verblijfsobject_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_verblijfsobject_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_verblijfsobject_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_verblijfsobject_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_verblijfsobject_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id** | **int**| Unieke aanduiding van een melding | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **melding_type** | **str**| Het type van een melding. Bijvoorbeeld: Algemene informatie | [optional] 
 **melding_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **melding_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **melding_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **melding_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **melding_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **rolcontainer_id** | **int**| Unieke aanduiding van een rolcontainer | [optional] 
 **rolcontainer_id_gt** | **int**| Greater than; number | [optional] 
 **rolcontainer_id_gte** | **int**| Greater than or equal to; number | [optional] 
 **rolcontainer_id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **rolcontainer_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **rolcontainer_id_lt** | **int**| Less than; number | [optional] 
 **rolcontainer_id_lte** | **int**| Less than or equal to; number | [optional] 
 **rolcontainer_id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **soort_verzoek** | **str**| Dit attribuut geeft aan welk communicatiemiddel is gebruikt om de melding te registreren. | [optional] 
 **soort_verzoek_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_verzoek_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_verzoek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_verzoek_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_verzoek_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **wijzigingsdatum** | **datetime**| De datum en tijd waarop de registratie van de melding voor het laatst in het systeem is aangepast | [optional] 
 **wijzigingsdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalrolcontainerMeldingList**](PaginatedHuishoudelijkafvalrolcontainerMeldingList.md)

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

# **huishoudelijkafval_rolcontainer_melding_retrieve_slash**
> HuishoudelijkafvalrolcontainerMelding huishoudelijkafval_rolcontainer_melding_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, afkomst_verzoek=afkomst_verzoek, afkomst_verzoek_in=afkomst_verzoek_in, afkomst_verzoek_isempty=afkomst_verzoek_isempty, afkomst_verzoek_isnull=afkomst_verzoek_isnull, afkomst_verzoek_like=afkomst_verzoek_like, afkomst_verzoek_not=afkomst_verzoek_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, melding_type=melding_type, melding_type_in=melding_type_in, melding_type_isempty=melding_type_isempty, melding_type_isnull=melding_type_isnull, melding_type_like=melding_type_like, melding_type_not=melding_type_not, rolcontainer_id=rolcontainer_id, rolcontainer_id_gt=rolcontainer_id_gt, rolcontainer_id_gte=rolcontainer_id_gte, rolcontainer_id_in=rolcontainer_id_in, rolcontainer_id_isnull=rolcontainer_id_isnull, rolcontainer_id_lt=rolcontainer_id_lt, rolcontainer_id_lte=rolcontainer_id_lte, rolcontainer_id_not=rolcontainer_id_not, soort_verzoek=soort_verzoek, soort_verzoek_in=soort_verzoek_in, soort_verzoek_isempty=soort_verzoek_isempty, soort_verzoek_isnull=soort_verzoek_isnull, soort_verzoek_like=soort_verzoek_like, soort_verzoek_not=soort_verzoek_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalrolcontainer_melding import HuishoudelijkafvalrolcontainerMelding
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
    api_instance = huishoudelijkafval_api_client.RolcontainerMeldingApi(api_client)
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
    aanmaakdatum = '2013-10-20T19:20:30+01:00' # datetime | De datum en tijd waarop de registratie van de melding in het systeem is vastgelegd (optional)
    aanmaakdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aanmaakdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aanmaakdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    aanmaakdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    afkomst_verzoek = 'afkomst_verzoek_example' # str | Dit attribuut geeft aan of de melding intern of extern is gedaan. (optional)
    afkomst_verzoek_in = ['afkomst_verzoek_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    afkomst_verzoek_isempty = True # bool | Whether the field is empty or not. (optional)
    afkomst_verzoek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    afkomst_verzoek_like = 'afkomst_verzoek_like_example' # str | Matches text using wildcards (? and *). (optional)
    afkomst_verzoek_not = ['afkomst_verzoek_not_example'] # List[str] | Exclude matches; text (optional)
    bag_nummeraanduiding_identificatie = 'bag_nummeraanduiding_identificatie_example' # str | De unieke aanduiding van een nummeraanduiding (optional)
    bag_nummeraanduiding_identificatie_in = ['bag_nummeraanduiding_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_nummeraanduiding_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_nummeraanduiding_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_nummeraanduiding_identificatie_like = 'bag_nummeraanduiding_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_nummeraanduiding_identificatie_not = ['bag_nummeraanduiding_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    bag_verblijfsobject_identificatie = 'bag_verblijfsobject_identificatie_example' # str | De unieke aanduiding van een verblijfsobject (optional)
    bag_verblijfsobject_identificatie_in = ['bag_verblijfsobject_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bag_verblijfsobject_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    bag_verblijfsobject_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bag_verblijfsobject_identificatie_like = 'bag_verblijfsobject_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    bag_verblijfsobject_identificatie_not = ['bag_verblijfsobject_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    id2 = 56 # int | Unieke aanduiding van een melding (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    melding_type = 'melding_type_example' # str | Het type van een melding. Bijvoorbeeld: Algemene informatie (optional)
    melding_type_in = ['melding_type_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    melding_type_isempty = True # bool | Whether the field is empty or not. (optional)
    melding_type_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    melding_type_like = 'melding_type_like_example' # str | Matches text using wildcards (? and *). (optional)
    melding_type_not = ['melding_type_not_example'] # List[str] | Exclude matches; text (optional)
    rolcontainer_id = 56 # int | Unieke aanduiding van een rolcontainer (optional)
    rolcontainer_id_gt = 56 # int | Greater than; number (optional)
    rolcontainer_id_gte = 56 # int | Greater than or equal to; number (optional)
    rolcontainer_id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    rolcontainer_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    rolcontainer_id_lt = 56 # int | Less than; number (optional)
    rolcontainer_id_lte = 56 # int | Less than or equal to; number (optional)
    rolcontainer_id_not = [56] # List[int] | Exclude matches; number (optional)
    soort_verzoek = 'soort_verzoek_example' # str | Dit attribuut geeft aan welk communicatiemiddel is gebruikt om de melding te registreren. (optional)
    soort_verzoek_in = ['soort_verzoek_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_verzoek_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_verzoek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_verzoek_like = 'soort_verzoek_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_verzoek_not = ['soort_verzoek_not_example'] # List[str] | Exclude matches; text (optional)
    wijzigingsdatum = '2013-10-20T19:20:30+01:00' # datetime | De datum en tijd waarop de registratie van de melding voor het laatst in het systeem is aangepast (optional)
    wijzigingsdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_rolcontainer_melding_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, afkomst_verzoek=afkomst_verzoek, afkomst_verzoek_in=afkomst_verzoek_in, afkomst_verzoek_isempty=afkomst_verzoek_isempty, afkomst_verzoek_isnull=afkomst_verzoek_isnull, afkomst_verzoek_like=afkomst_verzoek_like, afkomst_verzoek_not=afkomst_verzoek_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, melding_type=melding_type, melding_type_in=melding_type_in, melding_type_isempty=melding_type_isempty, melding_type_isnull=melding_type_isnull, melding_type_like=melding_type_like, melding_type_not=melding_type_not, rolcontainer_id=rolcontainer_id, rolcontainer_id_gt=rolcontainer_id_gt, rolcontainer_id_gte=rolcontainer_id_gte, rolcontainer_id_in=rolcontainer_id_in, rolcontainer_id_isnull=rolcontainer_id_isnull, rolcontainer_id_lt=rolcontainer_id_lt, rolcontainer_id_lte=rolcontainer_id_lte, rolcontainer_id_not=rolcontainer_id_not, soort_verzoek=soort_verzoek, soort_verzoek_in=soort_verzoek_in, soort_verzoek_isempty=soort_verzoek_isempty, soort_verzoek_isnull=soort_verzoek_isnull, soort_verzoek_like=soort_verzoek_like, soort_verzoek_not=soort_verzoek_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not)
        print("The response of RolcontainerMeldingApi->huishoudelijkafval_rolcontainer_melding_retrieve_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolcontainerMeldingApi->huishoudelijkafval_rolcontainer_melding_retrieve_slash: %s\n" % e)
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
 **aanmaakdatum** | **datetime**| De datum en tijd waarop de registratie van de melding in het systeem is vastgelegd | [optional] 
 **aanmaakdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aanmaakdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aanmaakdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **afkomst_verzoek** | **str**| Dit attribuut geeft aan of de melding intern of extern is gedaan. | [optional] 
 **afkomst_verzoek_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **afkomst_verzoek_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **afkomst_verzoek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **afkomst_verzoek_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **afkomst_verzoek_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_nummeraanduiding_identificatie** | **str**| De unieke aanduiding van een nummeraanduiding | [optional] 
 **bag_nummeraanduiding_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_nummeraanduiding_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_nummeraanduiding_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_nummeraanduiding_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_nummeraanduiding_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **bag_verblijfsobject_identificatie** | **str**| De unieke aanduiding van een verblijfsobject | [optional] 
 **bag_verblijfsobject_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bag_verblijfsobject_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **bag_verblijfsobject_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bag_verblijfsobject_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **bag_verblijfsobject_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id2** | **int**| Unieke aanduiding van een melding | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **melding_type** | **str**| Het type van een melding. Bijvoorbeeld: Algemene informatie | [optional] 
 **melding_type_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **melding_type_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **melding_type_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **melding_type_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **melding_type_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **rolcontainer_id** | **int**| Unieke aanduiding van een rolcontainer | [optional] 
 **rolcontainer_id_gt** | **int**| Greater than; number | [optional] 
 **rolcontainer_id_gte** | **int**| Greater than or equal to; number | [optional] 
 **rolcontainer_id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **rolcontainer_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **rolcontainer_id_lt** | **int**| Less than; number | [optional] 
 **rolcontainer_id_lte** | **int**| Less than or equal to; number | [optional] 
 **rolcontainer_id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **soort_verzoek** | **str**| Dit attribuut geeft aan welk communicatiemiddel is gebruikt om de melding te registreren. | [optional] 
 **soort_verzoek_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_verzoek_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_verzoek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_verzoek_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_verzoek_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **wijzigingsdatum** | **datetime**| De datum en tijd waarop de registratie van de melding voor het laatst in het systeem is aangepast | [optional] 
 **wijzigingsdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**HuishoudelijkafvalrolcontainerMelding**](HuishoudelijkafvalrolcontainerMelding.md)

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

