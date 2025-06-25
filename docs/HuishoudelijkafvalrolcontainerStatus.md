# HuishoudelijkafvalrolcontainerStatus

Deze tabel bevat informatie over de status historie van de rolcontainers.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**links** | [**HuishoudelijkafvaldefaultRolcontainerStatusLinks**](HuishoudelijkafvaldefaultRolcontainerStatusLinks.md) |  | 
**id** | **int** | Unieke aanduiding van een status record | 
**rolcontainer_id** | **int** | Unieke aanduiding van een rolcontainer | [readonly] 
**status** | **str** | Dit attribuut geeft de vorige status van een rolcontainer aan. De volgende statussen zijn mogelijk.  Active, inactive en blocked. | [optional] 
**vanaf_datum** | **datetime** | De datum en tijd waarop de status van een rolcontiner begint. | [optional] 
**tot_datum** | **datetime** | De datum en tijd waarop de satus van een rolcontiner eindigt. | [optional] 
**aanmaakdatum** | **datetime** | Datum tijd waarop de rolcontainer in het systeem is aangemaakt | [optional] 
**wijzigingsdatum** | **datetime** | Datum tijd waarop de rolcontainer in het systeem voor het laatst is aangepast | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.huishoudelijkafvalrolcontainer_status import HuishoudelijkafvalrolcontainerStatus

# TODO update the JSON string below
json = "{}"
# create an instance of HuishoudelijkafvalrolcontainerStatus from a JSON string
huishoudelijkafvalrolcontainer_status_instance = HuishoudelijkafvalrolcontainerStatus.from_json(json)
# print the JSON string representation of the object
print(HuishoudelijkafvalrolcontainerStatus.to_json())

# convert the object into a dict
huishoudelijkafvalrolcontainer_status_dict = huishoudelijkafvalrolcontainer_status_instance.to_dict()
# create an instance of HuishoudelijkafvalrolcontainerStatus from a dict
huishoudelijkafvalrolcontainer_status_from_dict = HuishoudelijkafvalrolcontainerStatus.from_dict(huishoudelijkafvalrolcontainer_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


