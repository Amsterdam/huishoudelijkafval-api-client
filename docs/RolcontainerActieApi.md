# huishoudelijkafval_api_client.RolcontainerActieApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_rolcontainer_actie_list2**](RolcontainerActieApi.md#huishoudelijkafval_rolcontainer_actie_list2) | **GET** /rolcontainer_actie | 
[**huishoudelijkafval_rolcontainer_actie_retrieve2**](RolcontainerActieApi.md#huishoudelijkafval_rolcontainer_actie_retrieve2) | **GET** /rolcontainer_actie/{id} | 


# **huishoudelijkafval_rolcontainer_actie_list2**
> PaginatedHuishoudelijkafvalrolcontainerActieList huishoudelijkafval_rolcontainer_actie_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, actie_type_code=actie_type_code, actie_type_code_in=actie_type_code_in, actie_type_code_isempty=actie_type_code_isempty, actie_type_code_isnull=actie_type_code_isnull, actie_type_code_like=actie_type_code_like, actie_type_code_not=actie_type_code_not, actie_type_naam=actie_type_naam, actie_type_naam_in=actie_type_naam_in, actie_type_naam_isempty=actie_type_naam_isempty, actie_type_naam_isnull=actie_type_naam_isnull, actie_type_naam_like=actie_type_naam_like, actie_type_naam_not=actie_type_naam_not, afkomst_verzoek=afkomst_verzoek, afkomst_verzoek_in=afkomst_verzoek_in, afkomst_verzoek_isempty=afkomst_verzoek_isempty, afkomst_verzoek_isnull=afkomst_verzoek_isnull, afkomst_verzoek_like=afkomst_verzoek_like, afkomst_verzoek_not=afkomst_verzoek_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bezoek=bezoek, bezoek_gt=bezoek_gt, bezoek_gte=bezoek_gte, bezoek_in=bezoek_in, bezoek_isnull=bezoek_isnull, bezoek_lt=bezoek_lt, bezoek_lte=bezoek_lte, bezoek_not=bezoek_not, chip_nummer=chip_nummer, chip_nummer_in=chip_nummer_in, chip_nummer_isempty=chip_nummer_isempty, chip_nummer_isnull=chip_nummer_isnull, chip_nummer_like=chip_nummer_like, chip_nummer_not=chip_nummer_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, interventie_datum=interventie_datum, interventie_datum_in=interventie_datum_in, interventie_datum_isempty=interventie_datum_isempty, interventie_datum_isnull=interventie_datum_isnull, interventie_datum_like=interventie_datum_like, interventie_datum_not=interventie_datum_not, page=page, rolcontainer_id=rolcontainer_id, rolcontainer_id_gt=rolcontainer_id_gt, rolcontainer_id_gte=rolcontainer_id_gte, rolcontainer_id_in=rolcontainer_id_in, rolcontainer_id_isnull=rolcontainer_id_isnull, rolcontainer_id_lt=rolcontainer_id_lt, rolcontainer_id_lte=rolcontainer_id_lte, rolcontainer_id_not=rolcontainer_id_not, ronde=ronde, ronde_in=ronde_in, ronde_isempty=ronde_isempty, ronde_isnull=ronde_isnull, ronde_like=ronde_like, ronde_not=ronde_not, soort_container=soort_container, soort_container_in=soort_container_in, soort_container_isempty=soort_container_isempty, soort_container_isnull=soort_container_isnull, soort_container_like=soort_container_like, soort_container_not=soort_container_not, soort_verzoek=soort_verzoek, soort_verzoek_in=soort_verzoek_in, soort_verzoek_isempty=soort_verzoek_isempty, soort_verzoek_isnull=soort_verzoek_isnull, soort_verzoek_like=soort_verzoek_like, soort_verzoek_not=soort_verzoek_not, status=status, status_in=status_in, status_isempty=status_isempty, status_isnull=status_isnull, status_like=status_like, status_not=status_not, team=team, team_in=team_in, team_isempty=team_isempty, team_isnull=team_isnull, team_like=team_like, team_not=team_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not)

