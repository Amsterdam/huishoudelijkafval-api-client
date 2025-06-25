# Huishoudelijkafvalv0AfvoermomentenLinks

The contents of the `afvoermomenten._links` field. It contains all relationships with objects.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**var_schema** | **str** | The schema field is exposed with every record | [readonly] 
**var_self** | [**HuishoudelijkafvalafvoermomentenLink**](HuishoudelijkafvalafvoermomentenLink.md) |  | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalv0_afvoermomenten_links import Huishoudelijkafvalv0AfvoermomentenLinks

# TODO update the JSON string below
json = "{}"
# create an instance of Huishoudelijkafvalv0AfvoermomentenLinks from a JSON string
huishoudelijkafvalv0_afvoermomenten_links_instance = Huishoudelijkafvalv0AfvoermomentenLinks.from_json(json)
# print the JSON string representation of the object
print(Huishoudelijkafvalv0AfvoermomentenLinks.to_json())

# convert the object into a dict
huishoudelijkafvalv0_afvoermomenten_links_dict = huishoudelijkafvalv0_afvoermomenten_links_instance.to_dict()
# create an instance of Huishoudelijkafvalv0AfvoermomentenLinks from a dict
huishoudelijkafvalv0_afvoermomenten_links_from_dict = Huishoudelijkafvalv0AfvoermomentenLinks.from_dict(huishoudelijkafvalv0_afvoermomenten_links_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


