# huishoudelijkafval_api_client.PlanningVoertuigenApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_planning_voertuigen_list_slash**](PlanningVoertuigenApi.md#huishoudelijkafval_planning_voertuigen_list_slash) | **GET** /planning_voertuigen | 
[**huishoudelijkafval_planning_voertuigen_retrieve_slash**](PlanningVoertuigenApi.md#huishoudelijkafval_planning_voertuigen_retrieve_slash) | **GET** /planning_voertuigen/{id} | 


# **huishoudelijkafval_planning_voertuigen_list_slash**
> PaginatedHuishoudelijkafvalplanningVoertuigenList huishoudelijkafval_planning_voertuigen_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aantal_medewerkers=aantal_medewerkers, aantal_medewerkers_inhuur=aantal_medewerkers_inhuur, aantal_medewerkers_inhuur_gt=aantal_medewerkers_inhuur_gt, aantal_medewerkers_inhuur_gte=aantal_medewerkers_inhuur_gte, aantal_medewerkers_inhuur_in=aantal_medewerkers_inhuur_in, aantal_medewerkers_inhuur_isnull=aantal_medewerkers_inhuur_isnull, aantal_medewerkers_inhuur_lt=aantal_medewerkers_inhuur_lt, aantal_medewerkers_inhuur_lte=aantal_medewerkers_inhuur_lte, aantal_medewerkers_inhuur_not=aantal_medewerkers_inhuur_not, aantal_medewerkers_intern=aantal_medewerkers_intern, aantal_medewerkers_intern_gt=aantal_medewerkers_intern_gt, aantal_medewerkers_intern_gte=aantal_medewerkers_intern_gte, aantal_medewerkers_intern_in=aantal_medewerkers_intern_in, aantal_medewerkers_intern_isnull=aantal_medewerkers_intern_isnull, aantal_medewerkers_intern_lt=aantal_medewerkers_intern_lt, aantal_medewerkers_intern_lte=aantal_medewerkers_intern_lte, aantal_medewerkers_intern_not=aantal_medewerkers_intern_not, aantal_medewerkers_gt=aantal_medewerkers_gt, aantal_medewerkers_gte=aantal_medewerkers_gte, aantal_medewerkers_in=aantal_medewerkers_in, aantal_medewerkers_isnull=aantal_medewerkers_isnull, aantal_medewerkers_lt=aantal_medewerkers_lt, aantal_medewerkers_lte=aantal_medewerkers_lte, aantal_medewerkers_not=aantal_medewerkers_not, activiteit=activiteit, activiteit_in=activiteit_in, activiteit_isempty=activiteit_isempty, activiteit_isnull=activiteit_isnull, activiteit_like=activiteit_like, activiteit_not=activiteit_not, categorie=categorie, categorie_in=categorie_in, categorie_isempty=categorie_isempty, categorie_isnull=categorie_isnull, categorie_like=categorie_like, categorie_not=categorie_not, datum_aanwezig_bron=datum_aanwezig_bron, datum_aanwezig_bron_gt=datum_aanwezig_bron_gt, datum_aanwezig_bron_gte=datum_aanwezig_bron_gte, datum_aanwezig_bron_in=datum_aanwezig_bron_in, datum_aanwezig_bron_isnull=datum_aanwezig_bron_isnull, datum_aanwezig_bron_lt=datum_aanwezig_bron_lt, datum_aanwezig_bron_lte=datum_aanwezig_bron_lte, datum_aanwezig_bron_not=datum_aanwezig_bron_not, datum_verwerkt_stadsdelen=datum_verwerkt_stadsdelen, datum_verwerkt_stadsdelen_gt=datum_verwerkt_stadsdelen_gt, datum_verwerkt_stadsdelen_gte=datum_verwerkt_stadsdelen_gte, datum_verwerkt_stadsdelen_in=datum_verwerkt_stadsdelen_in, datum_verwerkt_stadsdelen_isnull=datum_verwerkt_stadsdelen_isnull, datum_verwerkt_stadsdelen_lt=datum_verwerkt_stadsdelen_lt, datum_verwerkt_stadsdelen_lte=datum_verwerkt_stadsdelen_lte, datum_verwerkt_stadsdelen_not=datum_verwerkt_stadsdelen_not, fase=fase, fase_in=fase_in, fase_isempty=fase_isempty, fase_isnull=fase_isnull, fase_like=fase_like, fase_not=fase_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, kenteken=kenteken, kenteken_kort=kenteken_kort, kenteken_kort_in=kenteken_kort_in, kenteken_kort_isempty=kenteken_kort_isempty, kenteken_kort_isnull=kenteken_kort_isnull, kenteken_kort_like=kenteken_kort_like, kenteken_kort_not=kenteken_kort_not, kenteken_in=kenteken_in, kenteken_isempty=kenteken_isempty, kenteken_isnull=kenteken_isnull, kenteken_like=kenteken_like, kenteken_not=kenteken_not, memo=memo, memo_in=memo_in, memo_isempty=memo_isempty, memo_isnull=memo_isnull, memo_like=memo_like, memo_not=memo_not, page=page, pauze_eindtijd=pauze_eindtijd, pauze_eindtijd_in=pauze_eindtijd_in, pauze_eindtijd_isempty=pauze_eindtijd_isempty, pauze_eindtijd_isnull=pauze_eindtijd_isnull, pauze_eindtijd_like=pauze_eindtijd_like, pauze_eindtijd_not=pauze_eindtijd_not, pauze_starttijd=pauze_starttijd, pauze_starttijd_in=pauze_starttijd_in, pauze_starttijd_isempty=pauze_starttijd_isempty, pauze_starttijd_isnull=pauze_starttijd_isnull, pauze_starttijd_like=pauze_starttijd_like, pauze_starttijd_not=pauze_starttijd_not, pauze_uren_gepland=pauze_uren_gepland, pauze_uren_gepland_gt=pauze_uren_gepland_gt, pauze_uren_gepland_gte=pauze_uren_gepland_gte, pauze_uren_gepland_in=pauze_uren_gepland_in, pauze_uren_gepland_isnull=pauze_uren_gepland_isnull, pauze_uren_gepland_lt=pauze_uren_gepland_lt, pauze_uren_gepland_lte=pauze_uren_gepland_lte, pauze_uren_gepland_not=pauze_uren_gepland_not, soort_werkzaamheden=soort_werkzaamheden, soort_werkzaamheden_in=soort_werkzaamheden_in, soort_werkzaamheden_isempty=soort_werkzaamheden_isempty, soort_werkzaamheden_isnull=soort_werkzaamheden_isnull, soort_werkzaamheden_like=soort_werkzaamheden_like, soort_werkzaamheden_not=soort_werkzaamheden_not, team=team, team_in=team_in, team_isempty=team_isempty, team_isnull=team_isnull, team_like=team_like, team_not=team_not, uren_inzet_medewerker_inhuur=uren_inzet_medewerker_inhuur, uren_inzet_medewerker_inhuur_gt=uren_inzet_medewerker_inhuur_gt, uren_inzet_medewerker_inhuur_gte=uren_inzet_medewerker_inhuur_gte, uren_inzet_medewerker_inhuur_in=uren_inzet_medewerker_inhuur_in, uren_inzet_medewerker_inhuur_isnull=uren_inzet_medewerker_inhuur_isnull, uren_inzet_medewerker_inhuur_lt=uren_inzet_medewerker_inhuur_lt, uren_inzet_medewerker_inhuur_lte=uren_inzet_medewerker_inhuur_lte, uren_inzet_medewerker_inhuur_not=uren_inzet_medewerker_inhuur_not, uren_inzet_medewerker_intern=uren_inzet_medewerker_intern, uren_inzet_medewerker_intern_gt=uren_inzet_medewerker_intern_gt, uren_inzet_medewerker_intern_gte=uren_inzet_medewerker_intern_gte, uren_inzet_medewerker_intern_in=uren_inzet_medewerker_intern_in, uren_inzet_medewerker_intern_isnull=uren_inzet_medewerker_intern_isnull, uren_inzet_medewerker_intern_lt=uren_inzet_medewerker_intern_lt, uren_inzet_medewerker_intern_lte=uren_inzet_medewerker_intern_lte, uren_inzet_medewerker_intern_not=uren_inzet_medewerker_intern_not, uren_inzet_voertuig=uren_inzet_voertuig, uren_inzet_voertuig_gt=uren_inzet_voertuig_gt, uren_inzet_voertuig_gte=uren_inzet_voertuig_gte, uren_inzet_voertuig_in=uren_inzet_voertuig_in, uren_inzet_voertuig_isnull=uren_inzet_voertuig_isnull, uren_inzet_voertuig_lt=uren_inzet_voertuig_lt, uren_inzet_voertuig_lte=uren_inzet_voertuig_lte, uren_inzet_voertuig_not=uren_inzet_voertuig_not, voertuig_inhuur_indicatie=voertuig_inhuur_indicatie, voertuig_inhuur_indicatie_in=voertuig_inhuur_indicatie_in, voertuig_inhuur_indicatie_isempty=voertuig_inhuur_indicatie_isempty, voertuig_inhuur_indicatie_isnull=voertuig_inhuur_indicatie_isnull, voertuig_inhuur_indicatie_like=voertuig_inhuur_indicatie_like, voertuig_inhuur_indicatie_not=voertuig_inhuur_indicatie_not, werkzaamheden_code=werkzaamheden_code, werkzaamheden_code_in=werkzaamheden_code_in, werkzaamheden_code_isempty=werkzaamheden_code_isempty, werkzaamheden_code_isnull=werkzaamheden_code_isnull, werkzaamheden_code_like=werkzaamheden_code_like, werkzaamheden_code_not=werkzaamheden_code_not, werkzaamheden_datum=werkzaamheden_datum, werkzaamheden_datum_ref_id=werkzaamheden_datum_ref_id, werkzaamheden_datum_ref_id_gt=werkzaamheden_datum_ref_id_gt, werkzaamheden_datum_ref_id_gte=werkzaamheden_datum_ref_id_gte, werkzaamheden_datum_ref_id_in=werkzaamheden_datum_ref_id_in, werkzaamheden_datum_ref_id_isnull=werkzaamheden_datum_ref_id_isnull, werkzaamheden_datum_ref_id_lt=werkzaamheden_datum_ref_id_lt, werkzaamheden_datum_ref_id_lte=werkzaamheden_datum_ref_id_lte, werkzaamheden_datum_ref_id_not=werkzaamheden_datum_ref_id_not, werkzaamheden_datum_gt=werkzaamheden_datum_gt, werkzaamheden_datum_gte=werkzaamheden_datum_gte, werkzaamheden_datum_in=werkzaamheden_datum_in, werkzaamheden_datum_isnull=werkzaamheden_datum_isnull, werkzaamheden_datum_lt=werkzaamheden_datum_lt, werkzaamheden_datum_lte=werkzaamheden_datum_lte, werkzaamheden_datum_not=werkzaamheden_datum_not, werkzaamheden_eindtijd=werkzaamheden_eindtijd, werkzaamheden_eindtijd_in=werkzaamheden_eindtijd_in, werkzaamheden_eindtijd_isempty=werkzaamheden_eindtijd_isempty, werkzaamheden_eindtijd_isnull=werkzaamheden_eindtijd_isnull, werkzaamheden_eindtijd_like=werkzaamheden_eindtijd_like, werkzaamheden_eindtijd_not=werkzaamheden_eindtijd_not, werkzaamheden_omschrijving=werkzaamheden_omschrijving, werkzaamheden_omschrijving_in=werkzaamheden_omschrijving_in, werkzaamheden_omschrijving_isempty=werkzaamheden_omschrijving_isempty, werkzaamheden_omschrijving_isnull=werkzaamheden_omschrijving_isnull, werkzaamheden_omschrijving_like=werkzaamheden_omschrijving_like, werkzaamheden_omschrijving_not=werkzaamheden_omschrijving_not, werkzaamheden_starttijd=werkzaamheden_starttijd, werkzaamheden_starttijd_in=werkzaamheden_starttijd_in, werkzaamheden_starttijd_isempty=werkzaamheden_starttijd_isempty, werkzaamheden_starttijd_isnull=werkzaamheden_starttijd_isnull, werkzaamheden_starttijd_like=werkzaamheden_starttijd_like, werkzaamheden_starttijd_not=werkzaamheden_starttijd_not, werkzaamheden_uren_gepland=werkzaamheden_uren_gepland, werkzaamheden_uren_gepland_gt=werkzaamheden_uren_gepland_gt, werkzaamheden_uren_gepland_gte=werkzaamheden_uren_gepland_gte, werkzaamheden_uren_gepland_in=werkzaamheden_uren_gepland_in, werkzaamheden_uren_gepland_isnull=werkzaamheden_uren_gepland_isnull, werkzaamheden_uren_gepland_lt=werkzaamheden_uren_gepland_lt, werkzaamheden_uren_gepland_lte=werkzaamheden_uren_gepland_lte, werkzaamheden_uren_gepland_not=werkzaamheden_uren_gepland_not)

