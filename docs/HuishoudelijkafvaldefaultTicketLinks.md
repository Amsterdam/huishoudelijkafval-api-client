# HuishoudelijkafvaldefaultTicketLinks

The contents of the `ticket._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalticketLink**](HuishoudelijkafvalticketLink.md) |  | 
**container** | [**HuishoudelijkafvalcontainerLink**](HuishoudelijkafvalcontainerLink.md) |  | 
**containerlocatie** | [**HuishoudelijkafvalcontainerlocatieLink**](HuishoudelijkafvalcontainerlocatieLink.md) |  | 
**gbd_buurt** | [**GebiedenBuurtenRawIdentifier**](GebiedenBuurtenRawIdentifier.md) |  | 
**gbd_wijk** | [**GebiedenWijkenRawIdentifier**](GebiedenWijkenRawIdentifier.md) |  | 
**gbd_stadsdeel** | [**GebiedenStadsdelenRawIdentifier**](GebiedenStadsdelenRawIdentifier.md) |  | 
**gbd_ggw** | [**GebiedenGgwgebiedenRawIdentifier**](GebiedenGgwgebiedenRawIdentifier.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_ticket_links import HuishoudelijkafvaldefaultTicketLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultTicketLinks from a JSON string
huishoudelijkafvaldefault_ticket_links_instance = HuishoudelijkafvaldefaultTicketLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultTicketLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_ticket_links_dict = huishoudelijkafvaldefault_ticket_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultTicketLinks from a dict
huishoudelijkafvaldefault_ticket_links_from_dict = HuishoudelijkafvaldefaultTicketLinks.from_dict(huishoudelijkafvaldefault_ticket_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