Deze tabel bevat informatie over onderhoud handelingen.

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalrolcontainer_actie_list import PaginatedHuishoudelijkafvalrolcontainerActieList
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
    api_instance = huishoudelijkafval_api_client.RolcontainerActieApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
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
    actie_type_code = 'actie_type_code_example' # str | Dit attribuut beschrijft de code van de actie type (optional)
    actie_type_code_in = ['actie_type_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    actie_type_code_isempty = True # bool | Whether the field is empty or not. (optional)
    actie_type_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    actie_type_code_like = 'actie_type_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    actie_type_code_not = ['actie_type_code_not_example'] # List[str] | Exclude matches; text (optional)
    actie_type_naam = 'actie_type_naam_example' # str | Dit attribuut beschrijft de aard van de actie type (optional)
    actie_type_naam_in = ['actie_type_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    actie_type_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    actie_type_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    actie_type_naam_like = 'actie_type_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    actie_type_naam_not = ['actie_type_naam_not_example'] # List[str] | Exclude matches; text (optional)
    afkomst_verzoek = 'afkomst_verzoek_example' # str | Deze attribuut geeft aan of de actie door intern of extern verzoek is tot stand gekomen. (optional)
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
    bezoek = 56 # int | Het aantal bezoeken dat is afgelegd om het verzoek te realiseren. (optional)
    bezoek_gt = 56 # int | Greater than; number (optional)
    bezoek_gte = 56 # int | Greater than or equal to; number (optional)
    bezoek_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bezoek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bezoek_lt = 56 # int | Less than; number (optional)
    bezoek_lte = 56 # int | Less than or equal to; number (optional)
    bezoek_not = [56] # List[int] | Exclude matches; number (optional)
    chip_nummer = 'chip_nummer_example' # str | Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. (optional)
    chip_nummer_in = ['chip_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    chip_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    chip_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    chip_nummer_like = 'chip_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    chip_nummer_not = ['chip_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    id = 56 # int | Unieke aanduiding van een onderhoudsactie (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    interventie_datum = 'interventie_datum_example' # str | De geplande datum voor een bepaalde actie. (optional)
    interventie_datum_in = ['interventie_datum_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    interventie_datum_isempty = True # bool | Whether the field is empty or not. (optional)
    interventie_datum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    interventie_datum_like = 'interventie_datum_like_example' # str | Matches text using wildcards (? and *). (optional)
    interventie_datum_not = ['interventie_datum_not_example'] # List[str] | Exclude matches; text (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    rolcontainer_id = 56 # int | Unieke aanduiding van een rolcontainer (optional)
    rolcontainer_id_gt = 56 # int | Greater than; number (optional)
    rolcontainer_id_gte = 56 # int | Greater than or equal to; number (optional)
    rolcontainer_id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    rolcontainer_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    rolcontainer_id_lt = 56 # int | Less than; number (optional)
    rolcontainer_id_lte = 56 # int | Less than or equal to; number (optional)
    rolcontainer_id_not = [56] # List[int] | Exclude matches; number (optional)
    ronde = 'ronde_example' # str | Exact; text (optional)
    ronde_in = ['ronde_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    ronde_isempty = True # bool | Whether the field is empty or not. (optional)
    ronde_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    ronde_like = 'ronde_like_example' # str | Matches text using wildcards (? and *). (optional)
    ronde_not = ['ronde_not_example'] # List[str] | Exclude matches; text (optional)
    soort_container = 'soort_container_example' # str | Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. (optional)
    soort_container_in = ['soort_container_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_container_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_container_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_container_like = 'soort_container_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_container_not = ['soort_container_not_example'] # List[str] | Exclude matches; text (optional)
    soort_verzoek = 'soort_verzoek_example' # str | Dit attribuut geeft aan welk communicatiemiddel is gebruikt om het verzoek te registreren.. (optional)
    soort_verzoek_in = ['soort_verzoek_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_verzoek_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_verzoek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_verzoek_like = 'soort_verzoek_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_verzoek_not = ['soort_verzoek_not_example'] # List[str] | Exclude matches; text (optional)
    status = 'status_example' # str | Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. (optional)
    status_in = ['status_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isempty = True # bool | Whether the field is empty or not. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_like = 'status_like_example' # str | Matches text using wildcards (? and *). (optional)
    status_not = ['status_not_example'] # List[str] | Exclude matches; text (optional)
    team = 'team_example' # str | Het team dat verantwoordelijk is voor het afhandelen van het verzoek. (optional)
    team_in = ['team_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    team_isempty = True # bool | Whether the field is empty or not. (optional)
    team_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    team_like = 'team_like_example' # str | Matches text using wildcards (? and *). (optional)
    team_not = ['team_not_example'] # List[str] | Exclude matches; text (optional)
    wijzigingsdatum = '2013-10-20T19:20:30+01:00' # datetime | Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast (optional)
    wijzigingsdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_rolcontainer_actie_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, actie_type_code=actie_type_code, actie_type_code_in=actie_type_code_in, actie_type_code_isempty=actie_type_code_isempty, actie_type_code_isnull=actie_type_code_isnull, actie_type_code_like=actie_type_code_like, actie_type_code_not=actie_type_code_not, actie_type_naam=actie_type_naam, actie_type_naam_in=actie_type_naam_in, actie_type_naam_isempty=actie_type_naam_isempty, actie_type_naam_isnull=actie_type_naam_isnull, actie_type_naam_like=actie_type_naam_like, actie_type_naam_not=actie_type_naam_not, afkomst_verzoek=afkomst_verzoek, afkomst_verzoek_in=afkomst_verzoek_in, afkomst_verzoek_isempty=afkomst_verzoek_isempty, afkomst_verzoek_isnull=afkomst_verzoek_isnull, afkomst_verzoek_like=afkomst_verzoek_like, afkomst_verzoek_not=afkomst_verzoek_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bezoek=bezoek, bezoek_gt=bezoek_gt, bezoek_gte=bezoek_gte, bezoek_in=bezoek_in, bezoek_isnull=bezoek_isnull, bezoek_lt=bezoek_lt, bezoek_lte=bezoek_lte, bezoek_not=bezoek_not, chip_nummer=chip_nummer, chip_nummer_in=chip_nummer_in, chip_nummer_isempty=chip_nummer_isempty, chip_nummer_isnull=chip_nummer_isnull, chip_nummer_like=chip_nummer_like, chip_nummer_not=chip_nummer_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, interventie_datum=interventie_datum, interventie_datum_in=interventie_datum_in, interventie_datum_isempty=interventie_datum_isempty, interventie_datum_isnull=interventie_datum_isnull, interventie_datum_like=interventie_datum_like, interventie_datum_not=interventie_datum_not, page=page, rolcontainer_id=rolcontainer_id, rolcontainer_id_gt=rolcontainer_id_gt, rolcontainer_id_gte=rolcontainer_id_gte, rolcontainer_id_in=rolcontainer_id_in, rolcontainer_id_isnull=rolcontainer_id_isnull, rolcontainer_id_lt=rolcontainer_id_lt, rolcontainer_id_lte=rolcontainer_id_lte, rolcontainer_id_not=rolcontainer_id_not, ronde=ronde, ronde_in=ronde_in, ronde_isempty=ronde_isempty, ronde_isnull=ronde_isnull, ronde_like=ronde_like, ronde_not=ronde_not, soort_container=soort_container, soort_container_in=soort_container_in, soort_container_isempty=soort_container_isempty, soort_container_isnull=soort_container_isnull, soort_container_like=soort_container_like, soort_container_not=soort_container_not, soort_verzoek=soort_verzoek, soort_verzoek_in=soort_verzoek_in, soort_verzoek_isempty=soort_verzoek_isempty, soort_verzoek_isnull=soort_verzoek_isnull, soort_verzoek_like=soort_verzoek_like, soort_verzoek_not=soort_verzoek_not, status=status, status_in=status_in, status_isempty=status_isempty, status_isnull=status_isnull, status_like=status_like, status_not=status_not, team=team, team_in=team_in, team_isempty=team_isempty, team_isnull=team_isnull, team_like=team_like, team_not=team_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not)
        print("The response of RolcontainerActieApi->huishoudelijkafval_rolcontainer_actie_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolcontainerActieApi->huishoudelijkafval_rolcontainer_actie_list2: %s\n" % e)
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
 **aanmaakdatum** | **datetime**| Datum tijd waarop de rolcontainer in het systeem is aangemaakt | [optional] 
 **aanmaakdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aanmaakdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aanmaakdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **actie_type_code** | **str**| Dit attribuut beschrijft de code van de actie type | [optional] 
 **actie_type_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **actie_type_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **actie_type_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **actie_type_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **actie_type_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **actie_type_naam** | **str**| Dit attribuut beschrijft de aard van de actie type | [optional] 
 **actie_type_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **actie_type_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **actie_type_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **actie_type_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **actie_type_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **afkomst_verzoek** | **str**| Deze attribuut geeft aan of de actie door intern of extern verzoek is tot stand gekomen. | [optional] 
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
 **bezoek** | **int**| Het aantal bezoeken dat is afgelegd om het verzoek te realiseren. | [optional] 
 **bezoek_gt** | **int**| Greater than; number | [optional] 
 **bezoek_gte** | **int**| Greater than or equal to; number | [optional] 
 **bezoek_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bezoek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bezoek_lt** | **int**| Less than; number | [optional] 
 **bezoek_lte** | **int**| Less than or equal to; number | [optional] 
 **bezoek_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **chip_nummer** | **str**| Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. | [optional] 
 **chip_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **chip_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **chip_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **chip_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **chip_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id** | **int**| Unieke aanduiding van een onderhoudsactie | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **interventie_datum** | **str**| De geplande datum voor een bepaalde actie. | [optional] 
 **interventie_datum_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **interventie_datum_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **interventie_datum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **interventie_datum_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **interventie_datum_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **rolcontainer_id** | **int**| Unieke aanduiding van een rolcontainer | [optional] 
 **rolcontainer_id_gt** | **int**| Greater than; number | [optional] 
 **rolcontainer_id_gte** | **int**| Greater than or equal to; number | [optional] 
 **rolcontainer_id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **rolcontainer_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **rolcontainer_id_lt** | **int**| Less than; number | [optional] 
 **rolcontainer_id_lte** | **int**| Less than or equal to; number | [optional] 
 **rolcontainer_id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **ronde** | **str**| Exact; text | [optional] 
 **ronde_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **ronde_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **ronde_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **ronde_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **ronde_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **soort_container** | **str**| Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. | [optional] 
 **soort_container_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_container_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_container_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_container_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_container_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **soort_verzoek** | **str**| Dit attribuut geeft aan welk communicatiemiddel is gebruikt om het verzoek te registreren.. | [optional] 
 **soort_verzoek_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_verzoek_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_verzoek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_verzoek_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_verzoek_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **str**| Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. | [optional] 
 **status_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **status_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **team** | **str**| Het team dat verantwoordelijk is voor het afhandelen van het verzoek. | [optional] 
 **team_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **team_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **team_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **team_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **team_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **wijzigingsdatum** | **datetime**| Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast | [optional] 
 **wijzigingsdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalrolcontainerActieList**](PaginatedHuishoudelijkafvalrolcontainerActieList.md)

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

# **huishoudelijkafval_rolcontainer_actie_retrieve2**
> HuishoudelijkafvalrolcontainerActie huishoudelijkafval_rolcontainer_actie_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, actie_type_code=actie_type_code, actie_type_code_in=actie_type_code_in, actie_type_code_isempty=actie_type_code_isempty, actie_type_code_isnull=actie_type_code_isnull, actie_type_code_like=actie_type_code_like, actie_type_code_not=actie_type_code_not, actie_type_naam=actie_type_naam, actie_type_naam_in=actie_type_naam_in, actie_type_naam_isempty=actie_type_naam_isempty, actie_type_naam_isnull=actie_type_naam_isnull, actie_type_naam_like=actie_type_naam_like, actie_type_naam_not=actie_type_naam_not, afkomst_verzoek=afkomst_verzoek, afkomst_verzoek_in=afkomst_verzoek_in, afkomst_verzoek_isempty=afkomst_verzoek_isempty, afkomst_verzoek_isnull=afkomst_verzoek_isnull, afkomst_verzoek_like=afkomst_verzoek_like, afkomst_verzoek_not=afkomst_verzoek_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bezoek=bezoek, bezoek_gt=bezoek_gt, bezoek_gte=bezoek_gte, bezoek_in=bezoek_in, bezoek_isnull=bezoek_isnull, bezoek_lt=bezoek_lt, bezoek_lte=bezoek_lte, bezoek_not=bezoek_not, chip_nummer=chip_nummer, chip_nummer_in=chip_nummer_in, chip_nummer_isempty=chip_nummer_isempty, chip_nummer_isnull=chip_nummer_isnull, chip_nummer_like=chip_nummer_like, chip_nummer_not=chip_nummer_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, interventie_datum=interventie_datum, interventie_datum_in=interventie_datum_in, interventie_datum_isempty=interventie_datum_isempty, interventie_datum_isnull=interventie_datum_isnull, interventie_datum_like=interventie_datum_like, interventie_datum_not=interventie_datum_not, rolcontainer_id=rolcontainer_id, rolcontainer_id_gt=rolcontainer_id_gt, rolcontainer_id_gte=rolcontainer_id_gte, rolcontainer_id_in=rolcontainer_id_in, rolcontainer_id_isnull=rolcontainer_id_isnull, rolcontainer_id_lt=rolcontainer_id_lt, rolcontainer_id_lte=rolcontainer_id_lte, rolcontainer_id_not=rolcontainer_id_not, ronde=ronde, ronde_in=ronde_in, ronde_isempty=ronde_isempty, ronde_isnull=ronde_isnull, ronde_like=ronde_like, ronde_not=ronde_not, soort_container=soort_container, soort_container_in=soort_container_in, soort_container_isempty=soort_container_isempty, soort_container_isnull=soort_container_isnull, soort_container_like=soort_container_like, soort_container_not=soort_container_not, soort_verzoek=soort_verzoek, soort_verzoek_in=soort_verzoek_in, soort_verzoek_isempty=soort_verzoek_isempty, soort_verzoek_isnull=soort_verzoek_isnull, soort_verzoek_like=soort_verzoek_like, soort_verzoek_not=soort_verzoek_not, status=status, status_in=status_in, status_isempty=status_isempty, status_isnull=status_isnull, status_like=status_like, status_not=status_not, team=team, team_in=team_in, team_isempty=team_isempty, team_isnull=team_isnull, team_like=team_like, team_not=team_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalrolcontainer_actie import HuishoudelijkafvalrolcontainerActie
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
    api_instance = huishoudelijkafval_api_client.RolcontainerActieApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
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
    actie_type_code = 'actie_type_code_example' # str | Dit attribuut beschrijft de code van de actie type (optional)
    actie_type_code_in = ['actie_type_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    actie_type_code_isempty = True # bool | Whether the field is empty or not. (optional)
    actie_type_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    actie_type_code_like = 'actie_type_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    actie_type_code_not = ['actie_type_code_not_example'] # List[str] | Exclude matches; text (optional)
    actie_type_naam = 'actie_type_naam_example' # str | Dit attribuut beschrijft de aard van de actie type (optional)
    actie_type_naam_in = ['actie_type_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    actie_type_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    actie_type_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    actie_type_naam_like = 'actie_type_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    actie_type_naam_not = ['actie_type_naam_not_example'] # List[str] | Exclude matches; text (optional)
    afkomst_verzoek = 'afkomst_verzoek_example' # str | Deze attribuut geeft aan of de actie door intern of extern verzoek is tot stand gekomen. (optional)
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
    bezoek = 56 # int | Het aantal bezoeken dat is afgelegd om het verzoek te realiseren. (optional)
    bezoek_gt = 56 # int | Greater than; number (optional)
    bezoek_gte = 56 # int | Greater than or equal to; number (optional)
    bezoek_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    bezoek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    bezoek_lt = 56 # int | Less than; number (optional)
    bezoek_lte = 56 # int | Less than or equal to; number (optional)
    bezoek_not = [56] # List[int] | Exclude matches; number (optional)
    chip_nummer = 'chip_nummer_example' # str | Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. (optional)
    chip_nummer_in = ['chip_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    chip_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    chip_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    chip_nummer_like = 'chip_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    chip_nummer_not = ['chip_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    id2 = 56 # int | Unieke aanduiding van een onderhoudsactie (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    interventie_datum = 'interventie_datum_example' # str | De geplande datum voor een bepaalde actie. (optional)
    interventie_datum_in = ['interventie_datum_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    interventie_datum_isempty = True # bool | Whether the field is empty or not. (optional)
    interventie_datum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    interventie_datum_like = 'interventie_datum_like_example' # str | Matches text using wildcards (? and *). (optional)
    interventie_datum_not = ['interventie_datum_not_example'] # List[str] | Exclude matches; text (optional)
    rolcontainer_id = 56 # int | Unieke aanduiding van een rolcontainer (optional)
    rolcontainer_id_gt = 56 # int | Greater than; number (optional)
    rolcontainer_id_gte = 56 # int | Greater than or equal to; number (optional)
    rolcontainer_id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    rolcontainer_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    rolcontainer_id_lt = 56 # int | Less than; number (optional)
    rolcontainer_id_lte = 56 # int | Less than or equal to; number (optional)
    rolcontainer_id_not = [56] # List[int] | Exclude matches; number (optional)
    ronde = 'ronde_example' # str | Exact; text (optional)
    ronde_in = ['ronde_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    ronde_isempty = True # bool | Whether the field is empty or not. (optional)
    ronde_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    ronde_like = 'ronde_like_example' # str | Matches text using wildcards (? and *). (optional)
    ronde_not = ['ronde_not_example'] # List[str] | Exclude matches; text (optional)
    soort_container = 'soort_container_example' # str | Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. (optional)
    soort_container_in = ['soort_container_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_container_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_container_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_container_like = 'soort_container_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_container_not = ['soort_container_not_example'] # List[str] | Exclude matches; text (optional)
    soort_verzoek = 'soort_verzoek_example' # str | Dit attribuut geeft aan welk communicatiemiddel is gebruikt om het verzoek te registreren.. (optional)
    soort_verzoek_in = ['soort_verzoek_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_verzoek_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_verzoek_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_verzoek_like = 'soort_verzoek_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_verzoek_not = ['soort_verzoek_not_example'] # List[str] | Exclude matches; text (optional)
    status = 'status_example' # str | Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. (optional)
    status_in = ['status_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    status_isempty = True # bool | Whether the field is empty or not. (optional)
    status_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    status_like = 'status_like_example' # str | Matches text using wildcards (? and *). (optional)
    status_not = ['status_not_example'] # List[str] | Exclude matches; text (optional)
    team = 'team_example' # str | Het team dat verantwoordelijk is voor het afhandelen van het verzoek. (optional)
    team_in = ['team_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    team_isempty = True # bool | Whether the field is empty or not. (optional)
    team_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    team_like = 'team_like_example' # str | Matches text using wildcards (? and *). (optional)
    team_not = ['team_not_example'] # List[str] | Exclude matches; text (optional)
    wijzigingsdatum = '2013-10-20T19:20:30+01:00' # datetime | Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast (optional)
    wijzigingsdatum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    wijzigingsdatum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    wijzigingsdatum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    wijzigingsdatum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_rolcontainer_actie_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aanmaakdatum=aanmaakdatum, aanmaakdatum_gt=aanmaakdatum_gt, aanmaakdatum_gte=aanmaakdatum_gte, aanmaakdatum_in=aanmaakdatum_in, aanmaakdatum_isnull=aanmaakdatum_isnull, aanmaakdatum_lt=aanmaakdatum_lt, aanmaakdatum_lte=aanmaakdatum_lte, aanmaakdatum_not=aanmaakdatum_not, actie_type_code=actie_type_code, actie_type_code_in=actie_type_code_in, actie_type_code_isempty=actie_type_code_isempty, actie_type_code_isnull=actie_type_code_isnull, actie_type_code_like=actie_type_code_like, actie_type_code_not=actie_type_code_not, actie_type_naam=actie_type_naam, actie_type_naam_in=actie_type_naam_in, actie_type_naam_isempty=actie_type_naam_isempty, actie_type_naam_isnull=actie_type_naam_isnull, actie_type_naam_like=actie_type_naam_like, actie_type_naam_not=actie_type_naam_not, afkomst_verzoek=afkomst_verzoek, afkomst_verzoek_in=afkomst_verzoek_in, afkomst_verzoek_isempty=afkomst_verzoek_isempty, afkomst_verzoek_isnull=afkomst_verzoek_isnull, afkomst_verzoek_like=afkomst_verzoek_like, afkomst_verzoek_not=afkomst_verzoek_not, bag_nummeraanduiding_identificatie=bag_nummeraanduiding_identificatie, bag_nummeraanduiding_identificatie_in=bag_nummeraanduiding_identificatie_in, bag_nummeraanduiding_identificatie_isempty=bag_nummeraanduiding_identificatie_isempty, bag_nummeraanduiding_identificatie_isnull=bag_nummeraanduiding_identificatie_isnull, bag_nummeraanduiding_identificatie_like=bag_nummeraanduiding_identificatie_like, bag_nummeraanduiding_identificatie_not=bag_nummeraanduiding_identificatie_not, bag_verblijfsobject_identificatie=bag_verblijfsobject_identificatie, bag_verblijfsobject_identificatie_in=bag_verblijfsobject_identificatie_in, bag_verblijfsobject_identificatie_isempty=bag_verblijfsobject_identificatie_isempty, bag_verblijfsobject_identificatie_isnull=bag_verblijfsobject_identificatie_isnull, bag_verblijfsobject_identificatie_like=bag_verblijfsobject_identificatie_like, bag_verblijfsobject_identificatie_not=bag_verblijfsobject_identificatie_not, bezoek=bezoek, bezoek_gt=bezoek_gt, bezoek_gte=bezoek_gte, bezoek_in=bezoek_in, bezoek_isnull=bezoek_isnull, bezoek_lt=bezoek_lt, bezoek_lte=bezoek_lte, bezoek_not=bezoek_not, chip_nummer=chip_nummer, chip_nummer_in=chip_nummer_in, chip_nummer_isempty=chip_nummer_isempty, chip_nummer_isnull=chip_nummer_isnull, chip_nummer_like=chip_nummer_like, chip_nummer_not=chip_nummer_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, interventie_datum=interventie_datum, interventie_datum_in=interventie_datum_in, interventie_datum_isempty=interventie_datum_isempty, interventie_datum_isnull=interventie_datum_isnull, interventie_datum_like=interventie_datum_like, interventie_datum_not=interventie_datum_not, rolcontainer_id=rolcontainer_id, rolcontainer_id_gt=rolcontainer_id_gt, rolcontainer_id_gte=rolcontainer_id_gte, rolcontainer_id_in=rolcontainer_id_in, rolcontainer_id_isnull=rolcontainer_id_isnull, rolcontainer_id_lt=rolcontainer_id_lt, rolcontainer_id_lte=rolcontainer_id_lte, rolcontainer_id_not=rolcontainer_id_not, ronde=ronde, ronde_in=ronde_in, ronde_isempty=ronde_isempty, ronde_isnull=ronde_isnull, ronde_like=ronde_like, ronde_not=ronde_not, soort_container=soort_container, soort_container_in=soort_container_in, soort_container_isempty=soort_container_isempty, soort_container_isnull=soort_container_isnull, soort_container_like=soort_container_like, soort_container_not=soort_container_not, soort_verzoek=soort_verzoek, soort_verzoek_in=soort_verzoek_in, soort_verzoek_isempty=soort_verzoek_isempty, soort_verzoek_isnull=soort_verzoek_isnull, soort_verzoek_like=soort_verzoek_like, soort_verzoek_not=soort_verzoek_not, status=status, status_in=status_in, status_isempty=status_isempty, status_isnull=status_isnull, status_like=status_like, status_not=status_not, team=team, team_in=team_in, team_isempty=team_isempty, team_isnull=team_isnull, team_like=team_like, team_not=team_not, wijzigingsdatum=wijzigingsdatum, wijzigingsdatum_gt=wijzigingsdatum_gt, wijzigingsdatum_gte=wijzigingsdatum_gte, wijzigingsdatum_in=wijzigingsdatum_in, wijzigingsdatum_isnull=wijzigingsdatum_isnull, wijzigingsdatum_lt=wijzigingsdatum_lt, wijzigingsdatum_lte=wijzigingsdatum_lte, wijzigingsdatum_not=wijzigingsdatum_not)
        print("The response of RolcontainerActieApi->huishoudelijkafval_rolcontainer_actie_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolcontainerActieApi->huishoudelijkafval_rolcontainer_actie_retrieve2: %s\n" % e)
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
 **aanmaakdatum** | **datetime**| Datum tijd waarop de rolcontainer in het systeem is aangemaakt | [optional] 
 **aanmaakdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aanmaakdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aanmaakdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **aanmaakdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **actie_type_code** | **str**| Dit attribuut beschrijft de code van de actie type | [optional] 
 **actie_type_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **actie_type_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **actie_type_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **actie_type_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **actie_type_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **actie_type_naam** | **str**| Dit attribuut beschrijft de aard van de actie type | [optional] 
 **actie_type_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **actie_type_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **actie_type_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **actie_type_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **actie_type_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **afkomst_verzoek** | **str**| Deze attribuut geeft aan of de actie door intern of extern verzoek is tot stand gekomen. | [optional] 
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
 **bezoek** | **int**| Het aantal bezoeken dat is afgelegd om het verzoek te realiseren. | [optional] 
 **bezoek_gt** | **int**| Greater than; number | [optional] 
 **bezoek_gte** | **int**| Greater than or equal to; number | [optional] 
 **bezoek_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **bezoek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **bezoek_lt** | **int**| Less than; number | [optional] 
 **bezoek_lte** | **int**| Less than or equal to; number | [optional] 
 **bezoek_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **chip_nummer** | **str**| Unieke aanduiding van de chip dat aan de rolcontainer is bevestigd. Het chipnummer is van buitenaf niet leesbaar. | [optional] 
 **chip_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **chip_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **chip_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **chip_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **chip_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id2** | **int**| Unieke aanduiding van een onderhoudsactie | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **interventie_datum** | **str**| De geplande datum voor een bepaalde actie. | [optional] 
 **interventie_datum_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **interventie_datum_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **interventie_datum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **interventie_datum_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **interventie_datum_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **rolcontainer_id** | **int**| Unieke aanduiding van een rolcontainer | [optional] 
 **rolcontainer_id_gt** | **int**| Greater than; number | [optional] 
 **rolcontainer_id_gte** | **int**| Greater than or equal to; number | [optional] 
 **rolcontainer_id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **rolcontainer_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **rolcontainer_id_lt** | **int**| Less than; number | [optional] 
 **rolcontainer_id_lte** | **int**| Less than or equal to; number | [optional] 
 **rolcontainer_id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **ronde** | **str**| Exact; text | [optional] 
 **ronde_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **ronde_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **ronde_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **ronde_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **ronde_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **soort_container** | **str**| Dit attribuut geeft een aantal kenmerken (materieel, inhoud in liter en fractie) van een rolcontainer. Bijvoorbeeld: GFE/T 140 Kunststof. | [optional] 
 **soort_container_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_container_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_container_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_container_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_container_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **soort_verzoek** | **str**| Dit attribuut geeft aan welk communicatiemiddel is gebruikt om het verzoek te registreren.. | [optional] 
 **soort_verzoek_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_verzoek_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_verzoek_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_verzoek_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_verzoek_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **status** | **str**| Dit attribuut geeft de actuele status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. | [optional] 
 **status_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **status_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **status_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **status_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **status_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **team** | **str**| Het team dat verantwoordelijk is voor het afhandelen van het verzoek. | [optional] 
 **team_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **team_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **team_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **team_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **team_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **wijzigingsdatum** | **datetime**| Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast | [optional] 
 **wijzigingsdatum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **wijzigingsdatum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **wijzigingsdatum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **wijzigingsdatum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 

### Return type

[**HuishoudelijkafvalrolcontainerActie**](HuishoudelijkafvalrolcontainerActie.md)

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

