# HuishoudelijkafvalticketLink

The identifier of the relationship to ticket.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**href** | **str** |  | [readonly] 
**title** | **str** |  | 
**id** | **int** | Identificerend kenmerk van het ticket. | 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalticket_link import HuishoudelijkafvalticketLink

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalticketLink from a JSON string
huishoudelijkafvalticket_link_instance = HuishoudelijkafvalticketLink.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalticketLink.to_json())

# convert the object into a dict
huishoudelijkafvalticket_link_dict = huishoudelijkafvalticket_link_instance.to_dict()
# create an instance of HuishoudelijkafvalticketLink from a dict
huishoudelijkafvalticket_link_from_dict = HuishoudelijkafvalticketLink.from_dict(huishoudelijkafvalticket_link_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


