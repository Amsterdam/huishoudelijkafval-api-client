# HuishoudelijkafvalplanningVoertuigenLink

The identifier of the relationship to planningVoertuigen.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**id** | **int** | Uniek identificerend kenmerk van het record. | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalplanning_voertuigen_link import HuishoudelijkafvalplanningVoertuigenLink

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalplanningVoertuigenLink from a JSON string
huishoudelijkafvalplanning_voertuigen_link_instance = HuishoudelijkafvalplanningVoertuigenLink.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalplanningVoertuigenLink.to_json())

# convert the object into a dict
huishoudelijkafvalplanning_voertuigen_link_dict = huishoudelijkafvalplanning_voertuigen_link_instance.to_dict()
# create an instance of HuishoudelijkafvalplanningVoertuigenLink from a dict
huishoudelijkafvalplanning_voertuigen_link_from_dict = HuishoudelijkafvalplanningVoertuigenLink.from_dict(huishoudelijkafvalplanning_voertuigen_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


