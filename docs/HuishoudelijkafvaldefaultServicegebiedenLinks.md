# HuishoudelijkafvaldefaultServicegebiedenLinks

The contents of the `servicegebieden._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalservicegebiedenLink**](HuishoudelijkafvalservicegebiedenLink.md) |  | 
**servicegebieden_locatie** | [**HuishoudelijkafvalservicegebiedenLocatieLink**](HuishoudelijkafvalservicegebiedenLocatieLink.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_servicegebieden_links import HuishoudelijkafvaldefaultServicegebiedenLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultServicegebiedenLinks from a JSON string
huishoudelijkafvaldefault_servicegebieden_links_instance = HuishoudelijkafvaldefaultServicegebiedenLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultServicegebiedenLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_servicegebieden_links_dict = huishoudelijkafvaldefault_servicegebieden_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultServicegebiedenLinks from a dict
huishoudelijkafvaldefault_servicegebieden_links_from_dict = HuishoudelijkafvaldefaultServicegebiedenLinks.from_dict(huishoudelijkafvaldefault_servicegebieden_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