Planningsgegevens van afvalinzamelingsvoertuigen voor huishoudelijk- en bedrijfsafval

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalplanning_voertuigen_list import PaginatedHuishoudelijkafvalplanningVoertuigenList
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
    api_instance = huishoudelijkafval_api_client.PlanningVoertuigenApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'werkzaamhedenDatumRef' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    aantal_medewerkers = 3.4 # float | Aantal medewerkers dat op het voertuig is gepland. (optional)
    aantal_medewerkers_inhuur = 3.4 # float | Aantal externe medewerkers dat op het voertuig is gepland. (optional)
    aantal_medewerkers_inhuur_gt = 3.4 # float | Greater than; number (optional)
    aantal_medewerkers_inhuur_gte = 3.4 # float | Greater than or equal to; number (optional)
    aantal_medewerkers_inhuur_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_medewerkers_inhuur_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_medewerkers_inhuur_lt = 3.4 # float | Less than; number (optional)
    aantal_medewerkers_inhuur_lte = 3.4 # float | Less than or equal to; number (optional)
    aantal_medewerkers_inhuur_not = [3.4] # List[float] | Exclude matches; number (optional)
    aantal_medewerkers_intern = 3.4 # float | Aantal interne medewerkers dat op het voertuig is gepland. (optional)
    aantal_medewerkers_intern_gt = 3.4 # float | Greater than; number (optional)
    aantal_medewerkers_intern_gte = 3.4 # float | Greater than or equal to; number (optional)
    aantal_medewerkers_intern_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_medewerkers_intern_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_medewerkers_intern_lt = 3.4 # float | Less than; number (optional)
    aantal_medewerkers_intern_lte = 3.4 # float | Less than or equal to; number (optional)
    aantal_medewerkers_intern_not = [3.4] # List[float] | Exclude matches; number (optional)
    aantal_medewerkers_gt = 3.4 # float | Greater than; number (optional)
    aantal_medewerkers_gte = 3.4 # float | Greater than or equal to; number (optional)
    aantal_medewerkers_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_medewerkers_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_medewerkers_lt = 3.4 # float | Less than; number (optional)
    aantal_medewerkers_lte = 3.4 # float | Less than or equal to; number (optional)
    aantal_medewerkers_not = [3.4] # List[float] | Exclude matches; number (optional)
    activiteit = 'activiteit_example' # str | Fractie van de afvalverwerking (afgeleid van categorie, werkzaamheden en of memo). (optional)
    activiteit_in = ['activiteit_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    activiteit_isempty = True # bool | Whether the field is empty or not. (optional)
    activiteit_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    activiteit_like = 'activiteit_like_example' # str | Matches text using wildcards (? and *). (optional)
    activiteit_not = ['activiteit_not_example'] # List[str] | Exclude matches; text (optional)
    categorie = 'categorie_example' # str | Categorie afvalverwerking waar het voertuig op is gepland. (optional)
    categorie_in = ['categorie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    categorie_isempty = True # bool | Whether the field is empty or not. (optional)
    categorie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    categorie_like = 'categorie_like_example' # str | Matches text using wildcards (? and *). (optional)
    categorie_not = ['categorie_not_example'] # List[str] | Exclude matches; text (optional)
    datum_aanwezig_bron = '2013-10-20T19:20:30+01:00' # datetime | Indicatie over de actualiteit van de gegevens in deze set (laatste wijziging in de bron). (optional)
    datum_aanwezig_bron_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_aanwezig_bron_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_aanwezig_bron_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_aanwezig_bron_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_aanwezig_bron_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_aanwezig_bron_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_aanwezig_bron_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen = '2013-10-20T19:20:30+01:00' # datetime | Moment van laden data vanuit het (planningsdata)bronsysteem in het DWH stadsdelen (als intermediair voor datalevering). (optional)
    datum_verwerkt_stadsdelen_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_verwerkt_stadsdelen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_verwerkt_stadsdelen_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    fase = 'fase_example' # str | Label van de fase waarin de planning zich bevindt. (optional)
    fase_in = ['fase_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fase_isempty = True # bool | Whether the field is empty or not. (optional)
    fase_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fase_like = 'fase_like_example' # str | Matches text using wildcards (? and *). (optional)
    fase_not = ['fase_not_example'] # List[str] | Exclude matches; text (optional)
    id = 56 # int | Uniek identificerend kenmerk van het record. (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    kenteken = 'kenteken_example' # str | Kenteken afvalinzamelingsvoertuig. (optional)
    kenteken_kort = 'kenteken_kort_example' # str | Kenteken afvalinzamelingsvoertuig zonder koppeltekens (-). (optional)
    kenteken_kort_in = ['kenteken_kort_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    kenteken_kort_isempty = True # bool | Whether the field is empty or not. (optional)
    kenteken_kort_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    kenteken_kort_like = 'kenteken_kort_like_example' # str | Matches text using wildcards (? and *). (optional)
    kenteken_kort_not = ['kenteken_kort_not_example'] # List[str] | Exclude matches; text (optional)
    kenteken_in = ['kenteken_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    kenteken_isempty = True # bool | Whether the field is empty or not. (optional)
    kenteken_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    kenteken_like = 'kenteken_like_example' # str | Matches text using wildcards (? and *). (optional)
    kenteken_not = ['kenteken_not_example'] # List[str] | Exclude matches; text (optional)
    memo = 'memo_example' # str | Extra toelichting zoals opgegeven in (planningsdata)bronsysteem. (optional)
    memo_in = ['memo_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    memo_isempty = True # bool | Whether the field is empty or not. (optional)
    memo_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    memo_like = 'memo_like_example' # str | Matches text using wildcards (? and *). (optional)
    memo_not = ['memo_not_example'] # List[str] | Exclude matches; text (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    pauze_eindtijd = 'pauze_eindtijd_example' # str | Eindtijd van de pauze op de WERKZAAMHEDEN_DATUM. (optional)
    pauze_eindtijd_in = ['pauze_eindtijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    pauze_eindtijd_isempty = True # bool | Whether the field is empty or not. (optional)
    pauze_eindtijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    pauze_eindtijd_like = 'pauze_eindtijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    pauze_eindtijd_not = ['pauze_eindtijd_not_example'] # List[str] | Exclude matches; text (optional)
    pauze_starttijd = 'pauze_starttijd_example' # str | Starttijd van de pauze op de WERKZAAMHEDEN_DATUM. (optional)
    pauze_starttijd_in = ['pauze_starttijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    pauze_starttijd_isempty = True # bool | Whether the field is empty or not. (optional)
    pauze_starttijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    pauze_starttijd_like = 'pauze_starttijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    pauze_starttijd_not = ['pauze_starttijd_not_example'] # List[str] | Exclude matches; text (optional)
    pauze_uren_gepland = 3.4 # float | Berekening van het aantal bruto uren van de pauze (= eindtijd - starttijd). (optional)
    pauze_uren_gepland_gt = 3.4 # float | Greater than; number (optional)
    pauze_uren_gepland_gte = 3.4 # float | Greater than or equal to; number (optional)
    pauze_uren_gepland_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    pauze_uren_gepland_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    pauze_uren_gepland_lt = 3.4 # float | Less than; number (optional)
    pauze_uren_gepland_lte = 3.4 # float | Less than or equal to; number (optional)
    pauze_uren_gepland_not = [3.4] # List[float] | Exclude matches; number (optional)
    soort_werkzaamheden = 'soort_werkzaamheden_example' # str | Specificatie van soort planning (Inzet of Onderhoud). (optional)
    soort_werkzaamheden_in = ['soort_werkzaamheden_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_werkzaamheden_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_werkzaamheden_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_werkzaamheden_like = 'soort_werkzaamheden_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_werkzaamheden_not = ['soort_werkzaamheden_not_example'] # List[str] | Exclude matches; text (optional)
    team = 'team_example' # str | Team waarvoor de voertuigplanning is gemaakt. In veel gevallen een stadsdeel, maar kan ook bijvoorbeeld Bedrijfsafval Centrum (BAC) zijn). (optional)
    team_in = ['team_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    team_isempty = True # bool | Whether the field is empty or not. (optional)
    team_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    team_like = 'team_like_example' # str | Matches text using wildcards (? and *). (optional)
    team_not = ['team_not_example'] # List[str] | Exclude matches; text (optional)
    uren_inzet_medewerker_inhuur = 3.4 # float | Som van het totaal aantal netto uren van de externe medewerkers die op de planning zijn gezet (excl pauze). (optional)
    uren_inzet_medewerker_inhuur_gt = 3.4 # float | Greater than; number (optional)
    uren_inzet_medewerker_inhuur_gte = 3.4 # float | Greater than or equal to; number (optional)
    uren_inzet_medewerker_inhuur_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    uren_inzet_medewerker_inhuur_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    uren_inzet_medewerker_inhuur_lt = 3.4 # float | Less than; number (optional)
    uren_inzet_medewerker_inhuur_lte = 3.4 # float | Less than or equal to; number (optional)
    uren_inzet_medewerker_inhuur_not = [3.4] # List[float] | Exclude matches; number (optional)
    uren_inzet_medewerker_intern = 3.4 # float | Som van het totaal aantal netto uren van de interne medewerkers die op de planning zijn gezet (excl pauze). (optional)
    uren_inzet_medewerker_intern_gt = 3.4 # float | Greater than; number (optional)
    uren_inzet_medewerker_intern_gte = 3.4 # float | Greater than or equal to; number (optional)
    uren_inzet_medewerker_intern_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    uren_inzet_medewerker_intern_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    uren_inzet_medewerker_intern_lt = 3.4 # float | Less than; number (optional)
    uren_inzet_medewerker_intern_lte = 3.4 # float | Less than or equal to; number (optional)
    uren_inzet_medewerker_intern_not = [3.4] # List[float] | Exclude matches; number (optional)
    uren_inzet_voertuig = 3.4 # float | Netto inzeturen van het voertuig (bruto - pauze). (optional)
    uren_inzet_voertuig_gt = 3.4 # float | Greater than; number (optional)
    uren_inzet_voertuig_gte = 3.4 # float | Greater than or equal to; number (optional)
    uren_inzet_voertuig_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    uren_inzet_voertuig_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    uren_inzet_voertuig_lt = 3.4 # float | Less than; number (optional)
    uren_inzet_voertuig_lte = 3.4 # float | Less than or equal to; number (optional)
    uren_inzet_voertuig_not = [3.4] # List[float] | Exclude matches; number (optional)
    voertuig_inhuur_indicatie = 'voertuig_inhuur_indicatie_example' # str | Is het voertuig ingehuurd (Ja / Nee). (optional)
    voertuig_inhuur_indicatie_in = ['voertuig_inhuur_indicatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    voertuig_inhuur_indicatie_isempty = True # bool | Whether the field is empty or not. (optional)
    voertuig_inhuur_indicatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    voertuig_inhuur_indicatie_like = 'voertuig_inhuur_indicatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    voertuig_inhuur_indicatie_not = ['voertuig_inhuur_indicatie_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_code = 'werkzaamheden_code_example' # str | Code voor de werkzaamheden waarop het voertuig is gepland. (optional)
    werkzaamheden_code_in = ['werkzaamheden_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_code_isempty = True # bool | Whether the field is empty or not. (optional)
    werkzaamheden_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_code_like = 'werkzaamheden_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    werkzaamheden_code_not = ['werkzaamheden_code_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_datum = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop de werkzaamheden zijn gepland. (optional)
    werkzaamheden_datum_ref_id = 56 # int | Sleutelveld. Bij niveaucode dag is dit in feite de juliaanse dag. Zo kan bijvoorbeeld het verschil tussen twee datums bepaald worden door het verschil tussen de ID waarden van de datums te berekenen. De id waarden zijn zo geconstrueerd dat dit altijd kan ongeacht de waarde van niveaucode. Dus als b.v. niveaucode is 'Week' dan bevat een verschil in id waarden het aantal weken tussen de twee week records. (optional)
    werkzaamheden_datum_ref_id_gt = 56 # int | Greater than; number (optional)
    werkzaamheden_datum_ref_id_gte = 56 # int | Greater than or equal to; number (optional)
    werkzaamheden_datum_ref_id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_datum_ref_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_datum_ref_id_lt = 56 # int | Less than; number (optional)
    werkzaamheden_datum_ref_id_lte = 56 # int | Less than or equal to; number (optional)
    werkzaamheden_datum_ref_id_not = [56] # List[int] | Exclude matches; number (optional)
    werkzaamheden_datum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_datum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_datum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_datum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_datum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_datum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_datum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_eindtijd = 'werkzaamheden_eindtijd_example' # str | Eindtijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM. (optional)
    werkzaamheden_eindtijd_in = ['werkzaamheden_eindtijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_eindtijd_isempty = True # bool | Whether the field is empty or not. (optional)
    werkzaamheden_eindtijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_eindtijd_like = 'werkzaamheden_eindtijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    werkzaamheden_eindtijd_not = ['werkzaamheden_eindtijd_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_omschrijving = 'werkzaamheden_omschrijving_example' # str | Omschrijving voor de werkzaamheden waarop het voertuig is gepland. (optional)
    werkzaamheden_omschrijving_in = ['werkzaamheden_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    werkzaamheden_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_omschrijving_like = 'werkzaamheden_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    werkzaamheden_omschrijving_not = ['werkzaamheden_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_starttijd = 'werkzaamheden_starttijd_example' # str | Starttijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM (optional)
    werkzaamheden_starttijd_in = ['werkzaamheden_starttijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_starttijd_isempty = True # bool | Whether the field is empty or not. (optional)
    werkzaamheden_starttijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_starttijd_like = 'werkzaamheden_starttijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    werkzaamheden_starttijd_not = ['werkzaamheden_starttijd_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_uren_gepland = 3.4 # float | Berekening van het aantal bruto uren van de werkzaamheden (= eindtijd - starttijd). (optional)
    werkzaamheden_uren_gepland_gt = 3.4 # float | Greater than; number (optional)
    werkzaamheden_uren_gepland_gte = 3.4 # float | Greater than or equal to; number (optional)
    werkzaamheden_uren_gepland_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_uren_gepland_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_uren_gepland_lt = 3.4 # float | Less than; number (optional)
    werkzaamheden_uren_gepland_lte = 3.4 # float | Less than or equal to; number (optional)
    werkzaamheden_uren_gepland_not = [3.4] # List[float] | Exclude matches; number (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_planning_voertuigen_list_slash(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, aantal_medewerkers=aantal_medewerkers, aantal_medewerkers_inhuur=aantal_medewerkers_inhuur, aantal_medewerkers_inhuur_gt=aantal_medewerkers_inhuur_gt, aantal_medewerkers_inhuur_gte=aantal_medewerkers_inhuur_gte, aantal_medewerkers_inhuur_in=aantal_medewerkers_inhuur_in, aantal_medewerkers_inhuur_isnull=aantal_medewerkers_inhuur_isnull, aantal_medewerkers_inhuur_lt=aantal_medewerkers_inhuur_lt, aantal_medewerkers_inhuur_lte=aantal_medewerkers_inhuur_lte, aantal_medewerkers_inhuur_not=aantal_medewerkers_inhuur_not, aantal_medewerkers_intern=aantal_medewerkers_intern, aantal_medewerkers_intern_gt=aantal_medewerkers_intern_gt, aantal_medewerkers_intern_gte=aantal_medewerkers_intern_gte, aantal_medewerkers_intern_in=aantal_medewerkers_intern_in, aantal_medewerkers_intern_isnull=aantal_medewerkers_intern_isnull, aantal_medewerkers_intern_lt=aantal_medewerkers_intern_lt, aantal_medewerkers_intern_lte=aantal_medewerkers_intern_lte, aantal_medewerkers_intern_not=aantal_medewerkers_intern_not, aantal_medewerkers_gt=aantal_medewerkers_gt, aantal_medewerkers_gte=aantal_medewerkers_gte, aantal_medewerkers_in=aantal_medewerkers_in, aantal_medewerkers_isnull=aantal_medewerkers_isnull, aantal_medewerkers_lt=aantal_medewerkers_lt, aantal_medewerkers_lte=aantal_medewerkers_lte, aantal_medewerkers_not=aantal_medewerkers_not, activiteit=activiteit, activiteit_in=activiteit_in, activiteit_isempty=activiteit_isempty, activiteit_isnull=activiteit_isnull, activiteit_like=activiteit_like, activiteit_not=activiteit_not, categorie=categorie, categorie_in=categorie_in, categorie_isempty=categorie_isempty, categorie_isnull=categorie_isnull, categorie_like=categorie_like, categorie_not=categorie_not, datum_aanwezig_bron=datum_aanwezig_bron, datum_aanwezig_bron_gt=datum_aanwezig_bron_gt, datum_aanwezig_bron_gte=datum_aanwezig_bron_gte, datum_aanwezig_bron_in=datum_aanwezig_bron_in, datum_aanwezig_bron_isnull=datum_aanwezig_bron_isnull, datum_aanwezig_bron_lt=datum_aanwezig_bron_lt, datum_aanwezig_bron_lte=datum_aanwezig_bron_lte, datum_aanwezig_bron_not=datum_aanwezig_bron_not, datum_verwerkt_stadsdelen=datum_verwerkt_stadsdelen, datum_verwerkt_stadsdelen_gt=datum_verwerkt_stadsdelen_gt, datum_verwerkt_stadsdelen_gte=datum_verwerkt_stadsdelen_gte, datum_verwerkt_stadsdelen_in=datum_verwerkt_stadsdelen_in, datum_verwerkt_stadsdelen_isnull=datum_verwerkt_stadsdelen_isnull, datum_verwerkt_stadsdelen_lt=datum_verwerkt_stadsdelen_lt, datum_verwerkt_stadsdelen_lte=datum_verwerkt_stadsdelen_lte, datum_verwerkt_stadsdelen_not=datum_verwerkt_stadsdelen_not, fase=fase, fase_in=fase_in, fase_isempty=fase_isempty, fase_isnull=fase_isnull, fase_like=fase_like, fase_not=fase_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, kenteken=kenteken, kenteken_kort=kenteken_kort, kenteken_kort_in=kenteken_kort_in, kenteken_kort_isempty=kenteken_kort_isempty, kenteken_kort_isnull=kenteken_kort_isnull, kenteken_kort_like=kenteken_kort_like, kenteken_kort_not=kenteken_kort_not, kenteken_in=kenteken_in, kenteken_isempty=kenteken_isempty, kenteken_isnull=kenteken_isnull, kenteken_like=kenteken_like, kenteken_not=kenteken_not, memo=memo, memo_in=memo_in, memo_isempty=memo_isempty, memo_isnull=memo_isnull, memo_like=memo_like, memo_not=memo_not, page=page, pauze_eindtijd=pauze_eindtijd, pauze_eindtijd_in=pauze_eindtijd_in, pauze_eindtijd_isempty=pauze_eindtijd_isempty, pauze_eindtijd_isnull=pauze_eindtijd_isnull, pauze_eindtijd_like=pauze_eindtijd_like, pauze_eindtijd_not=pauze_eindtijd_not, pauze_starttijd=pauze_starttijd, pauze_starttijd_in=pauze_starttijd_in, pauze_starttijd_isempty=pauze_starttijd_isempty, pauze_starttijd_isnull=pauze_starttijd_isnull, pauze_starttijd_like=pauze_starttijd_like, pauze_starttijd_not=pauze_starttijd_not, pauze_uren_gepland=pauze_uren_gepland, pauze_uren_gepland_gt=pauze_uren_gepland_gt, pauze_uren_gepland_gte=pauze_uren_gepland_gte, pauze_uren_gepland_in=pauze_uren_gepland_in, pauze_uren_gepland_isnull=pauze_uren_gepland_isnull, pauze_uren_gepland_lt=pauze_uren_gepland_lt, pauze_uren_gepland_lte=pauze_uren_gepland_lte, pauze_uren_gepland_not=pauze_uren_gepland_not, soort_werkzaamheden=soort_werkzaamheden, soort_werkzaamheden_in=soort_werkzaamheden_in, soort_werkzaamheden_isempty=soort_werkzaamheden_isempty, soort_werkzaamheden_isnull=soort_werkzaamheden_isnull, soort_werkzaamheden_like=soort_werkzaamheden_like, soort_werkzaamheden_not=soort_werkzaamheden_not, team=team, team_in=team_in, team_isempty=team_isempty, team_isnull=team_isnull, team_like=team_like, team_not=team_not, uren_inzet_medewerker_inhuur=uren_inzet_medewerker_inhuur, uren_inzet_medewerker_inhuur_gt=uren_inzet_medewerker_inhuur_gt, uren_inzet_medewerker_inhuur_gte=uren_inzet_medewerker_inhuur_gte, uren_inzet_medewerker_inhuur_in=uren_inzet_medewerker_inhuur_in, uren_inzet_medewerker_inhuur_isnull=uren_inzet_medewerker_inhuur_isnull, uren_inzet_medewerker_inhuur_lt=uren_inzet_medewerker_inhuur_lt, uren_inzet_medewerker_inhuur_lte=uren_inzet_medewerker_inhuur_lte, uren_inzet_medewerker_inhuur_not=uren_inzet_medewerker_inhuur_not, uren_inzet_medewerker_intern=uren_inzet_medewerker_intern, uren_inzet_medewerker_intern_gt=uren_inzet_medewerker_intern_gt, uren_inzet_medewerker_intern_gte=uren_inzet_medewerker_intern_gte, uren_inzet_medewerker_intern_in=uren_inzet_medewerker_intern_in, uren_inzet_medewerker_intern_isnull=uren_inzet_medewerker_intern_isnull, uren_inzet_medewerker_intern_lt=uren_inzet_medewerker_intern_lt, uren_inzet_medewerker_intern_lte=uren_inzet_medewerker_intern_lte, uren_inzet_medewerker_intern_not=uren_inzet_medewerker_intern_not, uren_inzet_voertuig=uren_inzet_voertuig, uren_inzet_voertuig_gt=uren_inzet_voertuig_gt, uren_inzet_voertuig_gte=uren_inzet_voertuig_gte, uren_inzet_voertuig_in=uren_inzet_voertuig_in, uren_inzet_voertuig_isnull=uren_inzet_voertuig_isnull, uren_inzet_voertuig_lt=uren_inzet_voertuig_lt, uren_inzet_voertuig_lte=uren_inzet_voertuig_lte, uren_inzet_voertuig_not=uren_inzet_voertuig_not, voertuig_inhuur_indicatie=voertuig_inhuur_indicatie, voertuig_inhuur_indicatie_in=voertuig_inhuur_indicatie_in, voertuig_inhuur_indicatie_isempty=voertuig_inhuur_indicatie_isempty, voertuig_inhuur_indicatie_isnull=voertuig_inhuur_indicatie_isnull, voertuig_inhuur_indicatie_like=voertuig_inhuur_indicatie_like, voertuig_inhuur_indicatie_not=voertuig_inhuur_indicatie_not, werkzaamheden_code=werkzaamheden_code, werkzaamheden_code_in=werkzaamheden_code_in, werkzaamheden_code_isempty=werkzaamheden_code_isempty, werkzaamheden_code_isnull=werkzaamheden_code_isnull, werkzaamheden_code_like=werkzaamheden_code_like, werkzaamheden_code_not=werkzaamheden_code_not, werkzaamheden_datum=werkzaamheden_datum, werkzaamheden_datum_ref_id=werkzaamheden_datum_ref_id, werkzaamheden_datum_ref_id_gt=werkzaamheden_datum_ref_id_gt, werkzaamheden_datum_ref_id_gte=werkzaamheden_datum_ref_id_gte, werkzaamheden_datum_ref_id_in=werkzaamheden_datum_ref_id_in, werkzaamheden_datum_ref_id_isnull=werkzaamheden_datum_ref_id_isnull, werkzaamheden_datum_ref_id_lt=werkzaamheden_datum_ref_id_lt, werkzaamheden_datum_ref_id_lte=werkzaamheden_datum_ref_id_lte, werkzaamheden_datum_ref_id_not=werkzaamheden_datum_ref_id_not, werkzaamheden_datum_gt=werkzaamheden_datum_gt, werkzaamheden_datum_gte=werkzaamheden_datum_gte, werkzaamheden_datum_in=werkzaamheden_datum_in, werkzaamheden_datum_isnull=werkzaamheden_datum_isnull, werkzaamheden_datum_lt=werkzaamheden_datum_lt, werkzaamheden_datum_lte=werkzaamheden_datum_lte, werkzaamheden_datum_not=werkzaamheden_datum_not, werkzaamheden_eindtijd=werkzaamheden_eindtijd, werkzaamheden_eindtijd_in=werkzaamheden_eindtijd_in, werkzaamheden_eindtijd_isempty=werkzaamheden_eindtijd_isempty, werkzaamheden_eindtijd_isnull=werkzaamheden_eindtijd_isnull, werkzaamheden_eindtijd_like=werkzaamheden_eindtijd_like, werkzaamheden_eindtijd_not=werkzaamheden_eindtijd_not, werkzaamheden_omschrijving=werkzaamheden_omschrijving, werkzaamheden_omschrijving_in=werkzaamheden_omschrijving_in, werkzaamheden_omschrijving_isempty=werkzaamheden_omschrijving_isempty, werkzaamheden_omschrijving_isnull=werkzaamheden_omschrijving_isnull, werkzaamheden_omschrijving_like=werkzaamheden_omschrijving_like, werkzaamheden_omschrijving_not=werkzaamheden_omschrijving_not, werkzaamheden_starttijd=werkzaamheden_starttijd, werkzaamheden_starttijd_in=werkzaamheden_starttijd_in, werkzaamheden_starttijd_isempty=werkzaamheden_starttijd_isempty, werkzaamheden_starttijd_isnull=werkzaamheden_starttijd_isnull, werkzaamheden_starttijd_like=werkzaamheden_starttijd_like, werkzaamheden_starttijd_not=werkzaamheden_starttijd_not, werkzaamheden_uren_gepland=werkzaamheden_uren_gepland, werkzaamheden_uren_gepland_gt=werkzaamheden_uren_gepland_gt, werkzaamheden_uren_gepland_gte=werkzaamheden_uren_gepland_gte, werkzaamheden_uren_gepland_in=werkzaamheden_uren_gepland_in, werkzaamheden_uren_gepland_isnull=werkzaamheden_uren_gepland_isnull, werkzaamheden_uren_gepland_lt=werkzaamheden_uren_gepland_lt, werkzaamheden_uren_gepland_lte=werkzaamheden_uren_gepland_lte, werkzaamheden_uren_gepland_not=werkzaamheden_uren_gepland_not)
        print("The response of PlanningVoertuigenApi->huishoudelijkafval_planning_voertuigen_list_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PlanningVoertuigenApi->huishoudelijkafval_planning_voertuigen_list_slash: %s\n" % e)
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
 **aantal_medewerkers** | **float**| Aantal medewerkers dat op het voertuig is gepland. | [optional] 
 **aantal_medewerkers_inhuur** | **float**| Aantal externe medewerkers dat op het voertuig is gepland. | [optional] 
 **aantal_medewerkers_inhuur_gt** | **float**| Greater than; number | [optional] 
 **aantal_medewerkers_inhuur_gte** | **float**| Greater than or equal to; number | [optional] 
 **aantal_medewerkers_inhuur_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_medewerkers_inhuur_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_medewerkers_inhuur_lt** | **float**| Less than; number | [optional] 
 **aantal_medewerkers_inhuur_lte** | **float**| Less than or equal to; number | [optional] 
 **aantal_medewerkers_inhuur_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **aantal_medewerkers_intern** | **float**| Aantal interne medewerkers dat op het voertuig is gepland. | [optional] 
 **aantal_medewerkers_intern_gt** | **float**| Greater than; number | [optional] 
 **aantal_medewerkers_intern_gte** | **float**| Greater than or equal to; number | [optional] 
 **aantal_medewerkers_intern_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_medewerkers_intern_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_medewerkers_intern_lt** | **float**| Less than; number | [optional] 
 **aantal_medewerkers_intern_lte** | **float**| Less than or equal to; number | [optional] 
 **aantal_medewerkers_intern_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **aantal_medewerkers_gt** | **float**| Greater than; number | [optional] 
 **aantal_medewerkers_gte** | **float**| Greater than or equal to; number | [optional] 
 **aantal_medewerkers_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_medewerkers_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_medewerkers_lt** | **float**| Less than; number | [optional] 
 **aantal_medewerkers_lte** | **float**| Less than or equal to; number | [optional] 
 **aantal_medewerkers_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **activiteit** | **str**| Fractie van de afvalverwerking (afgeleid van categorie, werkzaamheden en of memo). | [optional] 
 **activiteit_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **activiteit_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **activiteit_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **activiteit_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **activiteit_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **categorie** | **str**| Categorie afvalverwerking waar het voertuig op is gepland. | [optional] 
 **categorie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **categorie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **categorie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **categorie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **categorie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_aanwezig_bron** | **datetime**| Indicatie over de actualiteit van de gegevens in deze set (laatste wijziging in de bron). | [optional] 
 **datum_aanwezig_bron_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_aanwezig_bron_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_aanwezig_bron_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_aanwezig_bron_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_aanwezig_bron_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_aanwezig_bron_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_aanwezig_bron_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen** | **datetime**| Moment van laden data vanuit het (planningsdata)bronsysteem in het DWH stadsdelen (als intermediair voor datalevering). | [optional] 
 **datum_verwerkt_stadsdelen_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_verwerkt_stadsdelen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_verwerkt_stadsdelen_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **fase** | **str**| Label van de fase waarin de planning zich bevindt. | [optional] 
 **fase_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fase_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fase_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fase_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fase_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id** | **int**| Uniek identificerend kenmerk van het record. | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **kenteken** | **str**| Kenteken afvalinzamelingsvoertuig. | [optional] 
 **kenteken_kort** | **str**| Kenteken afvalinzamelingsvoertuig zonder koppeltekens (-). | [optional] 
 **kenteken_kort_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **kenteken_kort_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **kenteken_kort_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **kenteken_kort_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **kenteken_kort_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **kenteken_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **kenteken_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **kenteken_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **kenteken_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **kenteken_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **memo** | **str**| Extra toelichting zoals opgegeven in (planningsdata)bronsysteem. | [optional] 
 **memo_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **memo_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **memo_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **memo_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **memo_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **pauze_eindtijd** | **str**| Eindtijd van de pauze op de WERKZAAMHEDEN_DATUM. | [optional] 
 **pauze_eindtijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **pauze_eindtijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **pauze_eindtijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **pauze_eindtijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **pauze_eindtijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **pauze_starttijd** | **str**| Starttijd van de pauze op de WERKZAAMHEDEN_DATUM. | [optional] 
 **pauze_starttijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **pauze_starttijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **pauze_starttijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **pauze_starttijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **pauze_starttijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **pauze_uren_gepland** | **float**| Berekening van het aantal bruto uren van de pauze (&#x3D; eindtijd - starttijd). | [optional] 
 **pauze_uren_gepland_gt** | **float**| Greater than; number | [optional] 
 **pauze_uren_gepland_gte** | **float**| Greater than or equal to; number | [optional] 
 **pauze_uren_gepland_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **pauze_uren_gepland_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **pauze_uren_gepland_lt** | **float**| Less than; number | [optional] 
 **pauze_uren_gepland_lte** | **float**| Less than or equal to; number | [optional] 
 **pauze_uren_gepland_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **soort_werkzaamheden** | **str**| Specificatie van soort planning (Inzet of Onderhoud). | [optional] 
 **soort_werkzaamheden_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_werkzaamheden_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_werkzaamheden_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_werkzaamheden_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_werkzaamheden_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **team** | **str**| Team waarvoor de voertuigplanning is gemaakt. In veel gevallen een stadsdeel, maar kan ook bijvoorbeeld Bedrijfsafval Centrum (BAC) zijn). | [optional] 
 **team_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **team_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **team_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **team_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **team_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **uren_inzet_medewerker_inhuur** | **float**| Som van het totaal aantal netto uren van de externe medewerkers die op de planning zijn gezet (excl pauze). | [optional] 
 **uren_inzet_medewerker_inhuur_gt** | **float**| Greater than; number | [optional] 
 **uren_inzet_medewerker_inhuur_gte** | **float**| Greater than or equal to; number | [optional] 
 **uren_inzet_medewerker_inhuur_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **uren_inzet_medewerker_inhuur_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **uren_inzet_medewerker_inhuur_lt** | **float**| Less than; number | [optional] 
 **uren_inzet_medewerker_inhuur_lte** | **float**| Less than or equal to; number | [optional] 
 **uren_inzet_medewerker_inhuur_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **uren_inzet_medewerker_intern** | **float**| Som van het totaal aantal netto uren van de interne medewerkers die op de planning zijn gezet (excl pauze). | [optional] 
 **uren_inzet_medewerker_intern_gt** | **float**| Greater than; number | [optional] 
 **uren_inzet_medewerker_intern_gte** | **float**| Greater than or equal to; number | [optional] 
 **uren_inzet_medewerker_intern_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **uren_inzet_medewerker_intern_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **uren_inzet_medewerker_intern_lt** | **float**| Less than; number | [optional] 
 **uren_inzet_medewerker_intern_lte** | **float**| Less than or equal to; number | [optional] 
 **uren_inzet_medewerker_intern_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **uren_inzet_voertuig** | **float**| Netto inzeturen van het voertuig (bruto - pauze). | [optional] 
 **uren_inzet_voertuig_gt** | **float**| Greater than; number | [optional] 
 **uren_inzet_voertuig_gte** | **float**| Greater than or equal to; number | [optional] 
 **uren_inzet_voertuig_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **uren_inzet_voertuig_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **uren_inzet_voertuig_lt** | **float**| Less than; number | [optional] 
 **uren_inzet_voertuig_lte** | **float**| Less than or equal to; number | [optional] 
 **uren_inzet_voertuig_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **voertuig_inhuur_indicatie** | **str**| Is het voertuig ingehuurd (Ja / Nee). | [optional] 
 **voertuig_inhuur_indicatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **voertuig_inhuur_indicatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **voertuig_inhuur_indicatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **voertuig_inhuur_indicatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **voertuig_inhuur_indicatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_code** | **str**| Code voor de werkzaamheden waarop het voertuig is gepland. | [optional] 
 **werkzaamheden_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **werkzaamheden_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **werkzaamheden_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_datum** | **datetime**| Datum waarop de werkzaamheden zijn gepland. | [optional] 
 **werkzaamheden_datum_ref_id** | **int**| Sleutelveld. Bij niveaucode dag is dit in feite de juliaanse dag. Zo kan bijvoorbeeld het verschil tussen twee datums bepaald worden door het verschil tussen de ID waarden van de datums te berekenen. De id waarden zijn zo geconstrueerd dat dit altijd kan ongeacht de waarde van niveaucode. Dus als b.v. niveaucode is &#39;Week&#39; dan bevat een verschil in id waarden het aantal weken tussen de twee week records. | [optional] 
 **werkzaamheden_datum_ref_id_gt** | **int**| Greater than; number | [optional] 
 **werkzaamheden_datum_ref_id_gte** | **int**| Greater than or equal to; number | [optional] 
 **werkzaamheden_datum_ref_id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_datum_ref_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_datum_ref_id_lt** | **int**| Less than; number | [optional] 
 **werkzaamheden_datum_ref_id_lte** | **int**| Less than or equal to; number | [optional] 
 **werkzaamheden_datum_ref_id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **werkzaamheden_datum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_datum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_datum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_datum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_datum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_datum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_datum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_eindtijd** | **str**| Eindtijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM. | [optional] 
 **werkzaamheden_eindtijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_eindtijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **werkzaamheden_eindtijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_eindtijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **werkzaamheden_eindtijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_omschrijving** | **str**| Omschrijving voor de werkzaamheden waarop het voertuig is gepland. | [optional] 
 **werkzaamheden_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **werkzaamheden_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **werkzaamheden_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_starttijd** | **str**| Starttijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM | [optional] 
 **werkzaamheden_starttijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_starttijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **werkzaamheden_starttijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_starttijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **werkzaamheden_starttijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_uren_gepland** | **float**| Berekening van het aantal bruto uren van de werkzaamheden (&#x3D; eindtijd - starttijd). | [optional] 
 **werkzaamheden_uren_gepland_gt** | **float**| Greater than; number | [optional] 
 **werkzaamheden_uren_gepland_gte** | **float**| Greater than or equal to; number | [optional] 
 **werkzaamheden_uren_gepland_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_uren_gepland_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_uren_gepland_lt** | **float**| Less than; number | [optional] 
 **werkzaamheden_uren_gepland_lte** | **float**| Less than or equal to; number | [optional] 
 **werkzaamheden_uren_gepland_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalplanningVoertuigenList**](PaginatedHuishoudelijkafvalplanningVoertuigenList.md)

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

# **huishoudelijkafval_planning_voertuigen_retrieve_slash**
> HuishoudelijkafvalplanningVoertuigen huishoudelijkafval_planning_voertuigen_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aantal_medewerkers=aantal_medewerkers, aantal_medewerkers_inhuur=aantal_medewerkers_inhuur, aantal_medewerkers_inhuur_gt=aantal_medewerkers_inhuur_gt, aantal_medewerkers_inhuur_gte=aantal_medewerkers_inhuur_gte, aantal_medewerkers_inhuur_in=aantal_medewerkers_inhuur_in, aantal_medewerkers_inhuur_isnull=aantal_medewerkers_inhuur_isnull, aantal_medewerkers_inhuur_lt=aantal_medewerkers_inhuur_lt, aantal_medewerkers_inhuur_lte=aantal_medewerkers_inhuur_lte, aantal_medewerkers_inhuur_not=aantal_medewerkers_inhuur_not, aantal_medewerkers_intern=aantal_medewerkers_intern, aantal_medewerkers_intern_gt=aantal_medewerkers_intern_gt, aantal_medewerkers_intern_gte=aantal_medewerkers_intern_gte, aantal_medewerkers_intern_in=aantal_medewerkers_intern_in, aantal_medewerkers_intern_isnull=aantal_medewerkers_intern_isnull, aantal_medewerkers_intern_lt=aantal_medewerkers_intern_lt, aantal_medewerkers_intern_lte=aantal_medewerkers_intern_lte, aantal_medewerkers_intern_not=aantal_medewerkers_intern_not, aantal_medewerkers_gt=aantal_medewerkers_gt, aantal_medewerkers_gte=aantal_medewerkers_gte, aantal_medewerkers_in=aantal_medewerkers_in, aantal_medewerkers_isnull=aantal_medewerkers_isnull, aantal_medewerkers_lt=aantal_medewerkers_lt, aantal_medewerkers_lte=aantal_medewerkers_lte, aantal_medewerkers_not=aantal_medewerkers_not, activiteit=activiteit, activiteit_in=activiteit_in, activiteit_isempty=activiteit_isempty, activiteit_isnull=activiteit_isnull, activiteit_like=activiteit_like, activiteit_not=activiteit_not, categorie=categorie, categorie_in=categorie_in, categorie_isempty=categorie_isempty, categorie_isnull=categorie_isnull, categorie_like=categorie_like, categorie_not=categorie_not, datum_aanwezig_bron=datum_aanwezig_bron, datum_aanwezig_bron_gt=datum_aanwezig_bron_gt, datum_aanwezig_bron_gte=datum_aanwezig_bron_gte, datum_aanwezig_bron_in=datum_aanwezig_bron_in, datum_aanwezig_bron_isnull=datum_aanwezig_bron_isnull, datum_aanwezig_bron_lt=datum_aanwezig_bron_lt, datum_aanwezig_bron_lte=datum_aanwezig_bron_lte, datum_aanwezig_bron_not=datum_aanwezig_bron_not, datum_verwerkt_stadsdelen=datum_verwerkt_stadsdelen, datum_verwerkt_stadsdelen_gt=datum_verwerkt_stadsdelen_gt, datum_verwerkt_stadsdelen_gte=datum_verwerkt_stadsdelen_gte, datum_verwerkt_stadsdelen_in=datum_verwerkt_stadsdelen_in, datum_verwerkt_stadsdelen_isnull=datum_verwerkt_stadsdelen_isnull, datum_verwerkt_stadsdelen_lt=datum_verwerkt_stadsdelen_lt, datum_verwerkt_stadsdelen_lte=datum_verwerkt_stadsdelen_lte, datum_verwerkt_stadsdelen_not=datum_verwerkt_stadsdelen_not, fase=fase, fase_in=fase_in, fase_isempty=fase_isempty, fase_isnull=fase_isnull, fase_like=fase_like, fase_not=fase_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, kenteken=kenteken, kenteken_kort=kenteken_kort, kenteken_kort_in=kenteken_kort_in, kenteken_kort_isempty=kenteken_kort_isempty, kenteken_kort_isnull=kenteken_kort_isnull, kenteken_kort_like=kenteken_kort_like, kenteken_kort_not=kenteken_kort_not, kenteken_in=kenteken_in, kenteken_isempty=kenteken_isempty, kenteken_isnull=kenteken_isnull, kenteken_like=kenteken_like, kenteken_not=kenteken_not, memo=memo, memo_in=memo_in, memo_isempty=memo_isempty, memo_isnull=memo_isnull, memo_like=memo_like, memo_not=memo_not, pauze_eindtijd=pauze_eindtijd, pauze_eindtijd_in=pauze_eindtijd_in, pauze_eindtijd_isempty=pauze_eindtijd_isempty, pauze_eindtijd_isnull=pauze_eindtijd_isnull, pauze_eindtijd_like=pauze_eindtijd_like, pauze_eindtijd_not=pauze_eindtijd_not, pauze_starttijd=pauze_starttijd, pauze_starttijd_in=pauze_starttijd_in, pauze_starttijd_isempty=pauze_starttijd_isempty, pauze_starttijd_isnull=pauze_starttijd_isnull, pauze_starttijd_like=pauze_starttijd_like, pauze_starttijd_not=pauze_starttijd_not, pauze_uren_gepland=pauze_uren_gepland, pauze_uren_gepland_gt=pauze_uren_gepland_gt, pauze_uren_gepland_gte=pauze_uren_gepland_gte, pauze_uren_gepland_in=pauze_uren_gepland_in, pauze_uren_gepland_isnull=pauze_uren_gepland_isnull, pauze_uren_gepland_lt=pauze_uren_gepland_lt, pauze_uren_gepland_lte=pauze_uren_gepland_lte, pauze_uren_gepland_not=pauze_uren_gepland_not, soort_werkzaamheden=soort_werkzaamheden, soort_werkzaamheden_in=soort_werkzaamheden_in, soort_werkzaamheden_isempty=soort_werkzaamheden_isempty, soort_werkzaamheden_isnull=soort_werkzaamheden_isnull, soort_werkzaamheden_like=soort_werkzaamheden_like, soort_werkzaamheden_not=soort_werkzaamheden_not, team=team, team_in=team_in, team_isempty=team_isempty, team_isnull=team_isnull, team_like=team_like, team_not=team_not, uren_inzet_medewerker_inhuur=uren_inzet_medewerker_inhuur, uren_inzet_medewerker_inhuur_gt=uren_inzet_medewerker_inhuur_gt, uren_inzet_medewerker_inhuur_gte=uren_inzet_medewerker_inhuur_gte, uren_inzet_medewerker_inhuur_in=uren_inzet_medewerker_inhuur_in, uren_inzet_medewerker_inhuur_isnull=uren_inzet_medewerker_inhuur_isnull, uren_inzet_medewerker_inhuur_lt=uren_inzet_medewerker_inhuur_lt, uren_inzet_medewerker_inhuur_lte=uren_inzet_medewerker_inhuur_lte, uren_inzet_medewerker_inhuur_not=uren_inzet_medewerker_inhuur_not, uren_inzet_medewerker_intern=uren_inzet_medewerker_intern, uren_inzet_medewerker_intern_gt=uren_inzet_medewerker_intern_gt, uren_inzet_medewerker_intern_gte=uren_inzet_medewerker_intern_gte, uren_inzet_medewerker_intern_in=uren_inzet_medewerker_intern_in, uren_inzet_medewerker_intern_isnull=uren_inzet_medewerker_intern_isnull, uren_inzet_medewerker_intern_lt=uren_inzet_medewerker_intern_lt, uren_inzet_medewerker_intern_lte=uren_inzet_medewerker_intern_lte, uren_inzet_medewerker_intern_not=uren_inzet_medewerker_intern_not, uren_inzet_voertuig=uren_inzet_voertuig, uren_inzet_voertuig_gt=uren_inzet_voertuig_gt, uren_inzet_voertuig_gte=uren_inzet_voertuig_gte, uren_inzet_voertuig_in=uren_inzet_voertuig_in, uren_inzet_voertuig_isnull=uren_inzet_voertuig_isnull, uren_inzet_voertuig_lt=uren_inzet_voertuig_lt, uren_inzet_voertuig_lte=uren_inzet_voertuig_lte, uren_inzet_voertuig_not=uren_inzet_voertuig_not, voertuig_inhuur_indicatie=voertuig_inhuur_indicatie, voertuig_inhuur_indicatie_in=voertuig_inhuur_indicatie_in, voertuig_inhuur_indicatie_isempty=voertuig_inhuur_indicatie_isempty, voertuig_inhuur_indicatie_isnull=voertuig_inhuur_indicatie_isnull, voertuig_inhuur_indicatie_like=voertuig_inhuur_indicatie_like, voertuig_inhuur_indicatie_not=voertuig_inhuur_indicatie_not, werkzaamheden_code=werkzaamheden_code, werkzaamheden_code_in=werkzaamheden_code_in, werkzaamheden_code_isempty=werkzaamheden_code_isempty, werkzaamheden_code_isnull=werkzaamheden_code_isnull, werkzaamheden_code_like=werkzaamheden_code_like, werkzaamheden_code_not=werkzaamheden_code_not, werkzaamheden_datum=werkzaamheden_datum, werkzaamheden_datum_ref_id=werkzaamheden_datum_ref_id, werkzaamheden_datum_ref_id_gt=werkzaamheden_datum_ref_id_gt, werkzaamheden_datum_ref_id_gte=werkzaamheden_datum_ref_id_gte, werkzaamheden_datum_ref_id_in=werkzaamheden_datum_ref_id_in, werkzaamheden_datum_ref_id_isnull=werkzaamheden_datum_ref_id_isnull, werkzaamheden_datum_ref_id_lt=werkzaamheden_datum_ref_id_lt, werkzaamheden_datum_ref_id_lte=werkzaamheden_datum_ref_id_lte, werkzaamheden_datum_ref_id_not=werkzaamheden_datum_ref_id_not, werkzaamheden_datum_gt=werkzaamheden_datum_gt, werkzaamheden_datum_gte=werkzaamheden_datum_gte, werkzaamheden_datum_in=werkzaamheden_datum_in, werkzaamheden_datum_isnull=werkzaamheden_datum_isnull, werkzaamheden_datum_lt=werkzaamheden_datum_lt, werkzaamheden_datum_lte=werkzaamheden_datum_lte, werkzaamheden_datum_not=werkzaamheden_datum_not, werkzaamheden_eindtijd=werkzaamheden_eindtijd, werkzaamheden_eindtijd_in=werkzaamheden_eindtijd_in, werkzaamheden_eindtijd_isempty=werkzaamheden_eindtijd_isempty, werkzaamheden_eindtijd_isnull=werkzaamheden_eindtijd_isnull, werkzaamheden_eindtijd_like=werkzaamheden_eindtijd_like, werkzaamheden_eindtijd_not=werkzaamheden_eindtijd_not, werkzaamheden_omschrijving=werkzaamheden_omschrijving, werkzaamheden_omschrijving_in=werkzaamheden_omschrijving_in, werkzaamheden_omschrijving_isempty=werkzaamheden_omschrijving_isempty, werkzaamheden_omschrijving_isnull=werkzaamheden_omschrijving_isnull, werkzaamheden_omschrijving_like=werkzaamheden_omschrijving_like, werkzaamheden_omschrijving_not=werkzaamheden_omschrijving_not, werkzaamheden_starttijd=werkzaamheden_starttijd, werkzaamheden_starttijd_in=werkzaamheden_starttijd_in, werkzaamheden_starttijd_isempty=werkzaamheden_starttijd_isempty, werkzaamheden_starttijd_isnull=werkzaamheden_starttijd_isnull, werkzaamheden_starttijd_like=werkzaamheden_starttijd_like, werkzaamheden_starttijd_not=werkzaamheden_starttijd_not, werkzaamheden_uren_gepland=werkzaamheden_uren_gepland, werkzaamheden_uren_gepland_gt=werkzaamheden_uren_gepland_gt, werkzaamheden_uren_gepland_gte=werkzaamheden_uren_gepland_gte, werkzaamheden_uren_gepland_in=werkzaamheden_uren_gepland_in, werkzaamheden_uren_gepland_isnull=werkzaamheden_uren_gepland_isnull, werkzaamheden_uren_gepland_lt=werkzaamheden_uren_gepland_lt, werkzaamheden_uren_gepland_lte=werkzaamheden_uren_gepland_lte, werkzaamheden_uren_gepland_not=werkzaamheden_uren_gepland_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalplanning_voertuigen import HuishoudelijkafvalplanningVoertuigen
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
    api_instance = huishoudelijkafval_api_client.PlanningVoertuigenApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    csv_header = 'csv_header_example' # str | Specify type of header for csv file (optional)
    csv_separator = 'csv_separator_example' # str | Specify type of separator for csv file (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'werkzaamhedenDatumRef' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    aantal_medewerkers = 3.4 # float | Aantal medewerkers dat op het voertuig is gepland. (optional)
    aantal_medewerkers_inhuur = 3.4 # float | Aantal externe medewerkers dat op het voertuig is gepland. (optional)
    aantal_medewerkers_inhuur_gt = 3.4 # float | Greater than; number (optional)
    aantal_medewerkers_inhuur_gte = 3.4 # float | Greater than or equal to; number (optional)
    aantal_medewerkers_inhuur_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_medewerkers_inhuur_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_medewerkers_inhuur_lt = 3.4 # float | Less than; number (optional)
    aantal_medewerkers_inhuur_lte = 3.4 # float | Less than or equal to; number (optional)
    aantal_medewerkers_inhuur_not = [3.4] # List[float] | Exclude matches; number (optional)
    aantal_medewerkers_intern = 3.4 # float | Aantal interne medewerkers dat op het voertuig is gepland. (optional)
    aantal_medewerkers_intern_gt = 3.4 # float | Greater than; number (optional)
    aantal_medewerkers_intern_gte = 3.4 # float | Greater than or equal to; number (optional)
    aantal_medewerkers_intern_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_medewerkers_intern_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_medewerkers_intern_lt = 3.4 # float | Less than; number (optional)
    aantal_medewerkers_intern_lte = 3.4 # float | Less than or equal to; number (optional)
    aantal_medewerkers_intern_not = [3.4] # List[float] | Exclude matches; number (optional)
    aantal_medewerkers_gt = 3.4 # float | Greater than; number (optional)
    aantal_medewerkers_gte = 3.4 # float | Greater than or equal to; number (optional)
    aantal_medewerkers_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    aantal_medewerkers_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    aantal_medewerkers_lt = 3.4 # float | Less than; number (optional)
    aantal_medewerkers_lte = 3.4 # float | Less than or equal to; number (optional)
    aantal_medewerkers_not = [3.4] # List[float] | Exclude matches; number (optional)
    activiteit = 'activiteit_example' # str | Fractie van de afvalverwerking (afgeleid van categorie, werkzaamheden en of memo). (optional)
    activiteit_in = ['activiteit_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    activiteit_isempty = True # bool | Whether the field is empty or not. (optional)
    activiteit_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    activiteit_like = 'activiteit_like_example' # str | Matches text using wildcards (? and *). (optional)
    activiteit_not = ['activiteit_not_example'] # List[str] | Exclude matches; text (optional)
    categorie = 'categorie_example' # str | Categorie afvalverwerking waar het voertuig op is gepland. (optional)
    categorie_in = ['categorie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    categorie_isempty = True # bool | Whether the field is empty or not. (optional)
    categorie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    categorie_like = 'categorie_like_example' # str | Matches text using wildcards (? and *). (optional)
    categorie_not = ['categorie_not_example'] # List[str] | Exclude matches; text (optional)
    datum_aanwezig_bron = '2013-10-20T19:20:30+01:00' # datetime | Indicatie over de actualiteit van de gegevens in deze set (laatste wijziging in de bron). (optional)
    datum_aanwezig_bron_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_aanwezig_bron_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_aanwezig_bron_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_aanwezig_bron_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_aanwezig_bron_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_aanwezig_bron_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_aanwezig_bron_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen = '2013-10-20T19:20:30+01:00' # datetime | Moment van laden data vanuit het (planningsdata)bronsysteem in het DWH stadsdelen (als intermediair voor datalevering). (optional)
    datum_verwerkt_stadsdelen_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_verwerkt_stadsdelen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_verwerkt_stadsdelen_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_verwerkt_stadsdelen_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    fase = 'fase_example' # str | Label van de fase waarin de planning zich bevindt. (optional)
    fase_in = ['fase_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    fase_isempty = True # bool | Whether the field is empty or not. (optional)
    fase_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    fase_like = 'fase_like_example' # str | Matches text using wildcards (? and *). (optional)
    fase_not = ['fase_not_example'] # List[str] | Exclude matches; text (optional)
    id2 = 56 # int | Uniek identificerend kenmerk van het record. (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    kenteken = 'kenteken_example' # str | Kenteken afvalinzamelingsvoertuig. (optional)
    kenteken_kort = 'kenteken_kort_example' # str | Kenteken afvalinzamelingsvoertuig zonder koppeltekens (-). (optional)
    kenteken_kort_in = ['kenteken_kort_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    kenteken_kort_isempty = True # bool | Whether the field is empty or not. (optional)
    kenteken_kort_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    kenteken_kort_like = 'kenteken_kort_like_example' # str | Matches text using wildcards (? and *). (optional)
    kenteken_kort_not = ['kenteken_kort_not_example'] # List[str] | Exclude matches; text (optional)
    kenteken_in = ['kenteken_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    kenteken_isempty = True # bool | Whether the field is empty or not. (optional)
    kenteken_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    kenteken_like = 'kenteken_like_example' # str | Matches text using wildcards (? and *). (optional)
    kenteken_not = ['kenteken_not_example'] # List[str] | Exclude matches; text (optional)
    memo = 'memo_example' # str | Extra toelichting zoals opgegeven in (planningsdata)bronsysteem. (optional)
    memo_in = ['memo_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    memo_isempty = True # bool | Whether the field is empty or not. (optional)
    memo_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    memo_like = 'memo_like_example' # str | Matches text using wildcards (? and *). (optional)
    memo_not = ['memo_not_example'] # List[str] | Exclude matches; text (optional)
    pauze_eindtijd = 'pauze_eindtijd_example' # str | Eindtijd van de pauze op de WERKZAAMHEDEN_DATUM. (optional)
    pauze_eindtijd_in = ['pauze_eindtijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    pauze_eindtijd_isempty = True # bool | Whether the field is empty or not. (optional)
    pauze_eindtijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    pauze_eindtijd_like = 'pauze_eindtijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    pauze_eindtijd_not = ['pauze_eindtijd_not_example'] # List[str] | Exclude matches; text (optional)
    pauze_starttijd = 'pauze_starttijd_example' # str | Starttijd van de pauze op de WERKZAAMHEDEN_DATUM. (optional)
    pauze_starttijd_in = ['pauze_starttijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    pauze_starttijd_isempty = True # bool | Whether the field is empty or not. (optional)
    pauze_starttijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    pauze_starttijd_like = 'pauze_starttijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    pauze_starttijd_not = ['pauze_starttijd_not_example'] # List[str] | Exclude matches; text (optional)
    pauze_uren_gepland = 3.4 # float | Berekening van het aantal bruto uren van de pauze (= eindtijd - starttijd). (optional)
    pauze_uren_gepland_gt = 3.4 # float | Greater than; number (optional)
    pauze_uren_gepland_gte = 3.4 # float | Greater than or equal to; number (optional)
    pauze_uren_gepland_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    pauze_uren_gepland_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    pauze_uren_gepland_lt = 3.4 # float | Less than; number (optional)
    pauze_uren_gepland_lte = 3.4 # float | Less than or equal to; number (optional)
    pauze_uren_gepland_not = [3.4] # List[float] | Exclude matches; number (optional)
    soort_werkzaamheden = 'soort_werkzaamheden_example' # str | Specificatie van soort planning (Inzet of Onderhoud). (optional)
    soort_werkzaamheden_in = ['soort_werkzaamheden_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    soort_werkzaamheden_isempty = True # bool | Whether the field is empty or not. (optional)
    soort_werkzaamheden_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    soort_werkzaamheden_like = 'soort_werkzaamheden_like_example' # str | Matches text using wildcards (? and *). (optional)
    soort_werkzaamheden_not = ['soort_werkzaamheden_not_example'] # List[str] | Exclude matches; text (optional)
    team = 'team_example' # str | Team waarvoor de voertuigplanning is gemaakt. In veel gevallen een stadsdeel, maar kan ook bijvoorbeeld Bedrijfsafval Centrum (BAC) zijn). (optional)
    team_in = ['team_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    team_isempty = True # bool | Whether the field is empty or not. (optional)
    team_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    team_like = 'team_like_example' # str | Matches text using wildcards (? and *). (optional)
    team_not = ['team_not_example'] # List[str] | Exclude matches; text (optional)
    uren_inzet_medewerker_inhuur = 3.4 # float | Som van het totaal aantal netto uren van de externe medewerkers die op de planning zijn gezet (excl pauze). (optional)
    uren_inzet_medewerker_inhuur_gt = 3.4 # float | Greater than; number (optional)
    uren_inzet_medewerker_inhuur_gte = 3.4 # float | Greater than or equal to; number (optional)
    uren_inzet_medewerker_inhuur_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    uren_inzet_medewerker_inhuur_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    uren_inzet_medewerker_inhuur_lt = 3.4 # float | Less than; number (optional)
    uren_inzet_medewerker_inhuur_lte = 3.4 # float | Less than or equal to; number (optional)
    uren_inzet_medewerker_inhuur_not = [3.4] # List[float] | Exclude matches; number (optional)
    uren_inzet_medewerker_intern = 3.4 # float | Som van het totaal aantal netto uren van de interne medewerkers die op de planning zijn gezet (excl pauze). (optional)
    uren_inzet_medewerker_intern_gt = 3.4 # float | Greater than; number (optional)
    uren_inzet_medewerker_intern_gte = 3.4 # float | Greater than or equal to; number (optional)
    uren_inzet_medewerker_intern_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    uren_inzet_medewerker_intern_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    uren_inzet_medewerker_intern_lt = 3.4 # float | Less than; number (optional)
    uren_inzet_medewerker_intern_lte = 3.4 # float | Less than or equal to; number (optional)
    uren_inzet_medewerker_intern_not = [3.4] # List[float] | Exclude matches; number (optional)
    uren_inzet_voertuig = 3.4 # float | Netto inzeturen van het voertuig (bruto - pauze). (optional)
    uren_inzet_voertuig_gt = 3.4 # float | Greater than; number (optional)
    uren_inzet_voertuig_gte = 3.4 # float | Greater than or equal to; number (optional)
    uren_inzet_voertuig_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    uren_inzet_voertuig_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    uren_inzet_voertuig_lt = 3.4 # float | Less than; number (optional)
    uren_inzet_voertuig_lte = 3.4 # float | Less than or equal to; number (optional)
    uren_inzet_voertuig_not = [3.4] # List[float] | Exclude matches; number (optional)
    voertuig_inhuur_indicatie = 'voertuig_inhuur_indicatie_example' # str | Is het voertuig ingehuurd (Ja / Nee). (optional)
    voertuig_inhuur_indicatie_in = ['voertuig_inhuur_indicatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    voertuig_inhuur_indicatie_isempty = True # bool | Whether the field is empty or not. (optional)
    voertuig_inhuur_indicatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    voertuig_inhuur_indicatie_like = 'voertuig_inhuur_indicatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    voertuig_inhuur_indicatie_not = ['voertuig_inhuur_indicatie_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_code = 'werkzaamheden_code_example' # str | Code voor de werkzaamheden waarop het voertuig is gepland. (optional)
    werkzaamheden_code_in = ['werkzaamheden_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_code_isempty = True # bool | Whether the field is empty or not. (optional)
    werkzaamheden_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_code_like = 'werkzaamheden_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    werkzaamheden_code_not = ['werkzaamheden_code_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_datum = '2013-10-20T19:20:30+01:00' # datetime | Datum waarop de werkzaamheden zijn gepland. (optional)
    werkzaamheden_datum_ref_id = 56 # int | Sleutelveld. Bij niveaucode dag is dit in feite de juliaanse dag. Zo kan bijvoorbeeld het verschil tussen twee datums bepaald worden door het verschil tussen de ID waarden van de datums te berekenen. De id waarden zijn zo geconstrueerd dat dit altijd kan ongeacht de waarde van niveaucode. Dus als b.v. niveaucode is 'Week' dan bevat een verschil in id waarden het aantal weken tussen de twee week records. (optional)
    werkzaamheden_datum_ref_id_gt = 56 # int | Greater than; number (optional)
    werkzaamheden_datum_ref_id_gte = 56 # int | Greater than or equal to; number (optional)
    werkzaamheden_datum_ref_id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_datum_ref_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_datum_ref_id_lt = 56 # int | Less than; number (optional)
    werkzaamheden_datum_ref_id_lte = 56 # int | Less than or equal to; number (optional)
    werkzaamheden_datum_ref_id_not = [56] # List[int] | Exclude matches; number (optional)
    werkzaamheden_datum_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_datum_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_datum_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_datum_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_datum_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_datum_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_datum_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    werkzaamheden_eindtijd = 'werkzaamheden_eindtijd_example' # str | Eindtijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM. (optional)
    werkzaamheden_eindtijd_in = ['werkzaamheden_eindtijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_eindtijd_isempty = True # bool | Whether the field is empty or not. (optional)
    werkzaamheden_eindtijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_eindtijd_like = 'werkzaamheden_eindtijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    werkzaamheden_eindtijd_not = ['werkzaamheden_eindtijd_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_omschrijving = 'werkzaamheden_omschrijving_example' # str | Omschrijving voor de werkzaamheden waarop het voertuig is gepland. (optional)
    werkzaamheden_omschrijving_in = ['werkzaamheden_omschrijving_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_omschrijving_isempty = True # bool | Whether the field is empty or not. (optional)
    werkzaamheden_omschrijving_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_omschrijving_like = 'werkzaamheden_omschrijving_like_example' # str | Matches text using wildcards (? and *). (optional)
    werkzaamheden_omschrijving_not = ['werkzaamheden_omschrijving_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_starttijd = 'werkzaamheden_starttijd_example' # str | Starttijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM (optional)
    werkzaamheden_starttijd_in = ['werkzaamheden_starttijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_starttijd_isempty = True # bool | Whether the field is empty or not. (optional)
    werkzaamheden_starttijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_starttijd_like = 'werkzaamheden_starttijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    werkzaamheden_starttijd_not = ['werkzaamheden_starttijd_not_example'] # List[str] | Exclude matches; text (optional)
    werkzaamheden_uren_gepland = 3.4 # float | Berekening van het aantal bruto uren van de werkzaamheden (= eindtijd - starttijd). (optional)
    werkzaamheden_uren_gepland_gt = 3.4 # float | Greater than; number (optional)
    werkzaamheden_uren_gepland_gte = 3.4 # float | Greater than or equal to; number (optional)
    werkzaamheden_uren_gepland_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    werkzaamheden_uren_gepland_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    werkzaamheden_uren_gepland_lt = 3.4 # float | Less than; number (optional)
    werkzaamheden_uren_gepland_lte = 3.4 # float | Less than or equal to; number (optional)
    werkzaamheden_uren_gepland_not = [3.4] # List[float] | Exclude matches; number (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_planning_voertuigen_retrieve_slash(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, csv_header=csv_header, csv_separator=csv_separator, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, aantal_medewerkers=aantal_medewerkers, aantal_medewerkers_inhuur=aantal_medewerkers_inhuur, aantal_medewerkers_inhuur_gt=aantal_medewerkers_inhuur_gt, aantal_medewerkers_inhuur_gte=aantal_medewerkers_inhuur_gte, aantal_medewerkers_inhuur_in=aantal_medewerkers_inhuur_in, aantal_medewerkers_inhuur_isnull=aantal_medewerkers_inhuur_isnull, aantal_medewerkers_inhuur_lt=aantal_medewerkers_inhuur_lt, aantal_medewerkers_inhuur_lte=aantal_medewerkers_inhuur_lte, aantal_medewerkers_inhuur_not=aantal_medewerkers_inhuur_not, aantal_medewerkers_intern=aantal_medewerkers_intern, aantal_medewerkers_intern_gt=aantal_medewerkers_intern_gt, aantal_medewerkers_intern_gte=aantal_medewerkers_intern_gte, aantal_medewerkers_intern_in=aantal_medewerkers_intern_in, aantal_medewerkers_intern_isnull=aantal_medewerkers_intern_isnull, aantal_medewerkers_intern_lt=aantal_medewerkers_intern_lt, aantal_medewerkers_intern_lte=aantal_medewerkers_intern_lte, aantal_medewerkers_intern_not=aantal_medewerkers_intern_not, aantal_medewerkers_gt=aantal_medewerkers_gt, aantal_medewerkers_gte=aantal_medewerkers_gte, aantal_medewerkers_in=aantal_medewerkers_in, aantal_medewerkers_isnull=aantal_medewerkers_isnull, aantal_medewerkers_lt=aantal_medewerkers_lt, aantal_medewerkers_lte=aantal_medewerkers_lte, aantal_medewerkers_not=aantal_medewerkers_not, activiteit=activiteit, activiteit_in=activiteit_in, activiteit_isempty=activiteit_isempty, activiteit_isnull=activiteit_isnull, activiteit_like=activiteit_like, activiteit_not=activiteit_not, categorie=categorie, categorie_in=categorie_in, categorie_isempty=categorie_isempty, categorie_isnull=categorie_isnull, categorie_like=categorie_like, categorie_not=categorie_not, datum_aanwezig_bron=datum_aanwezig_bron, datum_aanwezig_bron_gt=datum_aanwezig_bron_gt, datum_aanwezig_bron_gte=datum_aanwezig_bron_gte, datum_aanwezig_bron_in=datum_aanwezig_bron_in, datum_aanwezig_bron_isnull=datum_aanwezig_bron_isnull, datum_aanwezig_bron_lt=datum_aanwezig_bron_lt, datum_aanwezig_bron_lte=datum_aanwezig_bron_lte, datum_aanwezig_bron_not=datum_aanwezig_bron_not, datum_verwerkt_stadsdelen=datum_verwerkt_stadsdelen, datum_verwerkt_stadsdelen_gt=datum_verwerkt_stadsdelen_gt, datum_verwerkt_stadsdelen_gte=datum_verwerkt_stadsdelen_gte, datum_verwerkt_stadsdelen_in=datum_verwerkt_stadsdelen_in, datum_verwerkt_stadsdelen_isnull=datum_verwerkt_stadsdelen_isnull, datum_verwerkt_stadsdelen_lt=datum_verwerkt_stadsdelen_lt, datum_verwerkt_stadsdelen_lte=datum_verwerkt_stadsdelen_lte, datum_verwerkt_stadsdelen_not=datum_verwerkt_stadsdelen_not, fase=fase, fase_in=fase_in, fase_isempty=fase_isempty, fase_isnull=fase_isnull, fase_like=fase_like, fase_not=fase_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, kenteken=kenteken, kenteken_kort=kenteken_kort, kenteken_kort_in=kenteken_kort_in, kenteken_kort_isempty=kenteken_kort_isempty, kenteken_kort_isnull=kenteken_kort_isnull, kenteken_kort_like=kenteken_kort_like, kenteken_kort_not=kenteken_kort_not, kenteken_in=kenteken_in, kenteken_isempty=kenteken_isempty, kenteken_isnull=kenteken_isnull, kenteken_like=kenteken_like, kenteken_not=kenteken_not, memo=memo, memo_in=memo_in, memo_isempty=memo_isempty, memo_isnull=memo_isnull, memo_like=memo_like, memo_not=memo_not, pauze_eindtijd=pauze_eindtijd, pauze_eindtijd_in=pauze_eindtijd_in, pauze_eindtijd_isempty=pauze_eindtijd_isempty, pauze_eindtijd_isnull=pauze_eindtijd_isnull, pauze_eindtijd_like=pauze_eindtijd_like, pauze_eindtijd_not=pauze_eindtijd_not, pauze_starttijd=pauze_starttijd, pauze_starttijd_in=pauze_starttijd_in, pauze_starttijd_isempty=pauze_starttijd_isempty, pauze_starttijd_isnull=pauze_starttijd_isnull, pauze_starttijd_like=pauze_starttijd_like, pauze_starttijd_not=pauze_starttijd_not, pauze_uren_gepland=pauze_uren_gepland, pauze_uren_gepland_gt=pauze_uren_gepland_gt, pauze_uren_gepland_gte=pauze_uren_gepland_gte, pauze_uren_gepland_in=pauze_uren_gepland_in, pauze_uren_gepland_isnull=pauze_uren_gepland_isnull, pauze_uren_gepland_lt=pauze_uren_gepland_lt, pauze_uren_gepland_lte=pauze_uren_gepland_lte, pauze_uren_gepland_not=pauze_uren_gepland_not, soort_werkzaamheden=soort_werkzaamheden, soort_werkzaamheden_in=soort_werkzaamheden_in, soort_werkzaamheden_isempty=soort_werkzaamheden_isempty, soort_werkzaamheden_isnull=soort_werkzaamheden_isnull, soort_werkzaamheden_like=soort_werkzaamheden_like, soort_werkzaamheden_not=soort_werkzaamheden_not, team=team, team_in=team_in, team_isempty=team_isempty, team_isnull=team_isnull, team_like=team_like, team_not=team_not, uren_inzet_medewerker_inhuur=uren_inzet_medewerker_inhuur, uren_inzet_medewerker_inhuur_gt=uren_inzet_medewerker_inhuur_gt, uren_inzet_medewerker_inhuur_gte=uren_inzet_medewerker_inhuur_gte, uren_inzet_medewerker_inhuur_in=uren_inzet_medewerker_inhuur_in, uren_inzet_medewerker_inhuur_isnull=uren_inzet_medewerker_inhuur_isnull, uren_inzet_medewerker_inhuur_lt=uren_inzet_medewerker_inhuur_lt, uren_inzet_medewerker_inhuur_lte=uren_inzet_medewerker_inhuur_lte, uren_inzet_medewerker_inhuur_not=uren_inzet_medewerker_inhuur_not, uren_inzet_medewerker_intern=uren_inzet_medewerker_intern, uren_inzet_medewerker_intern_gt=uren_inzet_medewerker_intern_gt, uren_inzet_medewerker_intern_gte=uren_inzet_medewerker_intern_gte, uren_inzet_medewerker_intern_in=uren_inzet_medewerker_intern_in, uren_inzet_medewerker_intern_isnull=uren_inzet_medewerker_intern_isnull, uren_inzet_medewerker_intern_lt=uren_inzet_medewerker_intern_lt, uren_inzet_medewerker_intern_lte=uren_inzet_medewerker_intern_lte, uren_inzet_medewerker_intern_not=uren_inzet_medewerker_intern_not, uren_inzet_voertuig=uren_inzet_voertuig, uren_inzet_voertuig_gt=uren_inzet_voertuig_gt, uren_inzet_voertuig_gte=uren_inzet_voertuig_gte, uren_inzet_voertuig_in=uren_inzet_voertuig_in, uren_inzet_voertuig_isnull=uren_inzet_voertuig_isnull, uren_inzet_voertuig_lt=uren_inzet_voertuig_lt, uren_inzet_voertuig_lte=uren_inzet_voertuig_lte, uren_inzet_voertuig_not=uren_inzet_voertuig_not, voertuig_inhuur_indicatie=voertuig_inhuur_indicatie, voertuig_inhuur_indicatie_in=voertuig_inhuur_indicatie_in, voertuig_inhuur_indicatie_isempty=voertuig_inhuur_indicatie_isempty, voertuig_inhuur_indicatie_isnull=voertuig_inhuur_indicatie_isnull, voertuig_inhuur_indicatie_like=voertuig_inhuur_indicatie_like, voertuig_inhuur_indicatie_not=voertuig_inhuur_indicatie_not, werkzaamheden_code=werkzaamheden_code, werkzaamheden_code_in=werkzaamheden_code_in, werkzaamheden_code_isempty=werkzaamheden_code_isempty, werkzaamheden_code_isnull=werkzaamheden_code_isnull, werkzaamheden_code_like=werkzaamheden_code_like, werkzaamheden_code_not=werkzaamheden_code_not, werkzaamheden_datum=werkzaamheden_datum, werkzaamheden_datum_ref_id=werkzaamheden_datum_ref_id, werkzaamheden_datum_ref_id_gt=werkzaamheden_datum_ref_id_gt, werkzaamheden_datum_ref_id_gte=werkzaamheden_datum_ref_id_gte, werkzaamheden_datum_ref_id_in=werkzaamheden_datum_ref_id_in, werkzaamheden_datum_ref_id_isnull=werkzaamheden_datum_ref_id_isnull, werkzaamheden_datum_ref_id_lt=werkzaamheden_datum_ref_id_lt, werkzaamheden_datum_ref_id_lte=werkzaamheden_datum_ref_id_lte, werkzaamheden_datum_ref_id_not=werkzaamheden_datum_ref_id_not, werkzaamheden_datum_gt=werkzaamheden_datum_gt, werkzaamheden_datum_gte=werkzaamheden_datum_gte, werkzaamheden_datum_in=werkzaamheden_datum_in, werkzaamheden_datum_isnull=werkzaamheden_datum_isnull, werkzaamheden_datum_lt=werkzaamheden_datum_lt, werkzaamheden_datum_lte=werkzaamheden_datum_lte, werkzaamheden_datum_not=werkzaamheden_datum_not, werkzaamheden_eindtijd=werkzaamheden_eindtijd, werkzaamheden_eindtijd_in=werkzaamheden_eindtijd_in, werkzaamheden_eindtijd_isempty=werkzaamheden_eindtijd_isempty, werkzaamheden_eindtijd_isnull=werkzaamheden_eindtijd_isnull, werkzaamheden_eindtijd_like=werkzaamheden_eindtijd_like, werkzaamheden_eindtijd_not=werkzaamheden_eindtijd_not, werkzaamheden_omschrijving=werkzaamheden_omschrijving, werkzaamheden_omschrijving_in=werkzaamheden_omschrijving_in, werkzaamheden_omschrijving_isempty=werkzaamheden_omschrijving_isempty, werkzaamheden_omschrijving_isnull=werkzaamheden_omschrijving_isnull, werkzaamheden_omschrijving_like=werkzaamheden_omschrijving_like, werkzaamheden_omschrijving_not=werkzaamheden_omschrijving_not, werkzaamheden_starttijd=werkzaamheden_starttijd, werkzaamheden_starttijd_in=werkzaamheden_starttijd_in, werkzaamheden_starttijd_isempty=werkzaamheden_starttijd_isempty, werkzaamheden_starttijd_isnull=werkzaamheden_starttijd_isnull, werkzaamheden_starttijd_like=werkzaamheden_starttijd_like, werkzaamheden_starttijd_not=werkzaamheden_starttijd_not, werkzaamheden_uren_gepland=werkzaamheden_uren_gepland, werkzaamheden_uren_gepland_gt=werkzaamheden_uren_gepland_gt, werkzaamheden_uren_gepland_gte=werkzaamheden_uren_gepland_gte, werkzaamheden_uren_gepland_in=werkzaamheden_uren_gepland_in, werkzaamheden_uren_gepland_isnull=werkzaamheden_uren_gepland_isnull, werkzaamheden_uren_gepland_lt=werkzaamheden_uren_gepland_lt, werkzaamheden_uren_gepland_lte=werkzaamheden_uren_gepland_lte, werkzaamheden_uren_gepland_not=werkzaamheden_uren_gepland_not)
        print("The response of PlanningVoertuigenApi->huishoudelijkafval_planning_voertuigen_retrieve_slash:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PlanningVoertuigenApi->huishoudelijkafval_planning_voertuigen_retrieve_slash: %s\n" % e)
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
 **aantal_medewerkers** | **float**| Aantal medewerkers dat op het voertuig is gepland. | [optional] 
 **aantal_medewerkers_inhuur** | **float**| Aantal externe medewerkers dat op het voertuig is gepland. | [optional] 
 **aantal_medewerkers_inhuur_gt** | **float**| Greater than; number | [optional] 
 **aantal_medewerkers_inhuur_gte** | **float**| Greater than or equal to; number | [optional] 
 **aantal_medewerkers_inhuur_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_medewerkers_inhuur_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_medewerkers_inhuur_lt** | **float**| Less than; number | [optional] 
 **aantal_medewerkers_inhuur_lte** | **float**| Less than or equal to; number | [optional] 
 **aantal_medewerkers_inhuur_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **aantal_medewerkers_intern** | **float**| Aantal interne medewerkers dat op het voertuig is gepland. | [optional] 
 **aantal_medewerkers_intern_gt** | **float**| Greater than; number | [optional] 
 **aantal_medewerkers_intern_gte** | **float**| Greater than or equal to; number | [optional] 
 **aantal_medewerkers_intern_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_medewerkers_intern_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_medewerkers_intern_lt** | **float**| Less than; number | [optional] 
 **aantal_medewerkers_intern_lte** | **float**| Less than or equal to; number | [optional] 
 **aantal_medewerkers_intern_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **aantal_medewerkers_gt** | **float**| Greater than; number | [optional] 
 **aantal_medewerkers_gte** | **float**| Greater than or equal to; number | [optional] 
 **aantal_medewerkers_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **aantal_medewerkers_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **aantal_medewerkers_lt** | **float**| Less than; number | [optional] 
 **aantal_medewerkers_lte** | **float**| Less than or equal to; number | [optional] 
 **aantal_medewerkers_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **activiteit** | **str**| Fractie van de afvalverwerking (afgeleid van categorie, werkzaamheden en of memo). | [optional] 
 **activiteit_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **activiteit_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **activiteit_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **activiteit_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **activiteit_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **categorie** | **str**| Categorie afvalverwerking waar het voertuig op is gepland. | [optional] 
 **categorie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **categorie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **categorie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **categorie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **categorie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_aanwezig_bron** | **datetime**| Indicatie over de actualiteit van de gegevens in deze set (laatste wijziging in de bron). | [optional] 
 **datum_aanwezig_bron_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_aanwezig_bron_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_aanwezig_bron_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_aanwezig_bron_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_aanwezig_bron_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_aanwezig_bron_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_aanwezig_bron_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen** | **datetime**| Moment van laden data vanuit het (planningsdata)bronsysteem in het DWH stadsdelen (als intermediair voor datalevering). | [optional] 
 **datum_verwerkt_stadsdelen_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_verwerkt_stadsdelen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_verwerkt_stadsdelen_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_verwerkt_stadsdelen_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **fase** | **str**| Label van de fase waarin de planning zich bevindt. | [optional] 
 **fase_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **fase_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **fase_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **fase_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **fase_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **id2** | **int**| Uniek identificerend kenmerk van het record. | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **kenteken** | **str**| Kenteken afvalinzamelingsvoertuig. | [optional] 
 **kenteken_kort** | **str**| Kenteken afvalinzamelingsvoertuig zonder koppeltekens (-). | [optional] 
 **kenteken_kort_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **kenteken_kort_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **kenteken_kort_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **kenteken_kort_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **kenteken_kort_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **kenteken_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **kenteken_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **kenteken_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **kenteken_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **kenteken_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **memo** | **str**| Extra toelichting zoals opgegeven in (planningsdata)bronsysteem. | [optional] 
 **memo_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **memo_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **memo_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **memo_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **memo_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **pauze_eindtijd** | **str**| Eindtijd van de pauze op de WERKZAAMHEDEN_DATUM. | [optional] 
 **pauze_eindtijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **pauze_eindtijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **pauze_eindtijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **pauze_eindtijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **pauze_eindtijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **pauze_starttijd** | **str**| Starttijd van de pauze op de WERKZAAMHEDEN_DATUM. | [optional] 
 **pauze_starttijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **pauze_starttijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **pauze_starttijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **pauze_starttijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **pauze_starttijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **pauze_uren_gepland** | **float**| Berekening van het aantal bruto uren van de pauze (&#x3D; eindtijd - starttijd). | [optional] 
 **pauze_uren_gepland_gt** | **float**| Greater than; number | [optional] 
 **pauze_uren_gepland_gte** | **float**| Greater than or equal to; number | [optional] 
 **pauze_uren_gepland_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **pauze_uren_gepland_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **pauze_uren_gepland_lt** | **float**| Less than; number | [optional] 
 **pauze_uren_gepland_lte** | **float**| Less than or equal to; number | [optional] 
 **pauze_uren_gepland_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **soort_werkzaamheden** | **str**| Specificatie van soort planning (Inzet of Onderhoud). | [optional] 
 **soort_werkzaamheden_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **soort_werkzaamheden_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **soort_werkzaamheden_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **soort_werkzaamheden_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **soort_werkzaamheden_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **team** | **str**| Team waarvoor de voertuigplanning is gemaakt. In veel gevallen een stadsdeel, maar kan ook bijvoorbeeld Bedrijfsafval Centrum (BAC) zijn). | [optional] 
 **team_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **team_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **team_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **team_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **team_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **uren_inzet_medewerker_inhuur** | **float**| Som van het totaal aantal netto uren van de externe medewerkers die op de planning zijn gezet (excl pauze). | [optional] 
 **uren_inzet_medewerker_inhuur_gt** | **float**| Greater than; number | [optional] 
 **uren_inzet_medewerker_inhuur_gte** | **float**| Greater than or equal to; number | [optional] 
 **uren_inzet_medewerker_inhuur_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **uren_inzet_medewerker_inhuur_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **uren_inzet_medewerker_inhuur_lt** | **float**| Less than; number | [optional] 
 **uren_inzet_medewerker_inhuur_lte** | **float**| Less than or equal to; number | [optional] 
 **uren_inzet_medewerker_inhuur_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **uren_inzet_medewerker_intern** | **float**| Som van het totaal aantal netto uren van de interne medewerkers die op de planning zijn gezet (excl pauze). | [optional] 
 **uren_inzet_medewerker_intern_gt** | **float**| Greater than; number | [optional] 
 **uren_inzet_medewerker_intern_gte** | **float**| Greater than or equal to; number | [optional] 
 **uren_inzet_medewerker_intern_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **uren_inzet_medewerker_intern_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **uren_inzet_medewerker_intern_lt** | **float**| Less than; number | [optional] 
 **uren_inzet_medewerker_intern_lte** | **float**| Less than or equal to; number | [optional] 
 **uren_inzet_medewerker_intern_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **uren_inzet_voertuig** | **float**| Netto inzeturen van het voertuig (bruto - pauze). | [optional] 
 **uren_inzet_voertuig_gt** | **float**| Greater than; number | [optional] 
 **uren_inzet_voertuig_gte** | **float**| Greater than or equal to; number | [optional] 
 **uren_inzet_voertuig_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **uren_inzet_voertuig_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **uren_inzet_voertuig_lt** | **float**| Less than; number | [optional] 
 **uren_inzet_voertuig_lte** | **float**| Less than or equal to; number | [optional] 
 **uren_inzet_voertuig_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **voertuig_inhuur_indicatie** | **str**| Is het voertuig ingehuurd (Ja / Nee). | [optional] 
 **voertuig_inhuur_indicatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **voertuig_inhuur_indicatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **voertuig_inhuur_indicatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **voertuig_inhuur_indicatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **voertuig_inhuur_indicatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_code** | **str**| Code voor de werkzaamheden waarop het voertuig is gepland. | [optional] 
 **werkzaamheden_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **werkzaamheden_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **werkzaamheden_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_datum** | **datetime**| Datum waarop de werkzaamheden zijn gepland. | [optional] 
 **werkzaamheden_datum_ref_id** | **int**| Sleutelveld. Bij niveaucode dag is dit in feite de juliaanse dag. Zo kan bijvoorbeeld het verschil tussen twee datums bepaald worden door het verschil tussen de ID waarden van de datums te berekenen. De id waarden zijn zo geconstrueerd dat dit altijd kan ongeacht de waarde van niveaucode. Dus als b.v. niveaucode is &#39;Week&#39; dan bevat een verschil in id waarden het aantal weken tussen de twee week records. | [optional] 
 **werkzaamheden_datum_ref_id_gt** | **int**| Greater than; number | [optional] 
 **werkzaamheden_datum_ref_id_gte** | **int**| Greater than or equal to; number | [optional] 
 **werkzaamheden_datum_ref_id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_datum_ref_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_datum_ref_id_lt** | **int**| Less than; number | [optional] 
 **werkzaamheden_datum_ref_id_lte** | **int**| Less than or equal to; number | [optional] 
 **werkzaamheden_datum_ref_id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **werkzaamheden_datum_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_datum_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_datum_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_datum_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_datum_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_datum_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_datum_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **werkzaamheden_eindtijd** | **str**| Eindtijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM. | [optional] 
 **werkzaamheden_eindtijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_eindtijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **werkzaamheden_eindtijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_eindtijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **werkzaamheden_eindtijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_omschrijving** | **str**| Omschrijving voor de werkzaamheden waarop het voertuig is gepland. | [optional] 
 **werkzaamheden_omschrijving_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_omschrijving_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **werkzaamheden_omschrijving_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_omschrijving_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **werkzaamheden_omschrijving_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_starttijd** | **str**| Starttijd van de werkzaamheden op de WERKZAAMHEDEN_DATUM | [optional] 
 **werkzaamheden_starttijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_starttijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **werkzaamheden_starttijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_starttijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **werkzaamheden_starttijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **werkzaamheden_uren_gepland** | **float**| Berekening van het aantal bruto uren van de werkzaamheden (&#x3D; eindtijd - starttijd). | [optional] 
 **werkzaamheden_uren_gepland_gt** | **float**| Greater than; number | [optional] 
 **werkzaamheden_uren_gepland_gte** | **float**| Greater than or equal to; number | [optional] 
 **werkzaamheden_uren_gepland_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **werkzaamheden_uren_gepland_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **werkzaamheden_uren_gepland_lt** | **float**| Less than; number | [optional] 
 **werkzaamheden_uren_gepland_lte** | **float**| Less than or equal to; number | [optional] 
 **werkzaamheden_uren_gepland_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 

### Return type

[**HuishoudelijkafvalplanningVoertuigen**](HuishoudelijkafvalplanningVoertuigen.md)

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

