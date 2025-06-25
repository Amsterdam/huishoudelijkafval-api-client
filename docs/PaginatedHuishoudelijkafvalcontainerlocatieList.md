# PaginatedHuishoudelijkafvalcontainerlocatieList


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**page** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListPage.md) |  | [optional] 
**links** | [**PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks**](PaginatedHuishoudelijkafvaladresLoopafstandV2ListLinks.md) |  | [optional] 
**embedded** | [**PaginatedHuishoudelijkafvalcontainerlocatieListEmbedded**](PaginatedHuishoudelijkafvalcontainerlocatieListEmbedded.md) |  | [optional] 

## Example

```python
from huishoudelijkafval_api_client.models.paginated_huishoudelijkafvalcontainerlocatie_list import PaginatedHuishoudelijkafvalcontainerlocatieList

# TODO update the JSON string below
json = "{}"
# create an instance of PaginatedHuishoudelijkafvalcontainerlocatieList from a JSON string
paginated_huishoudelijkafvalcontainerlocatie_list_instance = PaginatedHuishoudelijkafvalcontainerlocatieList.from_json(json)
# print the JSON string representation of the object
print(PaginatedHuishoudelijkafvalcontainerlocatieList.to_json())

# convert the object into a dict
paginated_huishoudelijkafvalcontainerlocatie_list_dict = paginated_huishoudelijkafvalcontainerlocatie_list_instance.to_dict()
# create an instance of PaginatedHuishoudelijkafvalcontainerlocatieList from a dict
paginated_huishoudelijkafvalcontainerlocatie_list_from_dict = PaginatedHuishoudelijkafvalcontainerlocatieList.from_dict(paginated_huishoudelijkafvalcontainerlocatie_list_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


