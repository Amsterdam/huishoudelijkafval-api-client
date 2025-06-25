# HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links

The contents of the `bagObjectLoopafstandV2._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalbagObjectLoopafstandV2Link**](HuishoudelijkafvalbagObjectLoopafstandV2Link.md) |  | 
**cluster** | [**HuishoudelijkafvalclusterLink**](HuishoudelijkafvalclusterLink.md) |  | 
**loopafstand_categorie** | [**HuishoudelijkafvalloopafstandCategorieV2Link**](HuishoudelijkafvalloopafstandCategorieV2Link.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_bag_object_loopafstand_v2_links import HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links from a JSON string
huishoudelijkafvaldefault_bag_object_loopafstand_v2_links_instance = HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_bag_object_loopafstand_v2_links_dict = huishoudelijkafvaldefault_bag_object_loopafstand_v2_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links from a dict
huishoudelijkafvaldefault_bag_object_loopafstand_v2_links_from_dict = HuishoudelijkafvaldefaultBagObjectLoopafstandV2Links.from_dict(huishoudelijkafvaldefault_bag_object_loopafstand_v2_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


