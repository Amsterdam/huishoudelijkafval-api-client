# PaginatedHuishoudelijkafvalplanningVoertuigenList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalplanningVoertuigenListEmbedded**](PaginatedHuishoudelijkafvalplanningVoertuigenListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalplanning_voertuigen_list import PaginatedHuishoudelijkafvalplanningVoertuigenList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalplanningVoertuigenList from a JSON string
paginated_huishoudelijkafvalplanning_voertuigen_list_instance = PaginatedHuishoudelijkafvalplanningVoertuigenList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalplanningVoertuigenList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalplanning_voertuigen_list_dict = paginated_huishoudelijkafvalplanning_voertuigen_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalplanningVoertuigenList from a dict
paginated_huishoudelijkafvalplanning_voertuigen_list_from_dict = PaginatedHuishoudelijkafvalplanningVoertuigenList.from_dict(paginated_huishoudelijkafvalplanning_voertuigen_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


