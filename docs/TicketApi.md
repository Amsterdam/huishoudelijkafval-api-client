# huishoudelijkafval_api_client.TicketApi

All URIs are relative to *https://api.data.amsterdam.nl*

Method | HTTP request | Description
------------- | ------------- | -------------
[**huishoudelijkafval_ticket_list2**](TicketApi.md#huishoudelijkafval_ticket_list2) | **GET** /ticket | 
[**huishoudelijkafval_ticket_retrieve2**](TicketApi.md#huishoudelijkafval_ticket_retrieve2) | **GET** /ticket/{id} | 


# **huishoudelijkafval_ticket_list2**
> PaginatedHuishoudelijkafvalticketList huishoudelijkafval_ticket_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, container_id=container_id, container_id_in=container_id_in, container_id_isempty=container_id_isempty, container_id_isnull=container_id_isnull, container_id_like=container_id_like, container_id_not=container_id_not, containerlocatie_id=containerlocatie_id, containerlocatie_id_in=containerlocatie_id_in, containerlocatie_id_isempty=containerlocatie_id_isempty, containerlocatie_id_isnull=containerlocatie_id_isnull, containerlocatie_id_like=containerlocatie_id_like, containerlocatie_id_not=containerlocatie_id_not, datum_afgerond=datum_afgerond, datum_afgerond_gt=datum_afgerond_gt, datum_afgerond_gte=datum_afgerond_gte, datum_afgerond_in=datum_afgerond_in, datum_afgerond_isnull=datum_afgerond_isnull, datum_afgerond_lt=datum_afgerond_lt, datum_afgerond_lte=datum_afgerond_lte, datum_afgerond_not=datum_afgerond_not, datum_afgewezen=datum_afgewezen, datum_afgewezen_gt=datum_afgewezen_gt, datum_afgewezen_gte=datum_afgewezen_gte, datum_afgewezen_in=datum_afgewezen_in, datum_afgewezen_isnull=datum_afgewezen_isnull, datum_afgewezen_lt=datum_afgewezen_lt, datum_afgewezen_lte=datum_afgewezen_lte, datum_afgewezen_not=datum_afgewezen_not, datum_creatie=datum_creatie, datum_creatie_gt=datum_creatie_gt, datum_creatie_gte=datum_creatie_gte, datum_creatie_in=datum_creatie_in, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_lt=datum_creatie_lt, datum_creatie_lte=datum_creatie_lte, datum_creatie_not=datum_creatie_not, datum_factuur=datum_factuur, datum_factuur_gt=datum_factuur_gt, datum_factuur_gte=datum_factuur_gte, datum_factuur_in=datum_factuur_in, datum_factuur_isnull=datum_factuur_isnull, datum_factuur_lt=datum_factuur_lt, datum_factuur_lte=datum_factuur_lte, datum_factuur_not=datum_factuur_not, datum_financiele_goedkeuring=datum_financiele_goedkeuring, datum_financiele_goedkeuring_gt=datum_financiele_goedkeuring_gt, datum_financiele_goedkeuring_gte=datum_financiele_goedkeuring_gte, datum_financiele_goedkeuring_in=datum_financiele_goedkeuring_in, datum_financiele_goedkeuring_isnull=datum_financiele_goedkeuring_isnull, datum_financiele_goedkeuring_lt=datum_financiele_goedkeuring_lt, datum_financiele_goedkeuring_lte=datum_financiele_goedkeuring_lte, datum_financiele_goedkeuring_not=datum_financiele_goedkeuring_not, datum_geaccepteerd=datum_geaccepteerd, datum_geaccepteerd_gt=datum_geaccepteerd_gt, datum_geaccepteerd_gte=datum_geaccepteerd_gte, datum_geaccepteerd_in=datum_geaccepteerd_in, datum_geaccepteerd_isnull=datum_geaccepteerd_isnull, datum_geaccepteerd_lt=datum_geaccepteerd_lt, datum_geaccepteerd_lte=datum_geaccepteerd_lte, datum_geaccepteerd_not=datum_geaccepteerd_not, datum_gefactureerd=datum_gefactureerd, datum_gefactureerd_gt=datum_gefactureerd_gt, datum_gefactureerd_gte=datum_gefactureerd_gte, datum_gefactureerd_in=datum_gefactureerd_in, datum_gefactureerd_isnull=datum_gefactureerd_isnull, datum_gefactureerd_lt=datum_gefactureerd_lt, datum_gefactureerd_lte=datum_gefactureerd_lte, datum_gefactureerd_not=datum_gefactureerd_not, datum_gepland=datum_gepland, datum_gepland_gt=datum_gepland_gt, datum_gepland_gte=datum_gepland_gte, datum_gepland_in=datum_gepland_in, datum_gepland_isnull=datum_gepland_isnull, datum_gepland_lt=datum_gepland_lt, datum_gepland_lte=datum_gepland_lte, datum_gepland_not=datum_gepland_not, datum_gereed=datum_gereed, datum_gereed_gt=datum_gereed_gt, datum_gereed_gte=datum_gereed_gte, datum_gereed_in=datum_gereed_in, datum_gereed_isnull=datum_gereed_isnull, datum_gereed_lt=datum_gereed_lt, datum_gereed_lte=datum_gereed_lte, datum_gereed_not=datum_gereed_not, datum_offerte=datum_offerte, datum_offerte_gt=datum_offerte_gt, datum_offerte_gte=datum_offerte_gte, datum_offerte_in=datum_offerte_in, datum_offerte_isnull=datum_offerte_isnull, datum_offerte_lt=datum_offerte_lt, datum_offerte_lte=datum_offerte_lte, datum_offerte_not=datum_offerte_not, datum_technische_goedkeuring=datum_technische_goedkeuring, datum_technische_goedkeuring_gt=datum_technische_goedkeuring_gt, datum_technische_goedkeuring_gte=datum_technische_goedkeuring_gte, datum_technische_goedkeuring_in=datum_technische_goedkeuring_in, datum_technische_goedkeuring_isnull=datum_technische_goedkeuring_isnull, datum_technische_goedkeuring_lt=datum_technische_goedkeuring_lt, datum_technische_goedkeuring_lte=datum_technische_goedkeuring_lte, datum_technische_goedkeuring_not=datum_technische_goedkeuring_not, datum_wijziging=datum_wijziging, datum_wijziging_gt=datum_wijziging_gt, datum_wijziging_gte=datum_wijziging_gte, datum_wijziging_in=datum_wijziging_in, datum_wijziging_isnull=datum_wijziging_isnull, datum_wijziging_lt=datum_wijziging_lt, datum_wijziging_lte=datum_wijziging_lte, datum_wijziging_not=datum_wijziging_not, datum_workflow_start=datum_workflow_start, datum_workflow_start_gt=datum_workflow_start_gt, datum_workflow_start_gte=datum_workflow_start_gte, datum_workflow_start_in=datum_workflow_start_in, datum_workflow_start_isnull=datum_workflow_start_isnull, datum_workflow_start_lt=datum_workflow_start_lt, datum_workflow_start_lte=datum_workflow_start_lte, datum_workflow_start_not=datum_workflow_start_not, doorlooptijd=doorlooptijd, doorlooptijd_in=doorlooptijd_in, doorlooptijd_isempty=doorlooptijd_isempty, doorlooptijd_isnull=doorlooptijd_isnull, doorlooptijd_like=doorlooptijd_like, doorlooptijd_not=doorlooptijd_not, eigenaar=eigenaar, eigenaar_in=eigenaar_in, eigenaar_isempty=eigenaar_isempty, eigenaar_isnull=eigenaar_isnull, eigenaar_like=eigenaar_like, eigenaar_not=eigenaar_not, factuur_nummer=factuur_nummer, factuur_nummer_in=factuur_nummer_in, factuur_nummer_isempty=factuur_nummer_isempty, factuur_nummer_isnull=factuur_nummer_isnull, factuur_nummer_like=factuur_nummer_like, factuur_nummer_not=factuur_nummer_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, gbd_buurt_code=gbd_buurt_code, gbd_buurt_code_in=gbd_buurt_code_in, gbd_buurt_code_isempty=gbd_buurt_code_isempty, gbd_buurt_code_isnull=gbd_buurt_code_isnull, gbd_buurt_code_like=gbd_buurt_code_like, gbd_buurt_code_not=gbd_buurt_code_not, gbd_buurt_naam=gbd_buurt_naam, gbd_buurt_naam_in=gbd_buurt_naam_in, gbd_buurt_naam_isempty=gbd_buurt_naam_isempty, gbd_buurt_naam_isnull=gbd_buurt_naam_isnull, gbd_buurt_naam_like=gbd_buurt_naam_like, gbd_buurt_naam_not=gbd_buurt_naam_not, gbd_buurt_volgnummer=gbd_buurt_volgnummer, gbd_buurt_volgnummer_gt=gbd_buurt_volgnummer_gt, gbd_buurt_volgnummer_gte=gbd_buurt_volgnummer_gte, gbd_buurt_volgnummer_in=gbd_buurt_volgnummer_in, gbd_buurt_volgnummer_isnull=gbd_buurt_volgnummer_isnull, gbd_buurt_volgnummer_lt=gbd_buurt_volgnummer_lt, gbd_buurt_volgnummer_lte=gbd_buurt_volgnummer_lte, gbd_buurt_volgnummer_not=gbd_buurt_volgnummer_not, gbd_ggw_identificatie=gbd_ggw_identificatie, gbd_ggw_identificatie_in=gbd_ggw_identificatie_in, gbd_ggw_identificatie_isempty=gbd_ggw_identificatie_isempty, gbd_ggw_identificatie_isnull=gbd_ggw_identificatie_isnull, gbd_ggw_identificatie_like=gbd_ggw_identificatie_like, gbd_ggw_identificatie_not=gbd_ggw_identificatie_not, gbd_ggw_naam=gbd_ggw_naam, gbd_ggw_naam_in=gbd_ggw_naam_in, gbd_ggw_naam_isempty=gbd_ggw_naam_isempty, gbd_ggw_naam_isnull=gbd_ggw_naam_isnull, gbd_ggw_naam_like=gbd_ggw_naam_like, gbd_ggw_naam_not=gbd_ggw_naam_not, gbd_ggw_volgnummer=gbd_ggw_volgnummer, gbd_ggw_volgnummer_in=gbd_ggw_volgnummer_in, gbd_ggw_volgnummer_isempty=gbd_ggw_volgnummer_isempty, gbd_ggw_volgnummer_isnull=gbd_ggw_volgnummer_isnull, gbd_ggw_volgnummer_like=gbd_ggw_volgnummer_like, gbd_ggw_volgnummer_not=gbd_ggw_volgnummer_not, gbd_stadsdeel_identificatie=gbd_stadsdeel_identificatie, gbd_stadsdeel_identificatie_in=gbd_stadsdeel_identificatie_in, gbd_stadsdeel_identificatie_isempty=gbd_stadsdeel_identificatie_isempty, gbd_stadsdeel_identificatie_isnull=gbd_stadsdeel_identificatie_isnull, gbd_stadsdeel_identificatie_like=gbd_stadsdeel_identificatie_like, gbd_stadsdeel_identificatie_not=gbd_stadsdeel_identificatie_not, gbd_stadsdeel_naam=gbd_stadsdeel_naam, gbd_stadsdeel_naam_in=gbd_stadsdeel_naam_in, gbd_stadsdeel_naam_isempty=gbd_stadsdeel_naam_isempty, gbd_stadsdeel_naam_isnull=gbd_stadsdeel_naam_isnull, gbd_stadsdeel_naam_like=gbd_stadsdeel_naam_like, gbd_stadsdeel_naam_not=gbd_stadsdeel_naam_not, gbd_stadsdeel_volgnummer=gbd_stadsdeel_volgnummer, gbd_stadsdeel_volgnummer_gt=gbd_stadsdeel_volgnummer_gt, gbd_stadsdeel_volgnummer_gte=gbd_stadsdeel_volgnummer_gte, gbd_stadsdeel_volgnummer_in=gbd_stadsdeel_volgnummer_in, gbd_stadsdeel_volgnummer_isnull=gbd_stadsdeel_volgnummer_isnull, gbd_stadsdeel_volgnummer_lt=gbd_stadsdeel_volgnummer_lt, gbd_stadsdeel_volgnummer_lte=gbd_stadsdeel_volgnummer_lte, gbd_stadsdeel_volgnummer_not=gbd_stadsdeel_volgnummer_not, gbd_wijk_identificatie=gbd_wijk_identificatie, gbd_wijk_identificatie_in=gbd_wijk_identificatie_in, gbd_wijk_identificatie_isempty=gbd_wijk_identificatie_isempty, gbd_wijk_identificatie_isnull=gbd_wijk_identificatie_isnull, gbd_wijk_identificatie_like=gbd_wijk_identificatie_like, gbd_wijk_identificatie_not=gbd_wijk_identificatie_not, gbd_wijk_naam=gbd_wijk_naam, gbd_wijk_naam_in=gbd_wijk_naam_in, gbd_wijk_naam_isempty=gbd_wijk_naam_isempty, gbd_wijk_naam_isnull=gbd_wijk_naam_isnull, gbd_wijk_naam_like=gbd_wijk_naam_like, gbd_wijk_naam_not=gbd_wijk_naam_not, gbd_wijk_volgnummer=gbd_wijk_volgnummer, gbd_wijk_volgnummer_gt=gbd_wijk_volgnummer_gt, gbd_wijk_volgnummer_gte=gbd_wijk_volgnummer_gte, gbd_wijk_volgnummer_in=gbd_wijk_volgnummer_in, gbd_wijk_volgnummer_isnull=gbd_wijk_volgnummer_isnull, gbd_wijk_volgnummer_lt=gbd_wijk_volgnummer_lt, gbd_wijk_volgnummer_lte=gbd_wijk_volgnummer_lte, gbd_wijk_volgnummer_not=gbd_wijk_volgnummer_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, items_definitief=items_definitief, items_definitief_in=items_definitief_in, items_definitief_isempty=items_definitief_isempty, items_definitief_isnull=items_definitief_isnull, items_definitief_like=items_definitief_like, items_definitief_not=items_definitief_not, items_offerte=items_offerte, items_offerte_in=items_offerte_in, items_offerte_isempty=items_offerte_isempty, items_offerte_isnull=items_offerte_isnull, items_offerte_like=items_offerte_like, items_offerte_not=items_offerte_not, onderhoudsbedrijf=onderhoudsbedrijf, onderhoudsbedrijf_in=onderhoudsbedrijf_in, onderhoudsbedrijf_isempty=onderhoudsbedrijf_isempty, onderhoudsbedrijf_isnull=onderhoudsbedrijf_isnull, onderhoudsbedrijf_like=onderhoudsbedrijf_like, onderhoudsbedrijf_not=onderhoudsbedrijf_not, oorzaak=oorzaak, oorzaak_contains=oorzaak_contains, oplossing=oplossing, oplossing_contains=oplossing_contains, page=page, prijs=prijs, prijs_offerte=prijs_offerte, prijs_offerte_gt=prijs_offerte_gt, prijs_offerte_gte=prijs_offerte_gte, prijs_offerte_in=prijs_offerte_in, prijs_offerte_isnull=prijs_offerte_isnull, prijs_offerte_lt=prijs_offerte_lt, prijs_offerte_lte=prijs_offerte_lte, prijs_offerte_not=prijs_offerte_not, prijs_gt=prijs_gt, prijs_gte=prijs_gte, prijs_in=prijs_in, prijs_isnull=prijs_isnull, prijs_lt=prijs_lt, prijs_lte=prijs_lte, prijs_not=prijs_not, prioriteit_naam=prioriteit_naam, prioriteit_naam_in=prioriteit_naam_in, prioriteit_naam_isempty=prioriteit_naam_isempty, prioriteit_naam_isnull=prioriteit_naam_isnull, prioriteit_naam_like=prioriteit_naam_like, prioriteit_naam_not=prioriteit_naam_not, prioriteit_opmerking=prioriteit_opmerking, prioriteit_opmerking_in=prioriteit_opmerking_in, prioriteit_opmerking_isempty=prioriteit_opmerking_isempty, prioriteit_opmerking_isnull=prioriteit_opmerking_isnull, prioriteit_opmerking_like=prioriteit_opmerking_like, prioriteit_opmerking_not=prioriteit_opmerking_not, prioriteit_responstijd=prioriteit_responstijd, prioriteit_responstijd_gt=prioriteit_responstijd_gt, prioriteit_responstijd_gte=prioriteit_responstijd_gte, prioriteit_responstijd_in=prioriteit_responstijd_in, prioriteit_responstijd_isnull=prioriteit_responstijd_isnull, prioriteit_responstijd_lt=prioriteit_responstijd_lt, prioriteit_responstijd_lte=prioriteit_responstijd_lte, prioriteit_responstijd_not=prioriteit_responstijd_not, probleem=probleem, probleem_module_naam=probleem_module_naam, probleem_module_naam_contains=probleem_module_naam_contains, probleem_contains=probleem_contains, rangorde_nummer_tickettype=rangorde_nummer_tickettype, rangorde_nummer_tickettype_gt=rangorde_nummer_tickettype_gt, rangorde_nummer_tickettype_gte=rangorde_nummer_tickettype_gte, rangorde_nummer_tickettype_in=rangorde_nummer_tickettype_in, rangorde_nummer_tickettype_isnull=rangorde_nummer_tickettype_isnull, rangorde_nummer_tickettype_lt=rangorde_nummer_tickettype_lt, rangorde_nummer_tickettype_lte=rangorde_nummer_tickettype_lte, rangorde_nummer_tickettype_not=rangorde_nummer_tickettype_not, reden_afgewezen=reden_afgewezen, reden_afgewezen_in=reden_afgewezen_in, reden_afgewezen_isempty=reden_afgewezen_isempty, reden_afgewezen_isnull=reden_afgewezen_isnull, reden_afgewezen_like=reden_afgewezen_like, reden_afgewezen_not=reden_afgewezen_not, referentienummer_leverancier=referentienummer_leverancier, referentienummer_leverancier_in=referentienummer_leverancier_in, referentienummer_leverancier_isempty=referentienummer_leverancier_isempty, referentienummer_leverancier_isnull=referentienummer_leverancier_isnull, referentienummer_leverancier_like=referentienummer_leverancier_like, referentienummer_leverancier_not=referentienummer_leverancier_not, ticketstatus=ticketstatus, ticketstatus_in=ticketstatus_in, ticketstatus_isempty=ticketstatus_isempty, ticketstatus_isnull=ticketstatus_isnull, ticketstatus_like=ticketstatus_like, ticketstatus_not=ticketstatus_not, tickettype=tickettype, tickettype_in=tickettype_in, tickettype_isempty=tickettype_isempty, tickettype_isnull=tickettype_isnull, tickettype_like=tickettype_like, tickettype_not=tickettype_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalticket_list import PaginatedHuishoudelijkafvalticketList
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
    api_instance = huishoudelijkafval_api_client.TicketApi(api_client)
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    count = True # bool | Include a count of the total result set and the number of pages.Only works for responses that return a page. (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'container' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    page_size = 56 # int | Number of results to return per page. (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    container_id = 'container_id_example' # str | Unieke aanduiding objecttype (optional)
    container_id_in = ['container_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_id_isempty = True # bool | Whether the field is empty or not. (optional)
    container_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_id_like = 'container_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_id_not = ['container_id_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_id = 'containerlocatie_id_example' # str | Identificerend kenmerk van de put waarin de container is geplaatst (optional)
    containerlocatie_id_in = ['containerlocatie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_id_like = 'containerlocatie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_id_not = ['containerlocatie_id_not_example'] # List[str] | Exclude matches; text (optional)
    datum_afgerond = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de werkzaamheden als gereed aangegeven zijn door het onderhoudsbedrijf. (optional)
    datum_afgerond_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgerond_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgerond_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_afgerond_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_afgerond_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgerond_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgerond_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket de status 'afgewezen' krijgt. (optional)
    datum_afgewezen_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_afgewezen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_afgewezen_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket aangemaakt is. (optional)
    datum_creatie_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_creatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_creatie_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket gefactureerd is. (optional)
    datum_factuur_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_factuur_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_factuur_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de financiale aspecten van de werkzaamheden goed- of afgekeurd zijn. (optional)
    datum_financiele_goedkeuring_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_financiele_goedkeuring_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_financiele_goedkeuring_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket geaccepteerd is door het onderhoudsbedrijf. (optional)
    datum_geaccepteerd_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_geaccepteerd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_geaccepteerd_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de factuur in het systeem de status 'gefactureerd' krijgt. (optional)
    datum_gefactureerd_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_gefactureerd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_gefactureerd_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de uitvoering van de werkzaamheden is ingepland. (optional)
    datum_gepland_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_gepland_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_gepland_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de werkzaamheden uitgevoerd zijn. (optional)
    datum_gereed_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_gereed_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_gereed_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de offerte is aangemaakt . (optional)
    datum_offerte_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_offerte_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_offerte_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de technische aspecten van de werkzaamheden goed- of afgekeurd zijn. (optional)
    datum_technische_goedkeuring_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_technische_goedkeuring_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_technische_goedkeuring_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket is gewijzigd. (optional)
    datum_wijziging_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_wijziging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_wijziging_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de workflow start. (optional)
    datum_workflow_start_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_workflow_start_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_workflow_start_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    doorlooptijd = 'doorlooptijd_example' # str | De tijdsspanne in werkdagen tussen de 'datumCreatie'en de 'datumAfgerond' of de tijdsspanne in werkdagen tussen de 'datumCreatie' en de laatste statuswijziging in het geval het ticket nog niet afgerond is. (optional)
    doorlooptijd_in = ['doorlooptijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    doorlooptijd_isempty = True # bool | Whether the field is empty or not. (optional)
    doorlooptijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    doorlooptijd_like = 'doorlooptijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    doorlooptijd_not = ['doorlooptijd_not_example'] # List[str] | Exclude matches; text (optional)
    eigenaar = 'eigenaar_example' # str | De naam van de eigenaar van de container. (optional)
    eigenaar_in = ['eigenaar_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    eigenaar_isempty = True # bool | Whether the field is empty or not. (optional)
    eigenaar_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    eigenaar_like = 'eigenaar_like_example' # str | Matches text using wildcards (? and *). (optional)
    eigenaar_not = ['eigenaar_not_example'] # List[str] | Exclude matches; text (optional)
    factuur_nummer = 'factuur_nummer_example' # str | Het nummer van de factuur. (optional)
    factuur_nummer_in = ['factuur_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    factuur_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    factuur_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    factuur_nummer_like = 'factuur_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    factuur_nummer_not = ['factuur_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_code = 'gbd_buurt_code_example' # str | Unieke code. (optional)
    gbd_buurt_code_in = ['gbd_buurt_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_code_like = 'gbd_buurt_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_code_not = ['gbd_buurt_code_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_naam = 'gbd_buurt_naam_example' # str | De naam van het object. (optional)
    gbd_buurt_naam_in = ['gbd_buurt_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_naam_like = 'gbd_buurt_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_naam_not = ['gbd_buurt_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_volgnummer = 56 # int | Uniek volgnummer van de toestand van het object. (optional)
    gbd_buurt_volgnummer_gt = 56 # int | Greater than; number (optional)
    gbd_buurt_volgnummer_gte = 56 # int | Greater than or equal to; number (optional)
    gbd_buurt_volgnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_volgnummer_lt = 56 # int | Less than; number (optional)
    gbd_buurt_volgnummer_lte = 56 # int | Less than or equal to; number (optional)
    gbd_buurt_volgnummer_not = [56] # List[int] | Exclude matches; number (optional)
    gbd_ggw_identificatie = 'gbd_ggw_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_ggw_identificatie_in = ['gbd_ggw_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_ggw_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_ggw_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_ggw_identificatie_like = 'gbd_ggw_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_ggw_identificatie_not = ['gbd_ggw_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_ggw_naam = 'gbd_ggw_naam_example' # str | De naam van het object. (optional)
    gbd_ggw_naam_in = ['gbd_ggw_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_ggw_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_ggw_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_ggw_naam_like = 'gbd_ggw_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_ggw_naam_not = ['gbd_ggw_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_ggw_volgnummer = 'gbd_ggw_volgnummer_example' # str | Uniek volgnummer van de toestand van het object. (optional)
    gbd_ggw_volgnummer_in = ['gbd_ggw_volgnummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_ggw_volgnummer_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_ggw_volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_ggw_volgnummer_like = 'gbd_ggw_volgnummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_ggw_volgnummer_not = ['gbd_ggw_volgnummer_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_stadsdeel_identificatie = 'gbd_stadsdeel_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_stadsdeel_identificatie_in = ['gbd_stadsdeel_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_stadsdeel_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_stadsdeel_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_stadsdeel_identificatie_like = 'gbd_stadsdeel_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_stadsdeel_identificatie_not = ['gbd_stadsdeel_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_stadsdeel_naam = 'gbd_stadsdeel_naam_example' # str | De naam van het object. (optional)
    gbd_stadsdeel_naam_in = ['gbd_stadsdeel_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_stadsdeel_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_stadsdeel_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_stadsdeel_naam_like = 'gbd_stadsdeel_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_stadsdeel_naam_not = ['gbd_stadsdeel_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_stadsdeel_volgnummer = 56 # int | Uniek volgnummer van de toestand van het object. (optional)
    gbd_stadsdeel_volgnummer_gt = 56 # int | Greater than; number (optional)
    gbd_stadsdeel_volgnummer_gte = 56 # int | Greater than or equal to; number (optional)
    gbd_stadsdeel_volgnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_stadsdeel_volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_stadsdeel_volgnummer_lt = 56 # int | Less than; number (optional)
    gbd_stadsdeel_volgnummer_lte = 56 # int | Less than or equal to; number (optional)
    gbd_stadsdeel_volgnummer_not = [56] # List[int] | Exclude matches; number (optional)
    gbd_wijk_identificatie = 'gbd_wijk_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_wijk_identificatie_in = ['gbd_wijk_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_wijk_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_wijk_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_wijk_identificatie_like = 'gbd_wijk_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_wijk_identificatie_not = ['gbd_wijk_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_wijk_naam = 'gbd_wijk_naam_example' # str | De naam van het object. (optional)
    gbd_wijk_naam_in = ['gbd_wijk_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_wijk_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_wijk_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_wijk_naam_like = 'gbd_wijk_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_wijk_naam_not = ['gbd_wijk_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_wijk_volgnummer = 56 # int | Uniek volgnummer van de toestand van het object. (optional)
    gbd_wijk_volgnummer_gt = 56 # int | Greater than; number (optional)
    gbd_wijk_volgnummer_gte = 56 # int | Greater than or equal to; number (optional)
    gbd_wijk_volgnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_wijk_volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_wijk_volgnummer_lt = 56 # int | Less than; number (optional)
    gbd_wijk_volgnummer_lte = 56 # int | Less than or equal to; number (optional)
    gbd_wijk_volgnummer_not = [56] # List[int] | Exclude matches; number (optional)
    id = 56 # int | Identificerend kenmerk van het ticket. (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    items_definitief = 'items_definitief_example' # str | De onderdelen en de werkzaamheden zoals deze op de factuur vermeld worden. (optional)
    items_definitief_in = ['items_definitief_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    items_definitief_isempty = True # bool | Whether the field is empty or not. (optional)
    items_definitief_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    items_definitief_like = 'items_definitief_like_example' # str | Matches text using wildcards (? and *). (optional)
    items_definitief_not = ['items_definitief_not_example'] # List[str] | Exclude matches; text (optional)
    items_offerte = 'items_offerte_example' # str | De onderdelen en de werkzaamheden zoals deze op de offerte vermeld worden. (optional)
    items_offerte_in = ['items_offerte_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    items_offerte_isempty = True # bool | Whether the field is empty or not. (optional)
    items_offerte_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    items_offerte_like = 'items_offerte_like_example' # str | Matches text using wildcards (? and *). (optional)
    items_offerte_not = ['items_offerte_not_example'] # List[str] | Exclude matches; text (optional)
    onderhoudsbedrijf = 'onderhoudsbedrijf_example' # str | De naam van het onderhoudsbedrijf. (optional)
    onderhoudsbedrijf_in = ['onderhoudsbedrijf_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    onderhoudsbedrijf_isempty = True # bool | Whether the field is empty or not. (optional)
    onderhoudsbedrijf_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    onderhoudsbedrijf_like = 'onderhoudsbedrijf_like_example' # str | Matches text using wildcards (? and *). (optional)
    onderhoudsbedrijf_not = ['onderhoudsbedrijf_not_example'] # List[str] | Exclude matches; text (optional)
    oorzaak = ['oorzaak_example'] # List[str] | Exact; val1,val2 (optional)
    oorzaak_contains = ['oorzaak_contains_example'] # List[str] | Matches values from a comma-separated list: val1,val2,valN. (optional)
    oplossing = ['oplossing_example'] # List[str] | Exact; val1,val2 (optional)
    oplossing_contains = ['oplossing_contains_example'] # List[str] | Matches values from a comma-separated list: val1,val2,valN. (optional)
    page = 56 # int | A page number within the paginated result set. (optional)
    prijs = 3.4 # float | De totale prijs van de gebruikte onderdelen en de uitgevoerde werkzaamheden. (optional)
    prijs_offerte = 3.4 # float | De totale prijs op de offerte voor de te gebruiken onderdelen en de uit te voeren werkzaamheden. (optional)
    prijs_offerte_gt = 3.4 # float | Greater than; number (optional)
    prijs_offerte_gte = 3.4 # float | Greater than or equal to; number (optional)
    prijs_offerte_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prijs_offerte_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prijs_offerte_lt = 3.4 # float | Less than; number (optional)
    prijs_offerte_lte = 3.4 # float | Less than or equal to; number (optional)
    prijs_offerte_not = [3.4] # List[float] | Exclude matches; number (optional)
    prijs_gt = 3.4 # float | Greater than; number (optional)
    prijs_gte = 3.4 # float | Greater than or equal to; number (optional)
    prijs_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prijs_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prijs_lt = 3.4 # float | Less than; number (optional)
    prijs_lte = 3.4 # float | Less than or equal to; number (optional)
    prijs_not = [3.4] # List[float] | Exclude matches; number (optional)
    prioriteit_naam = 'prioriteit_naam_example' # str | De naam die de soort prioriteit weergeeft. (optional)
    prioriteit_naam_in = ['prioriteit_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prioriteit_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    prioriteit_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prioriteit_naam_like = 'prioriteit_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    prioriteit_naam_not = ['prioriteit_naam_not_example'] # List[str] | Exclude matches; text (optional)
    prioriteit_opmerking = 'prioriteit_opmerking_example' # str | Een opmerking die toegevoegd wordt om de prioritering te verduidelijken. (optional)
    prioriteit_opmerking_in = ['prioriteit_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prioriteit_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    prioriteit_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prioriteit_opmerking_like = 'prioriteit_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    prioriteit_opmerking_not = ['prioriteit_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    prioriteit_responstijd = 56 # int | De toegestane responsetijd voor deze prioriteit.  (optional)
    prioriteit_responstijd_gt = 56 # int | Greater than; number (optional)
    prioriteit_responstijd_gte = 56 # int | Greater than or equal to; number (optional)
    prioriteit_responstijd_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prioriteit_responstijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prioriteit_responstijd_lt = 56 # int | Less than; number (optional)
    prioriteit_responstijd_lte = 56 # int | Less than or equal to; number (optional)
    prioriteit_responstijd_not = [56] # List[int] | Exclude matches; number (optional)
    probleem = ['probleem_example'] # List[str] | Exact; val1,val2 (optional)
    probleem_module_naam = ['probleem_module_naam_example'] # List[str] | Exact; val1,val2 (optional)
    probleem_module_naam_contains = ['probleem_module_naam_contains_example'] # List[str] | Matches values from a comma-separated list: val1,val2,valN. (optional)
    probleem_contains = ['probleem_contains_example'] # List[str] | Matches values from a comma-separated list: val1,val2,valN. (optional)
    rangorde_nummer_tickettype = 56 # int | Het rangordenummer van het type ticket. (optional)
    rangorde_nummer_tickettype_gt = 56 # int | Greater than; number (optional)
    rangorde_nummer_tickettype_gte = 56 # int | Greater than or equal to; number (optional)
    rangorde_nummer_tickettype_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    rangorde_nummer_tickettype_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    rangorde_nummer_tickettype_lt = 56 # int | Less than; number (optional)
    rangorde_nummer_tickettype_lte = 56 # int | Less than or equal to; number (optional)
    rangorde_nummer_tickettype_not = [56] # List[int] | Exclude matches; number (optional)
    reden_afgewezen = 'reden_afgewezen_example' # str | De reden waarom het ticket de status 'afgewezen' heeft gekregen. (optional)
    reden_afgewezen_in = ['reden_afgewezen_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    reden_afgewezen_isempty = True # bool | Whether the field is empty or not. (optional)
    reden_afgewezen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    reden_afgewezen_like = 'reden_afgewezen_like_example' # str | Matches text using wildcards (? and *). (optional)
    reden_afgewezen_not = ['reden_afgewezen_not_example'] # List[str] | Exclude matches; text (optional)
    referentienummer_leverancier = 'referentienummer_leverancier_example' # str | Het referentienummer dat door de leverancier aan het ticket gegeven wordt. (optional)
    referentienummer_leverancier_in = ['referentienummer_leverancier_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    referentienummer_leverancier_isempty = True # bool | Whether the field is empty or not. (optional)
    referentienummer_leverancier_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    referentienummer_leverancier_like = 'referentienummer_leverancier_like_example' # str | Matches text using wildcards (? and *). (optional)
    referentienummer_leverancier_not = ['referentienummer_leverancier_not_example'] # List[str] | Exclude matches; text (optional)
    ticketstatus = 'ticketstatus_example' # str | De status van het ticket. (optional)
    ticketstatus_in = ['ticketstatus_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    ticketstatus_isempty = True # bool | Whether the field is empty or not. (optional)
    ticketstatus_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    ticketstatus_like = 'ticketstatus_like_example' # str | Matches text using wildcards (? and *). (optional)
    ticketstatus_not = ['ticketstatus_not_example'] # List[str] | Exclude matches; text (optional)
    tickettype = 'tickettype_example' # str | De naam van het type ticket. (optional)
    tickettype_in = ['tickettype_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    tickettype_isempty = True # bool | Whether the field is empty or not. (optional)
    tickettype_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    tickettype_like = 'tickettype_like_example' # str | Matches text using wildcards (? and *). (optional)
    tickettype_not = ['tickettype_not_example'] # List[str] | Exclude matches; text (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_ticket_list2(accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, count=count, expand=expand, expand_scope=expand_scope, fields=fields, format=format, page_size=page_size, sort=sort, container_id=container_id, container_id_in=container_id_in, container_id_isempty=container_id_isempty, container_id_isnull=container_id_isnull, container_id_like=container_id_like, container_id_not=container_id_not, containerlocatie_id=containerlocatie_id, containerlocatie_id_in=containerlocatie_id_in, containerlocatie_id_isempty=containerlocatie_id_isempty, containerlocatie_id_isnull=containerlocatie_id_isnull, containerlocatie_id_like=containerlocatie_id_like, containerlocatie_id_not=containerlocatie_id_not, datum_afgerond=datum_afgerond, datum_afgerond_gt=datum_afgerond_gt, datum_afgerond_gte=datum_afgerond_gte, datum_afgerond_in=datum_afgerond_in, datum_afgerond_isnull=datum_afgerond_isnull, datum_afgerond_lt=datum_afgerond_lt, datum_afgerond_lte=datum_afgerond_lte, datum_afgerond_not=datum_afgerond_not, datum_afgewezen=datum_afgewezen, datum_afgewezen_gt=datum_afgewezen_gt, datum_afgewezen_gte=datum_afgewezen_gte, datum_afgewezen_in=datum_afgewezen_in, datum_afgewezen_isnull=datum_afgewezen_isnull, datum_afgewezen_lt=datum_afgewezen_lt, datum_afgewezen_lte=datum_afgewezen_lte, datum_afgewezen_not=datum_afgewezen_not, datum_creatie=datum_creatie, datum_creatie_gt=datum_creatie_gt, datum_creatie_gte=datum_creatie_gte, datum_creatie_in=datum_creatie_in, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_lt=datum_creatie_lt, datum_creatie_lte=datum_creatie_lte, datum_creatie_not=datum_creatie_not, datum_factuur=datum_factuur, datum_factuur_gt=datum_factuur_gt, datum_factuur_gte=datum_factuur_gte, datum_factuur_in=datum_factuur_in, datum_factuur_isnull=datum_factuur_isnull, datum_factuur_lt=datum_factuur_lt, datum_factuur_lte=datum_factuur_lte, datum_factuur_not=datum_factuur_not, datum_financiele_goedkeuring=datum_financiele_goedkeuring, datum_financiele_goedkeuring_gt=datum_financiele_goedkeuring_gt, datum_financiele_goedkeuring_gte=datum_financiele_goedkeuring_gte, datum_financiele_goedkeuring_in=datum_financiele_goedkeuring_in, datum_financiele_goedkeuring_isnull=datum_financiele_goedkeuring_isnull, datum_financiele_goedkeuring_lt=datum_financiele_goedkeuring_lt, datum_financiele_goedkeuring_lte=datum_financiele_goedkeuring_lte, datum_financiele_goedkeuring_not=datum_financiele_goedkeuring_not, datum_geaccepteerd=datum_geaccepteerd, datum_geaccepteerd_gt=datum_geaccepteerd_gt, datum_geaccepteerd_gte=datum_geaccepteerd_gte, datum_geaccepteerd_in=datum_geaccepteerd_in, datum_geaccepteerd_isnull=datum_geaccepteerd_isnull, datum_geaccepteerd_lt=datum_geaccepteerd_lt, datum_geaccepteerd_lte=datum_geaccepteerd_lte, datum_geaccepteerd_not=datum_geaccepteerd_not, datum_gefactureerd=datum_gefactureerd, datum_gefactureerd_gt=datum_gefactureerd_gt, datum_gefactureerd_gte=datum_gefactureerd_gte, datum_gefactureerd_in=datum_gefactureerd_in, datum_gefactureerd_isnull=datum_gefactureerd_isnull, datum_gefactureerd_lt=datum_gefactureerd_lt, datum_gefactureerd_lte=datum_gefactureerd_lte, datum_gefactureerd_not=datum_gefactureerd_not, datum_gepland=datum_gepland, datum_gepland_gt=datum_gepland_gt, datum_gepland_gte=datum_gepland_gte, datum_gepland_in=datum_gepland_in, datum_gepland_isnull=datum_gepland_isnull, datum_gepland_lt=datum_gepland_lt, datum_gepland_lte=datum_gepland_lte, datum_gepland_not=datum_gepland_not, datum_gereed=datum_gereed, datum_gereed_gt=datum_gereed_gt, datum_gereed_gte=datum_gereed_gte, datum_gereed_in=datum_gereed_in, datum_gereed_isnull=datum_gereed_isnull, datum_gereed_lt=datum_gereed_lt, datum_gereed_lte=datum_gereed_lte, datum_gereed_not=datum_gereed_not, datum_offerte=datum_offerte, datum_offerte_gt=datum_offerte_gt, datum_offerte_gte=datum_offerte_gte, datum_offerte_in=datum_offerte_in, datum_offerte_isnull=datum_offerte_isnull, datum_offerte_lt=datum_offerte_lt, datum_offerte_lte=datum_offerte_lte, datum_offerte_not=datum_offerte_not, datum_technische_goedkeuring=datum_technische_goedkeuring, datum_technische_goedkeuring_gt=datum_technische_goedkeuring_gt, datum_technische_goedkeuring_gte=datum_technische_goedkeuring_gte, datum_technische_goedkeuring_in=datum_technische_goedkeuring_in, datum_technische_goedkeuring_isnull=datum_technische_goedkeuring_isnull, datum_technische_goedkeuring_lt=datum_technische_goedkeuring_lt, datum_technische_goedkeuring_lte=datum_technische_goedkeuring_lte, datum_technische_goedkeuring_not=datum_technische_goedkeuring_not, datum_wijziging=datum_wijziging, datum_wijziging_gt=datum_wijziging_gt, datum_wijziging_gte=datum_wijziging_gte, datum_wijziging_in=datum_wijziging_in, datum_wijziging_isnull=datum_wijziging_isnull, datum_wijziging_lt=datum_wijziging_lt, datum_wijziging_lte=datum_wijziging_lte, datum_wijziging_not=datum_wijziging_not, datum_workflow_start=datum_workflow_start, datum_workflow_start_gt=datum_workflow_start_gt, datum_workflow_start_gte=datum_workflow_start_gte, datum_workflow_start_in=datum_workflow_start_in, datum_workflow_start_isnull=datum_workflow_start_isnull, datum_workflow_start_lt=datum_workflow_start_lt, datum_workflow_start_lte=datum_workflow_start_lte, datum_workflow_start_not=datum_workflow_start_not, doorlooptijd=doorlooptijd, doorlooptijd_in=doorlooptijd_in, doorlooptijd_isempty=doorlooptijd_isempty, doorlooptijd_isnull=doorlooptijd_isnull, doorlooptijd_like=doorlooptijd_like, doorlooptijd_not=doorlooptijd_not, eigenaar=eigenaar, eigenaar_in=eigenaar_in, eigenaar_isempty=eigenaar_isempty, eigenaar_isnull=eigenaar_isnull, eigenaar_like=eigenaar_like, eigenaar_not=eigenaar_not, factuur_nummer=factuur_nummer, factuur_nummer_in=factuur_nummer_in, factuur_nummer_isempty=factuur_nummer_isempty, factuur_nummer_isnull=factuur_nummer_isnull, factuur_nummer_like=factuur_nummer_like, factuur_nummer_not=factuur_nummer_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, gbd_buurt_code=gbd_buurt_code, gbd_buurt_code_in=gbd_buurt_code_in, gbd_buurt_code_isempty=gbd_buurt_code_isempty, gbd_buurt_code_isnull=gbd_buurt_code_isnull, gbd_buurt_code_like=gbd_buurt_code_like, gbd_buurt_code_not=gbd_buurt_code_not, gbd_buurt_naam=gbd_buurt_naam, gbd_buurt_naam_in=gbd_buurt_naam_in, gbd_buurt_naam_isempty=gbd_buurt_naam_isempty, gbd_buurt_naam_isnull=gbd_buurt_naam_isnull, gbd_buurt_naam_like=gbd_buurt_naam_like, gbd_buurt_naam_not=gbd_buurt_naam_not, gbd_buurt_volgnummer=gbd_buurt_volgnummer, gbd_buurt_volgnummer_gt=gbd_buurt_volgnummer_gt, gbd_buurt_volgnummer_gte=gbd_buurt_volgnummer_gte, gbd_buurt_volgnummer_in=gbd_buurt_volgnummer_in, gbd_buurt_volgnummer_isnull=gbd_buurt_volgnummer_isnull, gbd_buurt_volgnummer_lt=gbd_buurt_volgnummer_lt, gbd_buurt_volgnummer_lte=gbd_buurt_volgnummer_lte, gbd_buurt_volgnummer_not=gbd_buurt_volgnummer_not, gbd_ggw_identificatie=gbd_ggw_identificatie, gbd_ggw_identificatie_in=gbd_ggw_identificatie_in, gbd_ggw_identificatie_isempty=gbd_ggw_identificatie_isempty, gbd_ggw_identificatie_isnull=gbd_ggw_identificatie_isnull, gbd_ggw_identificatie_like=gbd_ggw_identificatie_like, gbd_ggw_identificatie_not=gbd_ggw_identificatie_not, gbd_ggw_naam=gbd_ggw_naam, gbd_ggw_naam_in=gbd_ggw_naam_in, gbd_ggw_naam_isempty=gbd_ggw_naam_isempty, gbd_ggw_naam_isnull=gbd_ggw_naam_isnull, gbd_ggw_naam_like=gbd_ggw_naam_like, gbd_ggw_naam_not=gbd_ggw_naam_not, gbd_ggw_volgnummer=gbd_ggw_volgnummer, gbd_ggw_volgnummer_in=gbd_ggw_volgnummer_in, gbd_ggw_volgnummer_isempty=gbd_ggw_volgnummer_isempty, gbd_ggw_volgnummer_isnull=gbd_ggw_volgnummer_isnull, gbd_ggw_volgnummer_like=gbd_ggw_volgnummer_like, gbd_ggw_volgnummer_not=gbd_ggw_volgnummer_not, gbd_stadsdeel_identificatie=gbd_stadsdeel_identificatie, gbd_stadsdeel_identificatie_in=gbd_stadsdeel_identificatie_in, gbd_stadsdeel_identificatie_isempty=gbd_stadsdeel_identificatie_isempty, gbd_stadsdeel_identificatie_isnull=gbd_stadsdeel_identificatie_isnull, gbd_stadsdeel_identificatie_like=gbd_stadsdeel_identificatie_like, gbd_stadsdeel_identificatie_not=gbd_stadsdeel_identificatie_not, gbd_stadsdeel_naam=gbd_stadsdeel_naam, gbd_stadsdeel_naam_in=gbd_stadsdeel_naam_in, gbd_stadsdeel_naam_isempty=gbd_stadsdeel_naam_isempty, gbd_stadsdeel_naam_isnull=gbd_stadsdeel_naam_isnull, gbd_stadsdeel_naam_like=gbd_stadsdeel_naam_like, gbd_stadsdeel_naam_not=gbd_stadsdeel_naam_not, gbd_stadsdeel_volgnummer=gbd_stadsdeel_volgnummer, gbd_stadsdeel_volgnummer_gt=gbd_stadsdeel_volgnummer_gt, gbd_stadsdeel_volgnummer_gte=gbd_stadsdeel_volgnummer_gte, gbd_stadsdeel_volgnummer_in=gbd_stadsdeel_volgnummer_in, gbd_stadsdeel_volgnummer_isnull=gbd_stadsdeel_volgnummer_isnull, gbd_stadsdeel_volgnummer_lt=gbd_stadsdeel_volgnummer_lt, gbd_stadsdeel_volgnummer_lte=gbd_stadsdeel_volgnummer_lte, gbd_stadsdeel_volgnummer_not=gbd_stadsdeel_volgnummer_not, gbd_wijk_identificatie=gbd_wijk_identificatie, gbd_wijk_identificatie_in=gbd_wijk_identificatie_in, gbd_wijk_identificatie_isempty=gbd_wijk_identificatie_isempty, gbd_wijk_identificatie_isnull=gbd_wijk_identificatie_isnull, gbd_wijk_identificatie_like=gbd_wijk_identificatie_like, gbd_wijk_identificatie_not=gbd_wijk_identificatie_not, gbd_wijk_naam=gbd_wijk_naam, gbd_wijk_naam_in=gbd_wijk_naam_in, gbd_wijk_naam_isempty=gbd_wijk_naam_isempty, gbd_wijk_naam_isnull=gbd_wijk_naam_isnull, gbd_wijk_naam_like=gbd_wijk_naam_like, gbd_wijk_naam_not=gbd_wijk_naam_not, gbd_wijk_volgnummer=gbd_wijk_volgnummer, gbd_wijk_volgnummer_gt=gbd_wijk_volgnummer_gt, gbd_wijk_volgnummer_gte=gbd_wijk_volgnummer_gte, gbd_wijk_volgnummer_in=gbd_wijk_volgnummer_in, gbd_wijk_volgnummer_isnull=gbd_wijk_volgnummer_isnull, gbd_wijk_volgnummer_lt=gbd_wijk_volgnummer_lt, gbd_wijk_volgnummer_lte=gbd_wijk_volgnummer_lte, gbd_wijk_volgnummer_not=gbd_wijk_volgnummer_not, id=id, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, items_definitief=items_definitief, items_definitief_in=items_definitief_in, items_definitief_isempty=items_definitief_isempty, items_definitief_isnull=items_definitief_isnull, items_definitief_like=items_definitief_like, items_definitief_not=items_definitief_not, items_offerte=items_offerte, items_offerte_in=items_offerte_in, items_offerte_isempty=items_offerte_isempty, items_offerte_isnull=items_offerte_isnull, items_offerte_like=items_offerte_like, items_offerte_not=items_offerte_not, onderhoudsbedrijf=onderhoudsbedrijf, onderhoudsbedrijf_in=onderhoudsbedrijf_in, onderhoudsbedrijf_isempty=onderhoudsbedrijf_isempty, onderhoudsbedrijf_isnull=onderhoudsbedrijf_isnull, onderhoudsbedrijf_like=onderhoudsbedrijf_like, onderhoudsbedrijf_not=onderhoudsbedrijf_not, oorzaak=oorzaak, oorzaak_contains=oorzaak_contains, oplossing=oplossing, oplossing_contains=oplossing_contains, page=page, prijs=prijs, prijs_offerte=prijs_offerte, prijs_offerte_gt=prijs_offerte_gt, prijs_offerte_gte=prijs_offerte_gte, prijs_offerte_in=prijs_offerte_in, prijs_offerte_isnull=prijs_offerte_isnull, prijs_offerte_lt=prijs_offerte_lt, prijs_offerte_lte=prijs_offerte_lte, prijs_offerte_not=prijs_offerte_not, prijs_gt=prijs_gt, prijs_gte=prijs_gte, prijs_in=prijs_in, prijs_isnull=prijs_isnull, prijs_lt=prijs_lt, prijs_lte=prijs_lte, prijs_not=prijs_not, prioriteit_naam=prioriteit_naam, prioriteit_naam_in=prioriteit_naam_in, prioriteit_naam_isempty=prioriteit_naam_isempty, prioriteit_naam_isnull=prioriteit_naam_isnull, prioriteit_naam_like=prioriteit_naam_like, prioriteit_naam_not=prioriteit_naam_not, prioriteit_opmerking=prioriteit_opmerking, prioriteit_opmerking_in=prioriteit_opmerking_in, prioriteit_opmerking_isempty=prioriteit_opmerking_isempty, prioriteit_opmerking_isnull=prioriteit_opmerking_isnull, prioriteit_opmerking_like=prioriteit_opmerking_like, prioriteit_opmerking_not=prioriteit_opmerking_not, prioriteit_responstijd=prioriteit_responstijd, prioriteit_responstijd_gt=prioriteit_responstijd_gt, prioriteit_responstijd_gte=prioriteit_responstijd_gte, prioriteit_responstijd_in=prioriteit_responstijd_in, prioriteit_responstijd_isnull=prioriteit_responstijd_isnull, prioriteit_responstijd_lt=prioriteit_responstijd_lt, prioriteit_responstijd_lte=prioriteit_responstijd_lte, prioriteit_responstijd_not=prioriteit_responstijd_not, probleem=probleem, probleem_module_naam=probleem_module_naam, probleem_module_naam_contains=probleem_module_naam_contains, probleem_contains=probleem_contains, rangorde_nummer_tickettype=rangorde_nummer_tickettype, rangorde_nummer_tickettype_gt=rangorde_nummer_tickettype_gt, rangorde_nummer_tickettype_gte=rangorde_nummer_tickettype_gte, rangorde_nummer_tickettype_in=rangorde_nummer_tickettype_in, rangorde_nummer_tickettype_isnull=rangorde_nummer_tickettype_isnull, rangorde_nummer_tickettype_lt=rangorde_nummer_tickettype_lt, rangorde_nummer_tickettype_lte=rangorde_nummer_tickettype_lte, rangorde_nummer_tickettype_not=rangorde_nummer_tickettype_not, reden_afgewezen=reden_afgewezen, reden_afgewezen_in=reden_afgewezen_in, reden_afgewezen_isempty=reden_afgewezen_isempty, reden_afgewezen_isnull=reden_afgewezen_isnull, reden_afgewezen_like=reden_afgewezen_like, reden_afgewezen_not=reden_afgewezen_not, referentienummer_leverancier=referentienummer_leverancier, referentienummer_leverancier_in=referentienummer_leverancier_in, referentienummer_leverancier_isempty=referentienummer_leverancier_isempty, referentienummer_leverancier_isnull=referentienummer_leverancier_isnull, referentienummer_leverancier_like=referentienummer_leverancier_like, referentienummer_leverancier_not=referentienummer_leverancier_not, ticketstatus=ticketstatus, ticketstatus_in=ticketstatus_in, ticketstatus_isempty=ticketstatus_isempty, ticketstatus_isnull=ticketstatus_isnull, ticketstatus_like=ticketstatus_like, ticketstatus_not=ticketstatus_not, tickettype=tickettype, tickettype_in=tickettype_in, tickettype_isempty=tickettype_isempty, tickettype_isnull=tickettype_isnull, tickettype_like=tickettype_like, tickettype_not=tickettype_not)
        print("The response of TicketApi->huishoudelijkafval_ticket_list2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TicketApi->huishoudelijkafval_ticket_list2: %s\n" % e)
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
 **container_id** | **str**| Unieke aanduiding objecttype | [optional] 
 **container_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_id** | **str**| Identificerend kenmerk van de put waarin de container is geplaatst | [optional] 
 **containerlocatie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_afgerond** | **datetime**| De datum waarop de werkzaamheden als gereed aangegeven zijn door het onderhoudsbedrijf. | [optional] 
 **datum_afgerond_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgerond_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgerond_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_afgerond_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_afgerond_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgerond_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgerond_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen** | **datetime**| De datum waarop het ticket de status &#39;afgewezen&#39; krijgt. | [optional] 
 **datum_afgewezen_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_afgewezen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_afgewezen_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie** | **datetime**| De datum waarop het ticket aangemaakt is. | [optional] 
 **datum_creatie_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_creatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_creatie_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur** | **datetime**| De datum waarop het ticket gefactureerd is. | [optional] 
 **datum_factuur_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_factuur_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_factuur_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring** | **datetime**| De datum waarop de financiale aspecten van de werkzaamheden goed- of afgekeurd zijn. | [optional] 
 **datum_financiele_goedkeuring_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_financiele_goedkeuring_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_financiele_goedkeuring_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd** | **datetime**| De datum waarop het ticket geaccepteerd is door het onderhoudsbedrijf. | [optional] 
 **datum_geaccepteerd_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_geaccepteerd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_geaccepteerd_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd** | **datetime**| De datum waarop de factuur in het systeem de status &#39;gefactureerd&#39; krijgt. | [optional] 
 **datum_gefactureerd_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_gefactureerd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_gefactureerd_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland** | **datetime**| De datum waarop de uitvoering van de werkzaamheden is ingepland. | [optional] 
 **datum_gepland_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_gepland_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_gepland_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed** | **datetime**| De datum waarop de werkzaamheden uitgevoerd zijn. | [optional] 
 **datum_gereed_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_gereed_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_gereed_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte** | **datetime**| De datum waarop de offerte is aangemaakt . | [optional] 
 **datum_offerte_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_offerte_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_offerte_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring** | **datetime**| De datum waarop de technische aspecten van de werkzaamheden goed- of afgekeurd zijn. | [optional] 
 **datum_technische_goedkeuring_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_technische_goedkeuring_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_technische_goedkeuring_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging** | **datetime**| De datum waarop het ticket is gewijzigd. | [optional] 
 **datum_wijziging_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_wijziging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_wijziging_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start** | **datetime**| De datum waarop de workflow start. | [optional] 
 **datum_workflow_start_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_workflow_start_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_workflow_start_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **doorlooptijd** | **str**| De tijdsspanne in werkdagen tussen de &#39;datumCreatie&#39;en de &#39;datumAfgerond&#39; of de tijdsspanne in werkdagen tussen de &#39;datumCreatie&#39; en de laatste statuswijziging in het geval het ticket nog niet afgerond is. | [optional] 
 **doorlooptijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **doorlooptijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **doorlooptijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **doorlooptijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **doorlooptijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **eigenaar** | **str**| De naam van de eigenaar van de container. | [optional] 
 **eigenaar_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **eigenaar_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **eigenaar_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **eigenaar_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **eigenaar_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **factuur_nummer** | **str**| Het nummer van de factuur. | [optional] 
 **factuur_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **factuur_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **factuur_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **factuur_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **factuur_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_code** | **str**| Unieke code. | [optional] 
 **gbd_buurt_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_naam** | **str**| De naam van het object. | [optional] 
 **gbd_buurt_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_volgnummer** | **int**| Uniek volgnummer van de toestand van het object. | [optional] 
 **gbd_buurt_volgnummer_gt** | **int**| Greater than; number | [optional] 
 **gbd_buurt_volgnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **gbd_buurt_volgnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_volgnummer_lt** | **int**| Less than; number | [optional] 
 **gbd_buurt_volgnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **gbd_buurt_volgnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **gbd_ggw_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_ggw_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_ggw_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_ggw_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_ggw_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_ggw_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_ggw_naam** | **str**| De naam van het object. | [optional] 
 **gbd_ggw_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_ggw_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_ggw_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_ggw_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_ggw_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_ggw_volgnummer** | **str**| Uniek volgnummer van de toestand van het object. | [optional] 
 **gbd_ggw_volgnummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_ggw_volgnummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_ggw_volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_ggw_volgnummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_ggw_volgnummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_stadsdeel_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_stadsdeel_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_stadsdeel_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_stadsdeel_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_stadsdeel_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_stadsdeel_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_stadsdeel_naam** | **str**| De naam van het object. | [optional] 
 **gbd_stadsdeel_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_stadsdeel_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_stadsdeel_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_stadsdeel_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_stadsdeel_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_stadsdeel_volgnummer** | **int**| Uniek volgnummer van de toestand van het object. | [optional] 
 **gbd_stadsdeel_volgnummer_gt** | **int**| Greater than; number | [optional] 
 **gbd_stadsdeel_volgnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **gbd_stadsdeel_volgnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_stadsdeel_volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_stadsdeel_volgnummer_lt** | **int**| Less than; number | [optional] 
 **gbd_stadsdeel_volgnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **gbd_stadsdeel_volgnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **gbd_wijk_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_wijk_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_wijk_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_wijk_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_wijk_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_wijk_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_wijk_naam** | **str**| De naam van het object. | [optional] 
 **gbd_wijk_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_wijk_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_wijk_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_wijk_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_wijk_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_wijk_volgnummer** | **int**| Uniek volgnummer van de toestand van het object. | [optional] 
 **gbd_wijk_volgnummer_gt** | **int**| Greater than; number | [optional] 
 **gbd_wijk_volgnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **gbd_wijk_volgnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_wijk_volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_wijk_volgnummer_lt** | **int**| Less than; number | [optional] 
 **gbd_wijk_volgnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **gbd_wijk_volgnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **id** | **int**| Identificerend kenmerk van het ticket. | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **items_definitief** | **str**| De onderdelen en de werkzaamheden zoals deze op de factuur vermeld worden. | [optional] 
 **items_definitief_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **items_definitief_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **items_definitief_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **items_definitief_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **items_definitief_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **items_offerte** | **str**| De onderdelen en de werkzaamheden zoals deze op de offerte vermeld worden. | [optional] 
 **items_offerte_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **items_offerte_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **items_offerte_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **items_offerte_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **items_offerte_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **onderhoudsbedrijf** | **str**| De naam van het onderhoudsbedrijf. | [optional] 
 **onderhoudsbedrijf_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **onderhoudsbedrijf_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **onderhoudsbedrijf_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **onderhoudsbedrijf_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **onderhoudsbedrijf_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **oorzaak** | [**List[str]**](str.md)| Exact; val1,val2 | [optional] 
 **oorzaak_contains** | [**List[str]**](str.md)| Matches values from a comma-separated list: val1,val2,valN. | [optional] 
 **oplossing** | [**List[str]**](str.md)| Exact; val1,val2 | [optional] 
 **oplossing_contains** | [**List[str]**](str.md)| Matches values from a comma-separated list: val1,val2,valN. | [optional] 
 **page** | **int**| A page number within the paginated result set. | [optional] 
 **prijs** | **float**| De totale prijs van de gebruikte onderdelen en de uitgevoerde werkzaamheden. | [optional] 
 **prijs_offerte** | **float**| De totale prijs op de offerte voor de te gebruiken onderdelen en de uit te voeren werkzaamheden. | [optional] 
 **prijs_offerte_gt** | **float**| Greater than; number | [optional] 
 **prijs_offerte_gte** | **float**| Greater than or equal to; number | [optional] 
 **prijs_offerte_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prijs_offerte_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prijs_offerte_lt** | **float**| Less than; number | [optional] 
 **prijs_offerte_lte** | **float**| Less than or equal to; number | [optional] 
 **prijs_offerte_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **prijs_gt** | **float**| Greater than; number | [optional] 
 **prijs_gte** | **float**| Greater than or equal to; number | [optional] 
 **prijs_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prijs_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prijs_lt** | **float**| Less than; number | [optional] 
 **prijs_lte** | **float**| Less than or equal to; number | [optional] 
 **prijs_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **prioriteit_naam** | **str**| De naam die de soort prioriteit weergeeft. | [optional] 
 **prioriteit_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prioriteit_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **prioriteit_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prioriteit_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **prioriteit_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **prioriteit_opmerking** | **str**| Een opmerking die toegevoegd wordt om de prioritering te verduidelijken. | [optional] 
 **prioriteit_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prioriteit_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **prioriteit_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prioriteit_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **prioriteit_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **prioriteit_responstijd** | **int**| De toegestane responsetijd voor deze prioriteit.  | [optional] 
 **prioriteit_responstijd_gt** | **int**| Greater than; number | [optional] 
 **prioriteit_responstijd_gte** | **int**| Greater than or equal to; number | [optional] 
 **prioriteit_responstijd_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prioriteit_responstijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prioriteit_responstijd_lt** | **int**| Less than; number | [optional] 
 **prioriteit_responstijd_lte** | **int**| Less than or equal to; number | [optional] 
 **prioriteit_responstijd_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **probleem** | [**List[str]**](str.md)| Exact; val1,val2 | [optional] 
 **probleem_module_naam** | [**List[str]**](str.md)| Exact; val1,val2 | [optional] 
 **probleem_module_naam_contains** | [**List[str]**](str.md)| Matches values from a comma-separated list: val1,val2,valN. | [optional] 
 **probleem_contains** | [**List[str]**](str.md)| Matches values from a comma-separated list: val1,val2,valN. | [optional] 
 **rangorde_nummer_tickettype** | **int**| Het rangordenummer van het type ticket. | [optional] 
 **rangorde_nummer_tickettype_gt** | **int**| Greater than; number | [optional] 
 **rangorde_nummer_tickettype_gte** | **int**| Greater than or equal to; number | [optional] 
 **rangorde_nummer_tickettype_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **rangorde_nummer_tickettype_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **rangorde_nummer_tickettype_lt** | **int**| Less than; number | [optional] 
 **rangorde_nummer_tickettype_lte** | **int**| Less than or equal to; number | [optional] 
 **rangorde_nummer_tickettype_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **reden_afgewezen** | **str**| De reden waarom het ticket de status &#39;afgewezen&#39; heeft gekregen. | [optional] 
 **reden_afgewezen_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **reden_afgewezen_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **reden_afgewezen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **reden_afgewezen_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **reden_afgewezen_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **referentienummer_leverancier** | **str**| Het referentienummer dat door de leverancier aan het ticket gegeven wordt. | [optional] 
 **referentienummer_leverancier_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **referentienummer_leverancier_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **referentienummer_leverancier_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **referentienummer_leverancier_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **referentienummer_leverancier_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **ticketstatus** | **str**| De status van het ticket. | [optional] 
 **ticketstatus_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **ticketstatus_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **ticketstatus_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **ticketstatus_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **ticketstatus_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **tickettype** | **str**| De naam van het type ticket. | [optional] 
 **tickettype_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **tickettype_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **tickettype_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **tickettype_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **tickettype_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 

### Return type

[**PaginatedHuishoudelijkafvalticketList**](PaginatedHuishoudelijkafvalticketList.md)

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

# **huishoudelijkafval_ticket_retrieve2**
> Huishoudelijkafvalticket huishoudelijkafval_ticket_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, container_id=container_id, container_id_in=container_id_in, container_id_isempty=container_id_isempty, container_id_isnull=container_id_isnull, container_id_like=container_id_like, container_id_not=container_id_not, containerlocatie_id=containerlocatie_id, containerlocatie_id_in=containerlocatie_id_in, containerlocatie_id_isempty=containerlocatie_id_isempty, containerlocatie_id_isnull=containerlocatie_id_isnull, containerlocatie_id_like=containerlocatie_id_like, containerlocatie_id_not=containerlocatie_id_not, datum_afgerond=datum_afgerond, datum_afgerond_gt=datum_afgerond_gt, datum_afgerond_gte=datum_afgerond_gte, datum_afgerond_in=datum_afgerond_in, datum_afgerond_isnull=datum_afgerond_isnull, datum_afgerond_lt=datum_afgerond_lt, datum_afgerond_lte=datum_afgerond_lte, datum_afgerond_not=datum_afgerond_not, datum_afgewezen=datum_afgewezen, datum_afgewezen_gt=datum_afgewezen_gt, datum_afgewezen_gte=datum_afgewezen_gte, datum_afgewezen_in=datum_afgewezen_in, datum_afgewezen_isnull=datum_afgewezen_isnull, datum_afgewezen_lt=datum_afgewezen_lt, datum_afgewezen_lte=datum_afgewezen_lte, datum_afgewezen_not=datum_afgewezen_not, datum_creatie=datum_creatie, datum_creatie_gt=datum_creatie_gt, datum_creatie_gte=datum_creatie_gte, datum_creatie_in=datum_creatie_in, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_lt=datum_creatie_lt, datum_creatie_lte=datum_creatie_lte, datum_creatie_not=datum_creatie_not, datum_factuur=datum_factuur, datum_factuur_gt=datum_factuur_gt, datum_factuur_gte=datum_factuur_gte, datum_factuur_in=datum_factuur_in, datum_factuur_isnull=datum_factuur_isnull, datum_factuur_lt=datum_factuur_lt, datum_factuur_lte=datum_factuur_lte, datum_factuur_not=datum_factuur_not, datum_financiele_goedkeuring=datum_financiele_goedkeuring, datum_financiele_goedkeuring_gt=datum_financiele_goedkeuring_gt, datum_financiele_goedkeuring_gte=datum_financiele_goedkeuring_gte, datum_financiele_goedkeuring_in=datum_financiele_goedkeuring_in, datum_financiele_goedkeuring_isnull=datum_financiele_goedkeuring_isnull, datum_financiele_goedkeuring_lt=datum_financiele_goedkeuring_lt, datum_financiele_goedkeuring_lte=datum_financiele_goedkeuring_lte, datum_financiele_goedkeuring_not=datum_financiele_goedkeuring_not, datum_geaccepteerd=datum_geaccepteerd, datum_geaccepteerd_gt=datum_geaccepteerd_gt, datum_geaccepteerd_gte=datum_geaccepteerd_gte, datum_geaccepteerd_in=datum_geaccepteerd_in, datum_geaccepteerd_isnull=datum_geaccepteerd_isnull, datum_geaccepteerd_lt=datum_geaccepteerd_lt, datum_geaccepteerd_lte=datum_geaccepteerd_lte, datum_geaccepteerd_not=datum_geaccepteerd_not, datum_gefactureerd=datum_gefactureerd, datum_gefactureerd_gt=datum_gefactureerd_gt, datum_gefactureerd_gte=datum_gefactureerd_gte, datum_gefactureerd_in=datum_gefactureerd_in, datum_gefactureerd_isnull=datum_gefactureerd_isnull, datum_gefactureerd_lt=datum_gefactureerd_lt, datum_gefactureerd_lte=datum_gefactureerd_lte, datum_gefactureerd_not=datum_gefactureerd_not, datum_gepland=datum_gepland, datum_gepland_gt=datum_gepland_gt, datum_gepland_gte=datum_gepland_gte, datum_gepland_in=datum_gepland_in, datum_gepland_isnull=datum_gepland_isnull, datum_gepland_lt=datum_gepland_lt, datum_gepland_lte=datum_gepland_lte, datum_gepland_not=datum_gepland_not, datum_gereed=datum_gereed, datum_gereed_gt=datum_gereed_gt, datum_gereed_gte=datum_gereed_gte, datum_gereed_in=datum_gereed_in, datum_gereed_isnull=datum_gereed_isnull, datum_gereed_lt=datum_gereed_lt, datum_gereed_lte=datum_gereed_lte, datum_gereed_not=datum_gereed_not, datum_offerte=datum_offerte, datum_offerte_gt=datum_offerte_gt, datum_offerte_gte=datum_offerte_gte, datum_offerte_in=datum_offerte_in, datum_offerte_isnull=datum_offerte_isnull, datum_offerte_lt=datum_offerte_lt, datum_offerte_lte=datum_offerte_lte, datum_offerte_not=datum_offerte_not, datum_technische_goedkeuring=datum_technische_goedkeuring, datum_technische_goedkeuring_gt=datum_technische_goedkeuring_gt, datum_technische_goedkeuring_gte=datum_technische_goedkeuring_gte, datum_technische_goedkeuring_in=datum_technische_goedkeuring_in, datum_technische_goedkeuring_isnull=datum_technische_goedkeuring_isnull, datum_technische_goedkeuring_lt=datum_technische_goedkeuring_lt, datum_technische_goedkeuring_lte=datum_technische_goedkeuring_lte, datum_technische_goedkeuring_not=datum_technische_goedkeuring_not, datum_wijziging=datum_wijziging, datum_wijziging_gt=datum_wijziging_gt, datum_wijziging_gte=datum_wijziging_gte, datum_wijziging_in=datum_wijziging_in, datum_wijziging_isnull=datum_wijziging_isnull, datum_wijziging_lt=datum_wijziging_lt, datum_wijziging_lte=datum_wijziging_lte, datum_wijziging_not=datum_wijziging_not, datum_workflow_start=datum_workflow_start, datum_workflow_start_gt=datum_workflow_start_gt, datum_workflow_start_gte=datum_workflow_start_gte, datum_workflow_start_in=datum_workflow_start_in, datum_workflow_start_isnull=datum_workflow_start_isnull, datum_workflow_start_lt=datum_workflow_start_lt, datum_workflow_start_lte=datum_workflow_start_lte, datum_workflow_start_not=datum_workflow_start_not, doorlooptijd=doorlooptijd, doorlooptijd_in=doorlooptijd_in, doorlooptijd_isempty=doorlooptijd_isempty, doorlooptijd_isnull=doorlooptijd_isnull, doorlooptijd_like=doorlooptijd_like, doorlooptijd_not=doorlooptijd_not, eigenaar=eigenaar, eigenaar_in=eigenaar_in, eigenaar_isempty=eigenaar_isempty, eigenaar_isnull=eigenaar_isnull, eigenaar_like=eigenaar_like, eigenaar_not=eigenaar_not, factuur_nummer=factuur_nummer, factuur_nummer_in=factuur_nummer_in, factuur_nummer_isempty=factuur_nummer_isempty, factuur_nummer_isnull=factuur_nummer_isnull, factuur_nummer_like=factuur_nummer_like, factuur_nummer_not=factuur_nummer_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, gbd_buurt_code=gbd_buurt_code, gbd_buurt_code_in=gbd_buurt_code_in, gbd_buurt_code_isempty=gbd_buurt_code_isempty, gbd_buurt_code_isnull=gbd_buurt_code_isnull, gbd_buurt_code_like=gbd_buurt_code_like, gbd_buurt_code_not=gbd_buurt_code_not, gbd_buurt_naam=gbd_buurt_naam, gbd_buurt_naam_in=gbd_buurt_naam_in, gbd_buurt_naam_isempty=gbd_buurt_naam_isempty, gbd_buurt_naam_isnull=gbd_buurt_naam_isnull, gbd_buurt_naam_like=gbd_buurt_naam_like, gbd_buurt_naam_not=gbd_buurt_naam_not, gbd_buurt_volgnummer=gbd_buurt_volgnummer, gbd_buurt_volgnummer_gt=gbd_buurt_volgnummer_gt, gbd_buurt_volgnummer_gte=gbd_buurt_volgnummer_gte, gbd_buurt_volgnummer_in=gbd_buurt_volgnummer_in, gbd_buurt_volgnummer_isnull=gbd_buurt_volgnummer_isnull, gbd_buurt_volgnummer_lt=gbd_buurt_volgnummer_lt, gbd_buurt_volgnummer_lte=gbd_buurt_volgnummer_lte, gbd_buurt_volgnummer_not=gbd_buurt_volgnummer_not, gbd_ggw_identificatie=gbd_ggw_identificatie, gbd_ggw_identificatie_in=gbd_ggw_identificatie_in, gbd_ggw_identificatie_isempty=gbd_ggw_identificatie_isempty, gbd_ggw_identificatie_isnull=gbd_ggw_identificatie_isnull, gbd_ggw_identificatie_like=gbd_ggw_identificatie_like, gbd_ggw_identificatie_not=gbd_ggw_identificatie_not, gbd_ggw_naam=gbd_ggw_naam, gbd_ggw_naam_in=gbd_ggw_naam_in, gbd_ggw_naam_isempty=gbd_ggw_naam_isempty, gbd_ggw_naam_isnull=gbd_ggw_naam_isnull, gbd_ggw_naam_like=gbd_ggw_naam_like, gbd_ggw_naam_not=gbd_ggw_naam_not, gbd_ggw_volgnummer=gbd_ggw_volgnummer, gbd_ggw_volgnummer_in=gbd_ggw_volgnummer_in, gbd_ggw_volgnummer_isempty=gbd_ggw_volgnummer_isempty, gbd_ggw_volgnummer_isnull=gbd_ggw_volgnummer_isnull, gbd_ggw_volgnummer_like=gbd_ggw_volgnummer_like, gbd_ggw_volgnummer_not=gbd_ggw_volgnummer_not, gbd_stadsdeel_identificatie=gbd_stadsdeel_identificatie, gbd_stadsdeel_identificatie_in=gbd_stadsdeel_identificatie_in, gbd_stadsdeel_identificatie_isempty=gbd_stadsdeel_identificatie_isempty, gbd_stadsdeel_identificatie_isnull=gbd_stadsdeel_identificatie_isnull, gbd_stadsdeel_identificatie_like=gbd_stadsdeel_identificatie_like, gbd_stadsdeel_identificatie_not=gbd_stadsdeel_identificatie_not, gbd_stadsdeel_naam=gbd_stadsdeel_naam, gbd_stadsdeel_naam_in=gbd_stadsdeel_naam_in, gbd_stadsdeel_naam_isempty=gbd_stadsdeel_naam_isempty, gbd_stadsdeel_naam_isnull=gbd_stadsdeel_naam_isnull, gbd_stadsdeel_naam_like=gbd_stadsdeel_naam_like, gbd_stadsdeel_naam_not=gbd_stadsdeel_naam_not, gbd_stadsdeel_volgnummer=gbd_stadsdeel_volgnummer, gbd_stadsdeel_volgnummer_gt=gbd_stadsdeel_volgnummer_gt, gbd_stadsdeel_volgnummer_gte=gbd_stadsdeel_volgnummer_gte, gbd_stadsdeel_volgnummer_in=gbd_stadsdeel_volgnummer_in, gbd_stadsdeel_volgnummer_isnull=gbd_stadsdeel_volgnummer_isnull, gbd_stadsdeel_volgnummer_lt=gbd_stadsdeel_volgnummer_lt, gbd_stadsdeel_volgnummer_lte=gbd_stadsdeel_volgnummer_lte, gbd_stadsdeel_volgnummer_not=gbd_stadsdeel_volgnummer_not, gbd_wijk_identificatie=gbd_wijk_identificatie, gbd_wijk_identificatie_in=gbd_wijk_identificatie_in, gbd_wijk_identificatie_isempty=gbd_wijk_identificatie_isempty, gbd_wijk_identificatie_isnull=gbd_wijk_identificatie_isnull, gbd_wijk_identificatie_like=gbd_wijk_identificatie_like, gbd_wijk_identificatie_not=gbd_wijk_identificatie_not, gbd_wijk_naam=gbd_wijk_naam, gbd_wijk_naam_in=gbd_wijk_naam_in, gbd_wijk_naam_isempty=gbd_wijk_naam_isempty, gbd_wijk_naam_isnull=gbd_wijk_naam_isnull, gbd_wijk_naam_like=gbd_wijk_naam_like, gbd_wijk_naam_not=gbd_wijk_naam_not, gbd_wijk_volgnummer=gbd_wijk_volgnummer, gbd_wijk_volgnummer_gt=gbd_wijk_volgnummer_gt, gbd_wijk_volgnummer_gte=gbd_wijk_volgnummer_gte, gbd_wijk_volgnummer_in=gbd_wijk_volgnummer_in, gbd_wijk_volgnummer_isnull=gbd_wijk_volgnummer_isnull, gbd_wijk_volgnummer_lt=gbd_wijk_volgnummer_lt, gbd_wijk_volgnummer_lte=gbd_wijk_volgnummer_lte, gbd_wijk_volgnummer_not=gbd_wijk_volgnummer_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, items_definitief=items_definitief, items_definitief_in=items_definitief_in, items_definitief_isempty=items_definitief_isempty, items_definitief_isnull=items_definitief_isnull, items_definitief_like=items_definitief_like, items_definitief_not=items_definitief_not, items_offerte=items_offerte, items_offerte_in=items_offerte_in, items_offerte_isempty=items_offerte_isempty, items_offerte_isnull=items_offerte_isnull, items_offerte_like=items_offerte_like, items_offerte_not=items_offerte_not, onderhoudsbedrijf=onderhoudsbedrijf, onderhoudsbedrijf_in=onderhoudsbedrijf_in, onderhoudsbedrijf_isempty=onderhoudsbedrijf_isempty, onderhoudsbedrijf_isnull=onderhoudsbedrijf_isnull, onderhoudsbedrijf_like=onderhoudsbedrijf_like, onderhoudsbedrijf_not=onderhoudsbedrijf_not, oorzaak=oorzaak, oorzaak_contains=oorzaak_contains, oplossing=oplossing, oplossing_contains=oplossing_contains, prijs=prijs, prijs_offerte=prijs_offerte, prijs_offerte_gt=prijs_offerte_gt, prijs_offerte_gte=prijs_offerte_gte, prijs_offerte_in=prijs_offerte_in, prijs_offerte_isnull=prijs_offerte_isnull, prijs_offerte_lt=prijs_offerte_lt, prijs_offerte_lte=prijs_offerte_lte, prijs_offerte_not=prijs_offerte_not, prijs_gt=prijs_gt, prijs_gte=prijs_gte, prijs_in=prijs_in, prijs_isnull=prijs_isnull, prijs_lt=prijs_lt, prijs_lte=prijs_lte, prijs_not=prijs_not, prioriteit_naam=prioriteit_naam, prioriteit_naam_in=prioriteit_naam_in, prioriteit_naam_isempty=prioriteit_naam_isempty, prioriteit_naam_isnull=prioriteit_naam_isnull, prioriteit_naam_like=prioriteit_naam_like, prioriteit_naam_not=prioriteit_naam_not, prioriteit_opmerking=prioriteit_opmerking, prioriteit_opmerking_in=prioriteit_opmerking_in, prioriteit_opmerking_isempty=prioriteit_opmerking_isempty, prioriteit_opmerking_isnull=prioriteit_opmerking_isnull, prioriteit_opmerking_like=prioriteit_opmerking_like, prioriteit_opmerking_not=prioriteit_opmerking_not, prioriteit_responstijd=prioriteit_responstijd, prioriteit_responstijd_gt=prioriteit_responstijd_gt, prioriteit_responstijd_gte=prioriteit_responstijd_gte, prioriteit_responstijd_in=prioriteit_responstijd_in, prioriteit_responstijd_isnull=prioriteit_responstijd_isnull, prioriteit_responstijd_lt=prioriteit_responstijd_lt, prioriteit_responstijd_lte=prioriteit_responstijd_lte, prioriteit_responstijd_not=prioriteit_responstijd_not, probleem=probleem, probleem_module_naam=probleem_module_naam, probleem_module_naam_contains=probleem_module_naam_contains, probleem_contains=probleem_contains, rangorde_nummer_tickettype=rangorde_nummer_tickettype, rangorde_nummer_tickettype_gt=rangorde_nummer_tickettype_gt, rangorde_nummer_tickettype_gte=rangorde_nummer_tickettype_gte, rangorde_nummer_tickettype_in=rangorde_nummer_tickettype_in, rangorde_nummer_tickettype_isnull=rangorde_nummer_tickettype_isnull, rangorde_nummer_tickettype_lt=rangorde_nummer_tickettype_lt, rangorde_nummer_tickettype_lte=rangorde_nummer_tickettype_lte, rangorde_nummer_tickettype_not=rangorde_nummer_tickettype_not, reden_afgewezen=reden_afgewezen, reden_afgewezen_in=reden_afgewezen_in, reden_afgewezen_isempty=reden_afgewezen_isempty, reden_afgewezen_isnull=reden_afgewezen_isnull, reden_afgewezen_like=reden_afgewezen_like, reden_afgewezen_not=reden_afgewezen_not, referentienummer_leverancier=referentienummer_leverancier, referentienummer_leverancier_in=referentienummer_leverancier_in, referentienummer_leverancier_isempty=referentienummer_leverancier_isempty, referentienummer_leverancier_isnull=referentienummer_leverancier_isnull, referentienummer_leverancier_like=referentienummer_leverancier_like, referentienummer_leverancier_not=referentienummer_leverancier_not, ticketstatus=ticketstatus, ticketstatus_in=ticketstatus_in, ticketstatus_isempty=ticketstatus_isempty, ticketstatus_isnull=ticketstatus_isnull, ticketstatus_like=ticketstatus_like, ticketstatus_not=ticketstatus_not, tickettype=tickettype, tickettype_in=tickettype_in, tickettype_isempty=tickettype_isempty, tickettype_isnull=tickettype_isnull, tickettype_like=tickettype_like, tickettype_not=tickettype_not)

### Example

* OAuth Authentication (oauth2):

```python
import huishoudelijkafval_api_client
from huishoudelijkafval_api_client.models.huishoudelijkafvalticket import Huishoudelijkafvalticket
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
    api_instance = huishoudelijkafval_api_client.TicketApi(api_client)
    id = 'id_example' # str | 
    accept_crs = 'accept_crs_example' # str | Accept-Crs header for Geo queries (optional)
    content_crs = 'content_crs_example' # str | Content-Crs header for Geo queries (optional)
    x_api_key = 'x_api_key_example' # str | Api Key for statistical purposes, not for authentication (optional)
    expand = True # bool | Allow to expand relations. (optional)
    expand_scope = 'container' # str | Comma separated list of named relations to expand. (optional)
    fields = 'fields_example' # str | Comma-separated list of fields to display (optional)
    format = 'format_example' # str | Select the export format (optional)
    sort = 'sort_example' # str | Which field to use when ordering the results. (optional)
    container_id = 'container_id_example' # str | Unieke aanduiding objecttype (optional)
    container_id_in = ['container_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    container_id_isempty = True # bool | Whether the field is empty or not. (optional)
    container_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    container_id_like = 'container_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    container_id_not = ['container_id_not_example'] # List[str] | Exclude matches; text (optional)
    containerlocatie_id = 'containerlocatie_id_example' # str | Identificerend kenmerk van de put waarin de container is geplaatst (optional)
    containerlocatie_id_in = ['containerlocatie_id_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    containerlocatie_id_isempty = True # bool | Whether the field is empty or not. (optional)
    containerlocatie_id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    containerlocatie_id_like = 'containerlocatie_id_like_example' # str | Matches text using wildcards (? and *). (optional)
    containerlocatie_id_not = ['containerlocatie_id_not_example'] # List[str] | Exclude matches; text (optional)
    datum_afgerond = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de werkzaamheden als gereed aangegeven zijn door het onderhoudsbedrijf. (optional)
    datum_afgerond_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgerond_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgerond_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_afgerond_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_afgerond_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgerond_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgerond_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket de status 'afgewezen' krijgt. (optional)
    datum_afgewezen_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_afgewezen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_afgewezen_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_afgewezen_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket aangemaakt is. (optional)
    datum_creatie_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_creatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_creatie_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_creatie_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket gefactureerd is. (optional)
    datum_factuur_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_factuur_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_factuur_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_factuur_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de financiale aspecten van de werkzaamheden goed- of afgekeurd zijn. (optional)
    datum_financiele_goedkeuring_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_financiele_goedkeuring_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_financiele_goedkeuring_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_financiele_goedkeuring_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket geaccepteerd is door het onderhoudsbedrijf. (optional)
    datum_geaccepteerd_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_geaccepteerd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_geaccepteerd_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_geaccepteerd_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de factuur in het systeem de status 'gefactureerd' krijgt. (optional)
    datum_gefactureerd_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_gefactureerd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_gefactureerd_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gefactureerd_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de uitvoering van de werkzaamheden is ingepland. (optional)
    datum_gepland_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_gepland_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_gepland_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gepland_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de werkzaamheden uitgevoerd zijn. (optional)
    datum_gereed_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_gereed_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_gereed_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_gereed_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de offerte is aangemaakt . (optional)
    datum_offerte_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_offerte_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_offerte_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_offerte_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de technische aspecten van de werkzaamheden goed- of afgekeurd zijn. (optional)
    datum_technische_goedkeuring_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_technische_goedkeuring_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_technische_goedkeuring_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_technische_goedkeuring_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop het ticket is gewijzigd. (optional)
    datum_wijziging_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_wijziging_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_wijziging_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_wijziging_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start = '2013-10-20T19:20:30+01:00' # datetime | De datum waarop de workflow start. (optional)
    datum_workflow_start_gt = '2013-10-20T19:20:30+01:00' # datetime | Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start_gte = '2013-10-20T19:20:30+01:00' # datetime | Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start_in = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    datum_workflow_start_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    datum_workflow_start_lt = '2013-10-20T19:20:30+01:00' # datetime | Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start_lte = '2013-10-20T19:20:30+01:00' # datetime | Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    datum_workflow_start_not = ['2013-10-20T19:20:30+01:00'] # List[datetime] | Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] (optional)
    doorlooptijd = 'doorlooptijd_example' # str | De tijdsspanne in werkdagen tussen de 'datumCreatie'en de 'datumAfgerond' of de tijdsspanne in werkdagen tussen de 'datumCreatie' en de laatste statuswijziging in het geval het ticket nog niet afgerond is. (optional)
    doorlooptijd_in = ['doorlooptijd_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    doorlooptijd_isempty = True # bool | Whether the field is empty or not. (optional)
    doorlooptijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    doorlooptijd_like = 'doorlooptijd_like_example' # str | Matches text using wildcards (? and *). (optional)
    doorlooptijd_not = ['doorlooptijd_not_example'] # List[str] | Exclude matches; text (optional)
    eigenaar = 'eigenaar_example' # str | De naam van de eigenaar van de container. (optional)
    eigenaar_in = ['eigenaar_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    eigenaar_isempty = True # bool | Whether the field is empty or not. (optional)
    eigenaar_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    eigenaar_like = 'eigenaar_like_example' # str | Matches text using wildcards (? and *). (optional)
    eigenaar_not = ['eigenaar_not_example'] # List[str] | Exclude matches; text (optional)
    factuur_nummer = 'factuur_nummer_example' # str | Het nummer van de factuur. (optional)
    factuur_nummer_in = ['factuur_nummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    factuur_nummer_isempty = True # bool | Whether the field is empty or not. (optional)
    factuur_nummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    factuur_nummer_like = 'factuur_nummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    factuur_nummer_not = ['factuur_nummer_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_identificatie = 'gbd_buurt_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_buurt_identificatie_in = ['gbd_buurt_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_identificatie_like = 'gbd_buurt_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_identificatie_not = ['gbd_buurt_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_code = 'gbd_buurt_code_example' # str | Unieke code. (optional)
    gbd_buurt_code_in = ['gbd_buurt_code_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_code_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_code_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_code_like = 'gbd_buurt_code_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_code_not = ['gbd_buurt_code_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_naam = 'gbd_buurt_naam_example' # str | De naam van het object. (optional)
    gbd_buurt_naam_in = ['gbd_buurt_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_buurt_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_naam_like = 'gbd_buurt_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_buurt_naam_not = ['gbd_buurt_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_buurt_volgnummer = 56 # int | Uniek volgnummer van de toestand van het object. (optional)
    gbd_buurt_volgnummer_gt = 56 # int | Greater than; number (optional)
    gbd_buurt_volgnummer_gte = 56 # int | Greater than or equal to; number (optional)
    gbd_buurt_volgnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_buurt_volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_buurt_volgnummer_lt = 56 # int | Less than; number (optional)
    gbd_buurt_volgnummer_lte = 56 # int | Less than or equal to; number (optional)
    gbd_buurt_volgnummer_not = [56] # List[int] | Exclude matches; number (optional)
    gbd_ggw_identificatie = 'gbd_ggw_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_ggw_identificatie_in = ['gbd_ggw_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_ggw_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_ggw_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_ggw_identificatie_like = 'gbd_ggw_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_ggw_identificatie_not = ['gbd_ggw_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_ggw_naam = 'gbd_ggw_naam_example' # str | De naam van het object. (optional)
    gbd_ggw_naam_in = ['gbd_ggw_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_ggw_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_ggw_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_ggw_naam_like = 'gbd_ggw_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_ggw_naam_not = ['gbd_ggw_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_ggw_volgnummer = 'gbd_ggw_volgnummer_example' # str | Uniek volgnummer van de toestand van het object. (optional)
    gbd_ggw_volgnummer_in = ['gbd_ggw_volgnummer_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_ggw_volgnummer_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_ggw_volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_ggw_volgnummer_like = 'gbd_ggw_volgnummer_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_ggw_volgnummer_not = ['gbd_ggw_volgnummer_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_stadsdeel_identificatie = 'gbd_stadsdeel_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_stadsdeel_identificatie_in = ['gbd_stadsdeel_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_stadsdeel_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_stadsdeel_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_stadsdeel_identificatie_like = 'gbd_stadsdeel_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_stadsdeel_identificatie_not = ['gbd_stadsdeel_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_stadsdeel_naam = 'gbd_stadsdeel_naam_example' # str | De naam van het object. (optional)
    gbd_stadsdeel_naam_in = ['gbd_stadsdeel_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_stadsdeel_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_stadsdeel_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_stadsdeel_naam_like = 'gbd_stadsdeel_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_stadsdeel_naam_not = ['gbd_stadsdeel_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_stadsdeel_volgnummer = 56 # int | Uniek volgnummer van de toestand van het object. (optional)
    gbd_stadsdeel_volgnummer_gt = 56 # int | Greater than; number (optional)
    gbd_stadsdeel_volgnummer_gte = 56 # int | Greater than or equal to; number (optional)
    gbd_stadsdeel_volgnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_stadsdeel_volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_stadsdeel_volgnummer_lt = 56 # int | Less than; number (optional)
    gbd_stadsdeel_volgnummer_lte = 56 # int | Less than or equal to; number (optional)
    gbd_stadsdeel_volgnummer_not = [56] # List[int] | Exclude matches; number (optional)
    gbd_wijk_identificatie = 'gbd_wijk_identificatie_example' # str | Unieke identificatie van het object (optional)
    gbd_wijk_identificatie_in = ['gbd_wijk_identificatie_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_wijk_identificatie_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_wijk_identificatie_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_wijk_identificatie_like = 'gbd_wijk_identificatie_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_wijk_identificatie_not = ['gbd_wijk_identificatie_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_wijk_naam = 'gbd_wijk_naam_example' # str | De naam van het object. (optional)
    gbd_wijk_naam_in = ['gbd_wijk_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_wijk_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    gbd_wijk_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_wijk_naam_like = 'gbd_wijk_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    gbd_wijk_naam_not = ['gbd_wijk_naam_not_example'] # List[str] | Exclude matches; text (optional)
    gbd_wijk_volgnummer = 56 # int | Uniek volgnummer van de toestand van het object. (optional)
    gbd_wijk_volgnummer_gt = 56 # int | Greater than; number (optional)
    gbd_wijk_volgnummer_gte = 56 # int | Greater than or equal to; number (optional)
    gbd_wijk_volgnummer_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    gbd_wijk_volgnummer_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    gbd_wijk_volgnummer_lt = 56 # int | Less than; number (optional)
    gbd_wijk_volgnummer_lte = 56 # int | Less than or equal to; number (optional)
    gbd_wijk_volgnummer_not = [56] # List[int] | Exclude matches; number (optional)
    id2 = 56 # int | Identificerend kenmerk van het ticket. (optional)
    id_gt = 56 # int | Greater than; number (optional)
    id_gte = 56 # int | Greater than or equal to; number (optional)
    id_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    id_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    id_lt = 56 # int | Less than; number (optional)
    id_lte = 56 # int | Less than or equal to; number (optional)
    id_not = [56] # List[int] | Exclude matches; number (optional)
    items_definitief = 'items_definitief_example' # str | De onderdelen en de werkzaamheden zoals deze op de factuur vermeld worden. (optional)
    items_definitief_in = ['items_definitief_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    items_definitief_isempty = True # bool | Whether the field is empty or not. (optional)
    items_definitief_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    items_definitief_like = 'items_definitief_like_example' # str | Matches text using wildcards (? and *). (optional)
    items_definitief_not = ['items_definitief_not_example'] # List[str] | Exclude matches; text (optional)
    items_offerte = 'items_offerte_example' # str | De onderdelen en de werkzaamheden zoals deze op de offerte vermeld worden. (optional)
    items_offerte_in = ['items_offerte_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    items_offerte_isempty = True # bool | Whether the field is empty or not. (optional)
    items_offerte_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    items_offerte_like = 'items_offerte_like_example' # str | Matches text using wildcards (? and *). (optional)
    items_offerte_not = ['items_offerte_not_example'] # List[str] | Exclude matches; text (optional)
    onderhoudsbedrijf = 'onderhoudsbedrijf_example' # str | De naam van het onderhoudsbedrijf. (optional)
    onderhoudsbedrijf_in = ['onderhoudsbedrijf_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    onderhoudsbedrijf_isempty = True # bool | Whether the field is empty or not. (optional)
    onderhoudsbedrijf_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    onderhoudsbedrijf_like = 'onderhoudsbedrijf_like_example' # str | Matches text using wildcards (? and *). (optional)
    onderhoudsbedrijf_not = ['onderhoudsbedrijf_not_example'] # List[str] | Exclude matches; text (optional)
    oorzaak = ['oorzaak_example'] # List[str] | Exact; val1,val2 (optional)
    oorzaak_contains = ['oorzaak_contains_example'] # List[str] | Matches values from a comma-separated list: val1,val2,valN. (optional)
    oplossing = ['oplossing_example'] # List[str] | Exact; val1,val2 (optional)
    oplossing_contains = ['oplossing_contains_example'] # List[str] | Matches values from a comma-separated list: val1,val2,valN. (optional)
    prijs = 3.4 # float | De totale prijs van de gebruikte onderdelen en de uitgevoerde werkzaamheden. (optional)
    prijs_offerte = 3.4 # float | De totale prijs op de offerte voor de te gebruiken onderdelen en de uit te voeren werkzaamheden. (optional)
    prijs_offerte_gt = 3.4 # float | Greater than; number (optional)
    prijs_offerte_gte = 3.4 # float | Greater than or equal to; number (optional)
    prijs_offerte_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prijs_offerte_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prijs_offerte_lt = 3.4 # float | Less than; number (optional)
    prijs_offerte_lte = 3.4 # float | Less than or equal to; number (optional)
    prijs_offerte_not = [3.4] # List[float] | Exclude matches; number (optional)
    prijs_gt = 3.4 # float | Greater than; number (optional)
    prijs_gte = 3.4 # float | Greater than or equal to; number (optional)
    prijs_in = [3.4] # List[float] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prijs_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prijs_lt = 3.4 # float | Less than; number (optional)
    prijs_lte = 3.4 # float | Less than or equal to; number (optional)
    prijs_not = [3.4] # List[float] | Exclude matches; number (optional)
    prioriteit_naam = 'prioriteit_naam_example' # str | De naam die de soort prioriteit weergeeft. (optional)
    prioriteit_naam_in = ['prioriteit_naam_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prioriteit_naam_isempty = True # bool | Whether the field is empty or not. (optional)
    prioriteit_naam_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prioriteit_naam_like = 'prioriteit_naam_like_example' # str | Matches text using wildcards (? and *). (optional)
    prioriteit_naam_not = ['prioriteit_naam_not_example'] # List[str] | Exclude matches; text (optional)
    prioriteit_opmerking = 'prioriteit_opmerking_example' # str | Een opmerking die toegevoegd wordt om de prioritering te verduidelijken. (optional)
    prioriteit_opmerking_in = ['prioriteit_opmerking_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prioriteit_opmerking_isempty = True # bool | Whether the field is empty or not. (optional)
    prioriteit_opmerking_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prioriteit_opmerking_like = 'prioriteit_opmerking_like_example' # str | Matches text using wildcards (? and *). (optional)
    prioriteit_opmerking_not = ['prioriteit_opmerking_not_example'] # List[str] | Exclude matches; text (optional)
    prioriteit_responstijd = 56 # int | De toegestane responsetijd voor deze prioriteit.  (optional)
    prioriteit_responstijd_gt = 56 # int | Greater than; number (optional)
    prioriteit_responstijd_gte = 56 # int | Greater than or equal to; number (optional)
    prioriteit_responstijd_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    prioriteit_responstijd_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    prioriteit_responstijd_lt = 56 # int | Less than; number (optional)
    prioriteit_responstijd_lte = 56 # int | Less than or equal to; number (optional)
    prioriteit_responstijd_not = [56] # List[int] | Exclude matches; number (optional)
    probleem = ['probleem_example'] # List[str] | Exact; val1,val2 (optional)
    probleem_module_naam = ['probleem_module_naam_example'] # List[str] | Exact; val1,val2 (optional)
    probleem_module_naam_contains = ['probleem_module_naam_contains_example'] # List[str] | Matches values from a comma-separated list: val1,val2,valN. (optional)
    probleem_contains = ['probleem_contains_example'] # List[str] | Matches values from a comma-separated list: val1,val2,valN. (optional)
    rangorde_nummer_tickettype = 56 # int | Het rangordenummer van het type ticket. (optional)
    rangorde_nummer_tickettype_gt = 56 # int | Greater than; number (optional)
    rangorde_nummer_tickettype_gte = 56 # int | Greater than or equal to; number (optional)
    rangorde_nummer_tickettype_in = [56] # List[int] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    rangorde_nummer_tickettype_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    rangorde_nummer_tickettype_lt = 56 # int | Less than; number (optional)
    rangorde_nummer_tickettype_lte = 56 # int | Less than or equal to; number (optional)
    rangorde_nummer_tickettype_not = [56] # List[int] | Exclude matches; number (optional)
    reden_afgewezen = 'reden_afgewezen_example' # str | De reden waarom het ticket de status 'afgewezen' heeft gekregen. (optional)
    reden_afgewezen_in = ['reden_afgewezen_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    reden_afgewezen_isempty = True # bool | Whether the field is empty or not. (optional)
    reden_afgewezen_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    reden_afgewezen_like = 'reden_afgewezen_like_example' # str | Matches text using wildcards (? and *). (optional)
    reden_afgewezen_not = ['reden_afgewezen_not_example'] # List[str] | Exclude matches; text (optional)
    referentienummer_leverancier = 'referentienummer_leverancier_example' # str | Het referentienummer dat door de leverancier aan het ticket gegeven wordt. (optional)
    referentienummer_leverancier_in = ['referentienummer_leverancier_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    referentienummer_leverancier_isempty = True # bool | Whether the field is empty or not. (optional)
    referentienummer_leverancier_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    referentienummer_leverancier_like = 'referentienummer_leverancier_like_example' # str | Matches text using wildcards (? and *). (optional)
    referentienummer_leverancier_not = ['referentienummer_leverancier_not_example'] # List[str] | Exclude matches; text (optional)
    ticketstatus = 'ticketstatus_example' # str | De status van het ticket. (optional)
    ticketstatus_in = ['ticketstatus_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    ticketstatus_isempty = True # bool | Whether the field is empty or not. (optional)
    ticketstatus_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    ticketstatus_like = 'ticketstatus_like_example' # str | Matches text using wildcards (? and *). (optional)
    ticketstatus_not = ['ticketstatus_not_example'] # List[str] | Exclude matches; text (optional)
    tickettype = 'tickettype_example' # str | De naam van het type ticket. (optional)
    tickettype_in = ['tickettype_in_example'] # List[str] | Matches any value from a comma-separated list: val1,val2,valN. (optional)
    tickettype_isempty = True # bool | Whether the field is empty or not. (optional)
    tickettype_isnull = True # bool | Whether the field has a NULL value or not. (optional)
    tickettype_like = 'tickettype_like_example' # str | Matches text using wildcards (? and *). (optional)
    tickettype_not = ['tickettype_not_example'] # List[str] | Exclude matches; text (optional)

    try:
        api_response = await api_instance.huishoudelijkafval_ticket_retrieve2(id, accept_crs=accept_crs, content_crs=content_crs, x_api_key=x_api_key, expand=expand, expand_scope=expand_scope, fields=fields, format=format, sort=sort, container_id=container_id, container_id_in=container_id_in, container_id_isempty=container_id_isempty, container_id_isnull=container_id_isnull, container_id_like=container_id_like, container_id_not=container_id_not, containerlocatie_id=containerlocatie_id, containerlocatie_id_in=containerlocatie_id_in, containerlocatie_id_isempty=containerlocatie_id_isempty, containerlocatie_id_isnull=containerlocatie_id_isnull, containerlocatie_id_like=containerlocatie_id_like, containerlocatie_id_not=containerlocatie_id_not, datum_afgerond=datum_afgerond, datum_afgerond_gt=datum_afgerond_gt, datum_afgerond_gte=datum_afgerond_gte, datum_afgerond_in=datum_afgerond_in, datum_afgerond_isnull=datum_afgerond_isnull, datum_afgerond_lt=datum_afgerond_lt, datum_afgerond_lte=datum_afgerond_lte, datum_afgerond_not=datum_afgerond_not, datum_afgewezen=datum_afgewezen, datum_afgewezen_gt=datum_afgewezen_gt, datum_afgewezen_gte=datum_afgewezen_gte, datum_afgewezen_in=datum_afgewezen_in, datum_afgewezen_isnull=datum_afgewezen_isnull, datum_afgewezen_lt=datum_afgewezen_lt, datum_afgewezen_lte=datum_afgewezen_lte, datum_afgewezen_not=datum_afgewezen_not, datum_creatie=datum_creatie, datum_creatie_gt=datum_creatie_gt, datum_creatie_gte=datum_creatie_gte, datum_creatie_in=datum_creatie_in, datum_creatie_isnull=datum_creatie_isnull, datum_creatie_lt=datum_creatie_lt, datum_creatie_lte=datum_creatie_lte, datum_creatie_not=datum_creatie_not, datum_factuur=datum_factuur, datum_factuur_gt=datum_factuur_gt, datum_factuur_gte=datum_factuur_gte, datum_factuur_in=datum_factuur_in, datum_factuur_isnull=datum_factuur_isnull, datum_factuur_lt=datum_factuur_lt, datum_factuur_lte=datum_factuur_lte, datum_factuur_not=datum_factuur_not, datum_financiele_goedkeuring=datum_financiele_goedkeuring, datum_financiele_goedkeuring_gt=datum_financiele_goedkeuring_gt, datum_financiele_goedkeuring_gte=datum_financiele_goedkeuring_gte, datum_financiele_goedkeuring_in=datum_financiele_goedkeuring_in, datum_financiele_goedkeuring_isnull=datum_financiele_goedkeuring_isnull, datum_financiele_goedkeuring_lt=datum_financiele_goedkeuring_lt, datum_financiele_goedkeuring_lte=datum_financiele_goedkeuring_lte, datum_financiele_goedkeuring_not=datum_financiele_goedkeuring_not, datum_geaccepteerd=datum_geaccepteerd, datum_geaccepteerd_gt=datum_geaccepteerd_gt, datum_geaccepteerd_gte=datum_geaccepteerd_gte, datum_geaccepteerd_in=datum_geaccepteerd_in, datum_geaccepteerd_isnull=datum_geaccepteerd_isnull, datum_geaccepteerd_lt=datum_geaccepteerd_lt, datum_geaccepteerd_lte=datum_geaccepteerd_lte, datum_geaccepteerd_not=datum_geaccepteerd_not, datum_gefactureerd=datum_gefactureerd, datum_gefactureerd_gt=datum_gefactureerd_gt, datum_gefactureerd_gte=datum_gefactureerd_gte, datum_gefactureerd_in=datum_gefactureerd_in, datum_gefactureerd_isnull=datum_gefactureerd_isnull, datum_gefactureerd_lt=datum_gefactureerd_lt, datum_gefactureerd_lte=datum_gefactureerd_lte, datum_gefactureerd_not=datum_gefactureerd_not, datum_gepland=datum_gepland, datum_gepland_gt=datum_gepland_gt, datum_gepland_gte=datum_gepland_gte, datum_gepland_in=datum_gepland_in, datum_gepland_isnull=datum_gepland_isnull, datum_gepland_lt=datum_gepland_lt, datum_gepland_lte=datum_gepland_lte, datum_gepland_not=datum_gepland_not, datum_gereed=datum_gereed, datum_gereed_gt=datum_gereed_gt, datum_gereed_gte=datum_gereed_gte, datum_gereed_in=datum_gereed_in, datum_gereed_isnull=datum_gereed_isnull, datum_gereed_lt=datum_gereed_lt, datum_gereed_lte=datum_gereed_lte, datum_gereed_not=datum_gereed_not, datum_offerte=datum_offerte, datum_offerte_gt=datum_offerte_gt, datum_offerte_gte=datum_offerte_gte, datum_offerte_in=datum_offerte_in, datum_offerte_isnull=datum_offerte_isnull, datum_offerte_lt=datum_offerte_lt, datum_offerte_lte=datum_offerte_lte, datum_offerte_not=datum_offerte_not, datum_technische_goedkeuring=datum_technische_goedkeuring, datum_technische_goedkeuring_gt=datum_technische_goedkeuring_gt, datum_technische_goedkeuring_gte=datum_technische_goedkeuring_gte, datum_technische_goedkeuring_in=datum_technische_goedkeuring_in, datum_technische_goedkeuring_isnull=datum_technische_goedkeuring_isnull, datum_technische_goedkeuring_lt=datum_technische_goedkeuring_lt, datum_technische_goedkeuring_lte=datum_technische_goedkeuring_lte, datum_technische_goedkeuring_not=datum_technische_goedkeuring_not, datum_wijziging=datum_wijziging, datum_wijziging_gt=datum_wijziging_gt, datum_wijziging_gte=datum_wijziging_gte, datum_wijziging_in=datum_wijziging_in, datum_wijziging_isnull=datum_wijziging_isnull, datum_wijziging_lt=datum_wijziging_lt, datum_wijziging_lte=datum_wijziging_lte, datum_wijziging_not=datum_wijziging_not, datum_workflow_start=datum_workflow_start, datum_workflow_start_gt=datum_workflow_start_gt, datum_workflow_start_gte=datum_workflow_start_gte, datum_workflow_start_in=datum_workflow_start_in, datum_workflow_start_isnull=datum_workflow_start_isnull, datum_workflow_start_lt=datum_workflow_start_lt, datum_workflow_start_lte=datum_workflow_start_lte, datum_workflow_start_not=datum_workflow_start_not, doorlooptijd=doorlooptijd, doorlooptijd_in=doorlooptijd_in, doorlooptijd_isempty=doorlooptijd_isempty, doorlooptijd_isnull=doorlooptijd_isnull, doorlooptijd_like=doorlooptijd_like, doorlooptijd_not=doorlooptijd_not, eigenaar=eigenaar, eigenaar_in=eigenaar_in, eigenaar_isempty=eigenaar_isempty, eigenaar_isnull=eigenaar_isnull, eigenaar_like=eigenaar_like, eigenaar_not=eigenaar_not, factuur_nummer=factuur_nummer, factuur_nummer_in=factuur_nummer_in, factuur_nummer_isempty=factuur_nummer_isempty, factuur_nummer_isnull=factuur_nummer_isnull, factuur_nummer_like=factuur_nummer_like, factuur_nummer_not=factuur_nummer_not, gbd_buurt_identificatie=gbd_buurt_identificatie, gbd_buurt_identificatie_in=gbd_buurt_identificatie_in, gbd_buurt_identificatie_isempty=gbd_buurt_identificatie_isempty, gbd_buurt_identificatie_isnull=gbd_buurt_identificatie_isnull, gbd_buurt_identificatie_like=gbd_buurt_identificatie_like, gbd_buurt_identificatie_not=gbd_buurt_identificatie_not, gbd_buurt_code=gbd_buurt_code, gbd_buurt_code_in=gbd_buurt_code_in, gbd_buurt_code_isempty=gbd_buurt_code_isempty, gbd_buurt_code_isnull=gbd_buurt_code_isnull, gbd_buurt_code_like=gbd_buurt_code_like, gbd_buurt_code_not=gbd_buurt_code_not, gbd_buurt_naam=gbd_buurt_naam, gbd_buurt_naam_in=gbd_buurt_naam_in, gbd_buurt_naam_isempty=gbd_buurt_naam_isempty, gbd_buurt_naam_isnull=gbd_buurt_naam_isnull, gbd_buurt_naam_like=gbd_buurt_naam_like, gbd_buurt_naam_not=gbd_buurt_naam_not, gbd_buurt_volgnummer=gbd_buurt_volgnummer, gbd_buurt_volgnummer_gt=gbd_buurt_volgnummer_gt, gbd_buurt_volgnummer_gte=gbd_buurt_volgnummer_gte, gbd_buurt_volgnummer_in=gbd_buurt_volgnummer_in, gbd_buurt_volgnummer_isnull=gbd_buurt_volgnummer_isnull, gbd_buurt_volgnummer_lt=gbd_buurt_volgnummer_lt, gbd_buurt_volgnummer_lte=gbd_buurt_volgnummer_lte, gbd_buurt_volgnummer_not=gbd_buurt_volgnummer_not, gbd_ggw_identificatie=gbd_ggw_identificatie, gbd_ggw_identificatie_in=gbd_ggw_identificatie_in, gbd_ggw_identificatie_isempty=gbd_ggw_identificatie_isempty, gbd_ggw_identificatie_isnull=gbd_ggw_identificatie_isnull, gbd_ggw_identificatie_like=gbd_ggw_identificatie_like, gbd_ggw_identificatie_not=gbd_ggw_identificatie_not, gbd_ggw_naam=gbd_ggw_naam, gbd_ggw_naam_in=gbd_ggw_naam_in, gbd_ggw_naam_isempty=gbd_ggw_naam_isempty, gbd_ggw_naam_isnull=gbd_ggw_naam_isnull, gbd_ggw_naam_like=gbd_ggw_naam_like, gbd_ggw_naam_not=gbd_ggw_naam_not, gbd_ggw_volgnummer=gbd_ggw_volgnummer, gbd_ggw_volgnummer_in=gbd_ggw_volgnummer_in, gbd_ggw_volgnummer_isempty=gbd_ggw_volgnummer_isempty, gbd_ggw_volgnummer_isnull=gbd_ggw_volgnummer_isnull, gbd_ggw_volgnummer_like=gbd_ggw_volgnummer_like, gbd_ggw_volgnummer_not=gbd_ggw_volgnummer_not, gbd_stadsdeel_identificatie=gbd_stadsdeel_identificatie, gbd_stadsdeel_identificatie_in=gbd_stadsdeel_identificatie_in, gbd_stadsdeel_identificatie_isempty=gbd_stadsdeel_identificatie_isempty, gbd_stadsdeel_identificatie_isnull=gbd_stadsdeel_identificatie_isnull, gbd_stadsdeel_identificatie_like=gbd_stadsdeel_identificatie_like, gbd_stadsdeel_identificatie_not=gbd_stadsdeel_identificatie_not, gbd_stadsdeel_naam=gbd_stadsdeel_naam, gbd_stadsdeel_naam_in=gbd_stadsdeel_naam_in, gbd_stadsdeel_naam_isempty=gbd_stadsdeel_naam_isempty, gbd_stadsdeel_naam_isnull=gbd_stadsdeel_naam_isnull, gbd_stadsdeel_naam_like=gbd_stadsdeel_naam_like, gbd_stadsdeel_naam_not=gbd_stadsdeel_naam_not, gbd_stadsdeel_volgnummer=gbd_stadsdeel_volgnummer, gbd_stadsdeel_volgnummer_gt=gbd_stadsdeel_volgnummer_gt, gbd_stadsdeel_volgnummer_gte=gbd_stadsdeel_volgnummer_gte, gbd_stadsdeel_volgnummer_in=gbd_stadsdeel_volgnummer_in, gbd_stadsdeel_volgnummer_isnull=gbd_stadsdeel_volgnummer_isnull, gbd_stadsdeel_volgnummer_lt=gbd_stadsdeel_volgnummer_lt, gbd_stadsdeel_volgnummer_lte=gbd_stadsdeel_volgnummer_lte, gbd_stadsdeel_volgnummer_not=gbd_stadsdeel_volgnummer_not, gbd_wijk_identificatie=gbd_wijk_identificatie, gbd_wijk_identificatie_in=gbd_wijk_identificatie_in, gbd_wijk_identificatie_isempty=gbd_wijk_identificatie_isempty, gbd_wijk_identificatie_isnull=gbd_wijk_identificatie_isnull, gbd_wijk_identificatie_like=gbd_wijk_identificatie_like, gbd_wijk_identificatie_not=gbd_wijk_identificatie_not, gbd_wijk_naam=gbd_wijk_naam, gbd_wijk_naam_in=gbd_wijk_naam_in, gbd_wijk_naam_isempty=gbd_wijk_naam_isempty, gbd_wijk_naam_isnull=gbd_wijk_naam_isnull, gbd_wijk_naam_like=gbd_wijk_naam_like, gbd_wijk_naam_not=gbd_wijk_naam_not, gbd_wijk_volgnummer=gbd_wijk_volgnummer, gbd_wijk_volgnummer_gt=gbd_wijk_volgnummer_gt, gbd_wijk_volgnummer_gte=gbd_wijk_volgnummer_gte, gbd_wijk_volgnummer_in=gbd_wijk_volgnummer_in, gbd_wijk_volgnummer_isnull=gbd_wijk_volgnummer_isnull, gbd_wijk_volgnummer_lt=gbd_wijk_volgnummer_lt, gbd_wijk_volgnummer_lte=gbd_wijk_volgnummer_lte, gbd_wijk_volgnummer_not=gbd_wijk_volgnummer_not, id2=id2, id_gt=id_gt, id_gte=id_gte, id_in=id_in, id_isnull=id_isnull, id_lt=id_lt, id_lte=id_lte, id_not=id_not, items_definitief=items_definitief, items_definitief_in=items_definitief_in, items_definitief_isempty=items_definitief_isempty, items_definitief_isnull=items_definitief_isnull, items_definitief_like=items_definitief_like, items_definitief_not=items_definitief_not, items_offerte=items_offerte, items_offerte_in=items_offerte_in, items_offerte_isempty=items_offerte_isempty, items_offerte_isnull=items_offerte_isnull, items_offerte_like=items_offerte_like, items_offerte_not=items_offerte_not, onderhoudsbedrijf=onderhoudsbedrijf, onderhoudsbedrijf_in=onderhoudsbedrijf_in, onderhoudsbedrijf_isempty=onderhoudsbedrijf_isempty, onderhoudsbedrijf_isnull=onderhoudsbedrijf_isnull, onderhoudsbedrijf_like=onderhoudsbedrijf_like, onderhoudsbedrijf_not=onderhoudsbedrijf_not, oorzaak=oorzaak, oorzaak_contains=oorzaak_contains, oplossing=oplossing, oplossing_contains=oplossing_contains, prijs=prijs, prijs_offerte=prijs_offerte, prijs_offerte_gt=prijs_offerte_gt, prijs_offerte_gte=prijs_offerte_gte, prijs_offerte_in=prijs_offerte_in, prijs_offerte_isnull=prijs_offerte_isnull, prijs_offerte_lt=prijs_offerte_lt, prijs_offerte_lte=prijs_offerte_lte, prijs_offerte_not=prijs_offerte_not, prijs_gt=prijs_gt, prijs_gte=prijs_gte, prijs_in=prijs_in, prijs_isnull=prijs_isnull, prijs_lt=prijs_lt, prijs_lte=prijs_lte, prijs_not=prijs_not, prioriteit_naam=prioriteit_naam, prioriteit_naam_in=prioriteit_naam_in, prioriteit_naam_isempty=prioriteit_naam_isempty, prioriteit_naam_isnull=prioriteit_naam_isnull, prioriteit_naam_like=prioriteit_naam_like, prioriteit_naam_not=prioriteit_naam_not, prioriteit_opmerking=prioriteit_opmerking, prioriteit_opmerking_in=prioriteit_opmerking_in, prioriteit_opmerking_isempty=prioriteit_opmerking_isempty, prioriteit_opmerking_isnull=prioriteit_opmerking_isnull, prioriteit_opmerking_like=prioriteit_opmerking_like, prioriteit_opmerking_not=prioriteit_opmerking_not, prioriteit_responstijd=prioriteit_responstijd, prioriteit_responstijd_gt=prioriteit_responstijd_gt, prioriteit_responstijd_gte=prioriteit_responstijd_gte, prioriteit_responstijd_in=prioriteit_responstijd_in, prioriteit_responstijd_isnull=prioriteit_responstijd_isnull, prioriteit_responstijd_lt=prioriteit_responstijd_lt, prioriteit_responstijd_lte=prioriteit_responstijd_lte, prioriteit_responstijd_not=prioriteit_responstijd_not, probleem=probleem, probleem_module_naam=probleem_module_naam, probleem_module_naam_contains=probleem_module_naam_contains, probleem_contains=probleem_contains, rangorde_nummer_tickettype=rangorde_nummer_tickettype, rangorde_nummer_tickettype_gt=rangorde_nummer_tickettype_gt, rangorde_nummer_tickettype_gte=rangorde_nummer_tickettype_gte, rangorde_nummer_tickettype_in=rangorde_nummer_tickettype_in, rangorde_nummer_tickettype_isnull=rangorde_nummer_tickettype_isnull, rangorde_nummer_tickettype_lt=rangorde_nummer_tickettype_lt, rangorde_nummer_tickettype_lte=rangorde_nummer_tickettype_lte, rangorde_nummer_tickettype_not=rangorde_nummer_tickettype_not, reden_afgewezen=reden_afgewezen, reden_afgewezen_in=reden_afgewezen_in, reden_afgewezen_isempty=reden_afgewezen_isempty, reden_afgewezen_isnull=reden_afgewezen_isnull, reden_afgewezen_like=reden_afgewezen_like, reden_afgewezen_not=reden_afgewezen_not, referentienummer_leverancier=referentienummer_leverancier, referentienummer_leverancier_in=referentienummer_leverancier_in, referentienummer_leverancier_isempty=referentienummer_leverancier_isempty, referentienummer_leverancier_isnull=referentienummer_leverancier_isnull, referentienummer_leverancier_like=referentienummer_leverancier_like, referentienummer_leverancier_not=referentienummer_leverancier_not, ticketstatus=ticketstatus, ticketstatus_in=ticketstatus_in, ticketstatus_isempty=ticketstatus_isempty, ticketstatus_isnull=ticketstatus_isnull, ticketstatus_like=ticketstatus_like, ticketstatus_not=ticketstatus_not, tickettype=tickettype, tickettype_in=tickettype_in, tickettype_isempty=tickettype_isempty, tickettype_isnull=tickettype_isnull, tickettype_like=tickettype_like, tickettype_not=tickettype_not)
        print("The response of TicketApi->huishoudelijkafval_ticket_retrieve2:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TicketApi->huishoudelijkafval_ticket_retrieve2: %s\n" % e)
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
 **container_id** | **str**| Unieke aanduiding objecttype | [optional] 
 **container_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **container_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **container_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **container_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **container_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **containerlocatie_id** | **str**| Identificerend kenmerk van de put waarin de container is geplaatst | [optional] 
 **containerlocatie_id_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **containerlocatie_id_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **containerlocatie_id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **containerlocatie_id_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **containerlocatie_id_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **datum_afgerond** | **datetime**| De datum waarop de werkzaamheden als gereed aangegeven zijn door het onderhoudsbedrijf. | [optional] 
 **datum_afgerond_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgerond_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgerond_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_afgerond_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_afgerond_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgerond_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgerond_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen** | **datetime**| De datum waarop het ticket de status &#39;afgewezen&#39; krijgt. | [optional] 
 **datum_afgewezen_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_afgewezen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_afgewezen_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_afgewezen_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie** | **datetime**| De datum waarop het ticket aangemaakt is. | [optional] 
 **datum_creatie_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_creatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_creatie_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_creatie_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur** | **datetime**| De datum waarop het ticket gefactureerd is. | [optional] 
 **datum_factuur_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_factuur_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_factuur_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_factuur_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring** | **datetime**| De datum waarop de financiale aspecten van de werkzaamheden goed- of afgekeurd zijn. | [optional] 
 **datum_financiele_goedkeuring_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_financiele_goedkeuring_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_financiele_goedkeuring_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_financiele_goedkeuring_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd** | **datetime**| De datum waarop het ticket geaccepteerd is door het onderhoudsbedrijf. | [optional] 
 **datum_geaccepteerd_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_geaccepteerd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_geaccepteerd_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_geaccepteerd_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd** | **datetime**| De datum waarop de factuur in het systeem de status &#39;gefactureerd&#39; krijgt. | [optional] 
 **datum_gefactureerd_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_gefactureerd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_gefactureerd_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gefactureerd_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland** | **datetime**| De datum waarop de uitvoering van de werkzaamheden is ingepland. | [optional] 
 **datum_gepland_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_gepland_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_gepland_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gepland_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed** | **datetime**| De datum waarop de werkzaamheden uitgevoerd zijn. | [optional] 
 **datum_gereed_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_gereed_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_gereed_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_gereed_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte** | **datetime**| De datum waarop de offerte is aangemaakt . | [optional] 
 **datum_offerte_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_offerte_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_offerte_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_offerte_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring** | **datetime**| De datum waarop de technische aspecten van de werkzaamheden goed- of afgekeurd zijn. | [optional] 
 **datum_technische_goedkeuring_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_technische_goedkeuring_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_technische_goedkeuring_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_technische_goedkeuring_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging** | **datetime**| De datum waarop het ticket is gewijzigd. | [optional] 
 **datum_wijziging_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_wijziging_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_wijziging_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_wijziging_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start** | **datetime**| De datum waarop de workflow start. | [optional] 
 **datum_workflow_start_gt** | **datetime**| Greater than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start_gte** | **datetime**| Greater than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start_in** | [**List[datetime]**](datetime.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **datum_workflow_start_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **datum_workflow_start_lt** | **datetime**| Less than; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start_lte** | **datetime**| Less than or equal to; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **datum_workflow_start_not** | [**List[datetime]**](datetime.md)| Exclude matches; use yyyy-mm-dd or yyyy-mm-ddThh:mm[:ss[.ms]] | [optional] 
 **doorlooptijd** | **str**| De tijdsspanne in werkdagen tussen de &#39;datumCreatie&#39;en de &#39;datumAfgerond&#39; of de tijdsspanne in werkdagen tussen de &#39;datumCreatie&#39; en de laatste statuswijziging in het geval het ticket nog niet afgerond is. | [optional] 
 **doorlooptijd_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **doorlooptijd_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **doorlooptijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **doorlooptijd_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **doorlooptijd_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **eigenaar** | **str**| De naam van de eigenaar van de container. | [optional] 
 **eigenaar_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **eigenaar_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **eigenaar_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **eigenaar_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **eigenaar_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **factuur_nummer** | **str**| Het nummer van de factuur. | [optional] 
 **factuur_nummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **factuur_nummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **factuur_nummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **factuur_nummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **factuur_nummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_buurt_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_code** | **str**| Unieke code. | [optional] 
 **gbd_buurt_code_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_code_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_code_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_code_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_code_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_naam** | **str**| De naam van het object. | [optional] 
 **gbd_buurt_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_buurt_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_buurt_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_buurt_volgnummer** | **int**| Uniek volgnummer van de toestand van het object. | [optional] 
 **gbd_buurt_volgnummer_gt** | **int**| Greater than; number | [optional] 
 **gbd_buurt_volgnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **gbd_buurt_volgnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_buurt_volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_buurt_volgnummer_lt** | **int**| Less than; number | [optional] 
 **gbd_buurt_volgnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **gbd_buurt_volgnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **gbd_ggw_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_ggw_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_ggw_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_ggw_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_ggw_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_ggw_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_ggw_naam** | **str**| De naam van het object. | [optional] 
 **gbd_ggw_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_ggw_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_ggw_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_ggw_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_ggw_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_ggw_volgnummer** | **str**| Uniek volgnummer van de toestand van het object. | [optional] 
 **gbd_ggw_volgnummer_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_ggw_volgnummer_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_ggw_volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_ggw_volgnummer_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_ggw_volgnummer_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_stadsdeel_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_stadsdeel_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_stadsdeel_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_stadsdeel_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_stadsdeel_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_stadsdeel_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_stadsdeel_naam** | **str**| De naam van het object. | [optional] 
 **gbd_stadsdeel_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_stadsdeel_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_stadsdeel_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_stadsdeel_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_stadsdeel_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_stadsdeel_volgnummer** | **int**| Uniek volgnummer van de toestand van het object. | [optional] 
 **gbd_stadsdeel_volgnummer_gt** | **int**| Greater than; number | [optional] 
 **gbd_stadsdeel_volgnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **gbd_stadsdeel_volgnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_stadsdeel_volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_stadsdeel_volgnummer_lt** | **int**| Less than; number | [optional] 
 **gbd_stadsdeel_volgnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **gbd_stadsdeel_volgnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **gbd_wijk_identificatie** | **str**| Unieke identificatie van het object | [optional] 
 **gbd_wijk_identificatie_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_wijk_identificatie_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_wijk_identificatie_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_wijk_identificatie_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_wijk_identificatie_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_wijk_naam** | **str**| De naam van het object. | [optional] 
 **gbd_wijk_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_wijk_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **gbd_wijk_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_wijk_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **gbd_wijk_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **gbd_wijk_volgnummer** | **int**| Uniek volgnummer van de toestand van het object. | [optional] 
 **gbd_wijk_volgnummer_gt** | **int**| Greater than; number | [optional] 
 **gbd_wijk_volgnummer_gte** | **int**| Greater than or equal to; number | [optional] 
 **gbd_wijk_volgnummer_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **gbd_wijk_volgnummer_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **gbd_wijk_volgnummer_lt** | **int**| Less than; number | [optional] 
 **gbd_wijk_volgnummer_lte** | **int**| Less than or equal to; number | [optional] 
 **gbd_wijk_volgnummer_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **id2** | **int**| Identificerend kenmerk van het ticket. | [optional] 
 **id_gt** | **int**| Greater than; number | [optional] 
 **id_gte** | **int**| Greater than or equal to; number | [optional] 
 **id_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **id_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **id_lt** | **int**| Less than; number | [optional] 
 **id_lte** | **int**| Less than or equal to; number | [optional] 
 **id_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **items_definitief** | **str**| De onderdelen en de werkzaamheden zoals deze op de factuur vermeld worden. | [optional] 
 **items_definitief_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **items_definitief_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **items_definitief_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **items_definitief_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **items_definitief_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **items_offerte** | **str**| De onderdelen en de werkzaamheden zoals deze op de offerte vermeld worden. | [optional] 
 **items_offerte_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **items_offerte_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **items_offerte_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **items_offerte_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **items_offerte_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **onderhoudsbedrijf** | **str**| De naam van het onderhoudsbedrijf. | [optional] 
 **onderhoudsbedrijf_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **onderhoudsbedrijf_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **onderhoudsbedrijf_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **onderhoudsbedrijf_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **onderhoudsbedrijf_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **oorzaak** | [**List[str]**](str.md)| Exact; val1,val2 | [optional] 
 **oorzaak_contains** | [**List[str]**](str.md)| Matches values from a comma-separated list: val1,val2,valN. | [optional] 
 **oplossing** | [**List[str]**](str.md)| Exact; val1,val2 | [optional] 
 **oplossing_contains** | [**List[str]**](str.md)| Matches values from a comma-separated list: val1,val2,valN. | [optional] 
 **prijs** | **float**| De totale prijs van de gebruikte onderdelen en de uitgevoerde werkzaamheden. | [optional] 
 **prijs_offerte** | **float**| De totale prijs op de offerte voor de te gebruiken onderdelen en de uit te voeren werkzaamheden. | [optional] 
 **prijs_offerte_gt** | **float**| Greater than; number | [optional] 
 **prijs_offerte_gte** | **float**| Greater than or equal to; number | [optional] 
 **prijs_offerte_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prijs_offerte_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prijs_offerte_lt** | **float**| Less than; number | [optional] 
 **prijs_offerte_lte** | **float**| Less than or equal to; number | [optional] 
 **prijs_offerte_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **prijs_gt** | **float**| Greater than; number | [optional] 
 **prijs_gte** | **float**| Greater than or equal to; number | [optional] 
 **prijs_in** | [**List[float]**](float.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prijs_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prijs_lt** | **float**| Less than; number | [optional] 
 **prijs_lte** | **float**| Less than or equal to; number | [optional] 
 **prijs_not** | [**List[float]**](float.md)| Exclude matches; number | [optional] 
 **prioriteit_naam** | **str**| De naam die de soort prioriteit weergeeft. | [optional] 
 **prioriteit_naam_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prioriteit_naam_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **prioriteit_naam_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prioriteit_naam_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **prioriteit_naam_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **prioriteit_opmerking** | **str**| Een opmerking die toegevoegd wordt om de prioritering te verduidelijken. | [optional] 
 **prioriteit_opmerking_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prioriteit_opmerking_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **prioriteit_opmerking_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prioriteit_opmerking_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **prioriteit_opmerking_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **prioriteit_responstijd** | **int**| De toegestane responsetijd voor deze prioriteit.  | [optional] 
 **prioriteit_responstijd_gt** | **int**| Greater than; number | [optional] 
 **prioriteit_responstijd_gte** | **int**| Greater than or equal to; number | [optional] 
 **prioriteit_responstijd_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **prioriteit_responstijd_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **prioriteit_responstijd_lt** | **int**| Less than; number | [optional] 
 **prioriteit_responstijd_lte** | **int**| Less than or equal to; number | [optional] 
 **prioriteit_responstijd_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **probleem** | [**List[str]**](str.md)| Exact; val1,val2 | [optional] 
 **probleem_module_naam** | [**List[str]**](str.md)| Exact; val1,val2 | [optional] 
 **probleem_module_naam_contains** | [**List[str]**](str.md)| Matches values from a comma-separated list: val1,val2,valN. | [optional] 
 **probleem_contains** | [**List[str]**](str.md)| Matches values from a comma-separated list: val1,val2,valN. | [optional] 
 **rangorde_nummer_tickettype** | **int**| Het rangordenummer van het type ticket. | [optional] 
 **rangorde_nummer_tickettype_gt** | **int**| Greater than; number | [optional] 
 **rangorde_nummer_tickettype_gte** | **int**| Greater than or equal to; number | [optional] 
 **rangorde_nummer_tickettype_in** | [**List[int]**](int.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **rangorde_nummer_tickettype_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **rangorde_nummer_tickettype_lt** | **int**| Less than; number | [optional] 
 **rangorde_nummer_tickettype_lte** | **int**| Less than or equal to; number | [optional] 
 **rangorde_nummer_tickettype_not** | [**List[int]**](int.md)| Exclude matches; number | [optional] 
 **reden_afgewezen** | **str**| De reden waarom het ticket de status &#39;afgewezen&#39; heeft gekregen. | [optional] 
 **reden_afgewezen_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **reden_afgewezen_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **reden_afgewezen_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **reden_afgewezen_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **reden_afgewezen_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **referentienummer_leverancier** | **str**| Het referentienummer dat door de leverancier aan het ticket gegeven wordt. | [optional] 
 **referentienummer_leverancier_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **referentienummer_leverancier_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **referentienummer_leverancier_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **referentienummer_leverancier_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **referentienummer_leverancier_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **ticketstatus** | **str**| De status van het ticket. | [optional] 
 **ticketstatus_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **ticketstatus_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **ticketstatus_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **ticketstatus_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **ticketstatus_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 
 **tickettype** | **str**| De naam van het type ticket. | [optional] 
 **tickettype_in** | [**List[str]**](str.md)| Matches any value from a comma-separated list: val1,val2,valN. | [optional] 
 **tickettype_isempty** | **bool**| Whether the field is empty or not. | [optional] 
 **tickettype_isnull** | **bool**| Whether the field has a NULL value or not. | [optional] 
 **tickettype_like** | **str**| Matches text using wildcards (? and *). | [optional] 
 **tickettype_not** | [**List[str]**](str.md)| Exclude matches; text | [optional] 

### Return type

[**Huishoudelijkafvalticket**](Huishoudelijkafvalticket.md)

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

