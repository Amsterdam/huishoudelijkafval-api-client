# HuishoudelijkafvaldefaultPlanningVoertuigenLinks

The contents of the `planningVoertuigen._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalplanningVoertuigenLink**](HuishoudelijkafvalplanningVoertuigenLink.md) |  | 
**werkzaamheden_datum_ref** | [**ReferentiekalenderdatumLink**](ReferentiekalenderdatumLink.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_planning_voertuigen_links import HuishoudelijkafvaldefaultPlanningVoertuigenLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultPlanningVoertuigenLinks from a JSON string
huishoudelijkafvaldefault_planning_voertuigen_links_instance = HuishoudelijkafvaldefaultPlanningVoertuigenLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultPlanningVoertuigenLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_planning_voertuigen_links_dict = huishoudelijkafvaldefault_planning_voertuigen_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultPlanningVoertuigenLinks from a dict
huishoudelijkafvaldefault_planning_voertuigen_links_from_dict = HuishoudelijkafvaldefaultPlanningVoertuigenLinks.from_dict(huishoudelijkafvaldefault_planning_voertuigen_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


