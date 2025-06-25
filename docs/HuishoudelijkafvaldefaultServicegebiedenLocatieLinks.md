# HuishoudelijkafvaldefaultServicegebiedenLocatieLinks

The contents of the `servicegebiedenLocatie._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalservicegebiedenLocatieLink**](HuishoudelijkafvalservicegebiedenLocatieLink.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvaldefault_servicegebieden_locatie_links import HuishoudelijkafvaldefaultServicegebiedenLocatieLinks

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvaldefaultServicegebiedenLocatieLinks from a JSON string
huishoudelijkafvaldefault_servicegebieden_locatie_links_instance = HuishoudelijkafvaldefaultServicegebiedenLocatieLinks.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvaldefaultServicegebiedenLocatieLinks.to_json())

# convert the object into a dict
huishoudelijkafvaldefault_servicegebieden_locatie_links_dict = huishoudelijkafvaldefault_servicegebieden_locatie_links_instance.to_dict()
# create an instance of HuishoudelijkafvaldefaultServicegebiedenLocatieLinks from a dict
huishoudelijkafvaldefault_servicegebieden_locatie_links_from_dict = HuishoudelijkafvaldefaultServicegebiedenLocatieLinks.from_dict(huishoudelijkafvaldefault_servicegebieden_locatie_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


