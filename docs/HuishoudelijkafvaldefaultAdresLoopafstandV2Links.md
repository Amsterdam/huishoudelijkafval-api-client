# HuishoudelijkafvaldefaultAdresLoopafstandV2Links

The contents of the `adresLoopafstandV2._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvaladresLoopafstandV2Link**](HuishoudelijkafvaladresLoopafstandV2Link.md) |  | 
**cluster** | [**HuishoudelijkafvalclusterLink**](HuishoudelijkafvalclusterLink.md) |  | 
**loopafstand_categorie** | [**HuishoudelijkafvalloopafstandCategorieV2Link**](HuishoudelijkafvalloopafstandCategorieV2Link.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_adres_loopafstand_v2_links import HuishoudelijkafvaldefaultAdresLoopafstandV2Links

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultAdresLoopafstandV2Links from a JSON string
huishoudelijkafvaldefault_adres_loopafstand_v2_links_instance = HuishoudelijkafvaldefaultAdresLoopafstandV2Links.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultAdresLoopafstandV2Links.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_adres_loopafstand_v2_links_dict = huishoudelijkafvaldefault_adres_loopafstand_v2_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultAdresLoopafstandV2Links from a dict
huishoudelijkafvaldefault_adres_loopafstand_v2_links_from_dict = HuishoudelijkafvaldefaultAdresLoopafstandV2Links.from_dict(huishoudelijkafvaldefault_adres_loopafstand_v2_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


